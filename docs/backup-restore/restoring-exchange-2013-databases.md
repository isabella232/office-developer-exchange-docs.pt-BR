---
title: Restaurando Exchange bancos de dados 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: e0804bb1-fd66-448a-b2cb-9ae2726ae888
description: Encontre informações sobre as diferentes maneiras de restaurar seus bancos de dados Exchange 2013.
ms.openlocfilehash: 522128026bcbef893ce4909174d3fd9a95f1e8a9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513273"
---
# <a name="restoring-exchange-2013-databases"></a>Restaurando Exchange bancos de dados 2013

Encontre informações sobre as diferentes maneiras de restaurar seus bancos de dados Exchange 2013. 
  
**Aplica-se a:** Exchange Server 2013 
  
O Exchange que está incluído no Exchange Server 2013 permite alguma flexibilidade na forma como você restaura seus bancos de dados Exchange de dados. Usando o Exchange no Exchange 2013, você pode restaurar seus backups de cópia de sombra para os seguintes locais:
  
- O banco de dados original, independentemente de a configuração do caminho do arquivo de log de transações ou do banco de dados ter sido modificada.
    
- Um banco de dados de recuperação.
    
- Qualquer banco de dados de produção, independentemente de o nome de exibição do banco de dados corresponde ao nome em um conjunto de backup VSS.
    
Quando o aplicativo de restauração restaura informações para o banco de dados original, os arquivos de log devem ser restaurados para o caminho de diretório especificado no Active Directory Domain Services (AD DS) para esse banco de dados. Se o aplicativo restaurar um banco de dados para um local diferente, os arquivos de log devem ser restaurados para uma pasta chamada **_restoredLogs** que está localizada dentro do diretório de arquivos de log do banco de dados. 
  
Ao restaurar para um servidor ou banco de dados diferente do banco de dados original, seu aplicativo de restauração deve certificar-se de que os caminhos de diretório de banco de dados fornecidos para VSS corresponderão àqueles no AD DS. Você pode usar o [cmdlet get-MailboxDatabase](https://technet.microsoft.com/library/bb124924%28v=exchg.150%29.aspx)Exchange Shell de Gerenciamento para obter informações sobre bancos de dados existentes. Para obter mais informações sobre o Exchange Management Shell, confira [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps). 
  
A figura a seguir mostra a sequência de eventos em uma restauração típica de um banco de dados Exchange que é gerenciado pelo Serviço de Cópia de Sombra de Volume (VSS).
  
**Figura 1. Sequência de eventos para restaurar bancos de dados**

![A diagram that shows the sequence of events for the restore process. The sequence begins with the Exchange store startup, and then continues through many steps between the Exchange writer, VSS, and the client application.](media/VSS_StoreWriterRestore.gif)
  
## <a name="restoring-exchange-databases-to-the-original-location"></a>Restaurando Exchange bancos de dados para o local original
<a name="bk_OriginalLocation"> </a>

O Exchange permite que os aplicativos restaurem bancos de dados e arquivos de log de transações para seus locais originais no Exchange servidor. Por padrão, o Exchange replay dos arquivos de log de transação após o solicitante confirmar que a restauração foi concluída durante a [operação OnPostRestore.](https://msdn.microsoft.com/library/windows/desktop/aa381566%28v=vs.85%29.aspx) O aplicativo de restauração deve usar o método VSS [SetAdditionalRestores](https://msdn.microsoft.com/library/windows/desktop/aa382829%28v=vs.85%29.aspx) para evitar a repetição dos arquivos de log. Os arquivos de log podem ser replayados posteriormente quando o administrador Exchange ou seu aplicativo reapresenta o banco de dados restaurado. 
  
Ao restaurar bancos de dados de volta para seus objetos de banco de dados originais (de forma que os GUIDs de destino no banco de dados correspondam àqueles no conjunto de backup), mas para caminhos de arquivo diferentes, o aplicativo deve determinar os caminhos de arquivo atuais e restaurar os arquivos de backup para os caminhos de arquivo correspondentes especificados nas propriedades do banco de dados. O solicitante deve chamar o [método AddNewTarget](https://msdn.microsoft.com/library/windows/desktop/aa382648%28v=vs.85%29.aspx) para se comunicar com o Exchange o local onde os arquivos são restaurados antes que o escritor possa continuar com o restante do processo de restauração. Se **AddNewTarget** não for chamado, o Exchange supõe que os backups sejam restaurados para os caminhos de arquivo especificados no documento de metadados de backup. 
  
Normalmente, seu aplicativo não precisa especificar um novo caminho para backups executados a partir de uma cópia do Grupo de Disponibilidade de Banco de Dados (DAG). Exchange administradores geralmente não alteram caminhos de arquivo de banco de dados ou de log. No entanto, em uma configuração do DAG, o aplicativo de backup pode ter que especificar o banco de dados ativo e os caminhos de log, pois os caminhos de cópia do DAG são sempre diferentes desses caminhos.
  
Observe que Exchange 2013 não dá suporte à restauração de cópias de banco de dados inativas do DAG. Cópias do DAG só podem ser restauradas a partir de dados de backup quando a cópia do banco de dados ativo for restaurada. Usar conjuntos de dados de backup diferentes ou tentar restaurar um subconjunto das cópias do banco de dados pode fazer com que o banco de dados se torne desmontável. Nesse caso, os aplicativos de backup não precisam chamar a função [SetRestoreOptions,](https://msdn.microsoft.com/library/windows/desktop/aa382856%28v=vs.85%29.aspx) pois os backups são restaurados para os objetos de banco de dados originais de onde foram criados. No entanto, se o aplicativo de backup chamar **SetRestoreOptions** e o documento de metadados XML tiver os parâmetros corretos, o resultado não será um erro. 
  
## <a name="restoring-exchange-databases-to-a-recovery-database"></a>Restaurando Exchange bancos de dados para um banco de dados de recuperação
<a name="bk_RecoveryDatabase"> </a>

O Exchange permite restaurar dados diretamente em um banco de dados de recuperação. A montagem dos dados recuperados como um banco de dados de recuperação permite ao administrador Exchange restaurar caixas de correio individuais e até mesmo itens individuais em uma caixa de correio.
  
Se um banco de dados de recuperação já existir, seu aplicativo poderá desmontar o banco de dados, restaurar os dados no banco de dados de recuperação e nos arquivos de log e, em seguida, remontar o banco de dados.
  
Cada Exchange 2013 permite que apenas um banco de dados de recuperação seja montado por vez. O servidor pode conter quantos bancos de dados recuperados o espaço em disco permitir, mas apenas um pode ser montado como o banco de dados de recuperação. O banco de dados montado como o banco de dados de recuperação é contado no número máximo de bancos de dados que podem ser montados por vez. Um banco de dados recuperado montado como banco de dados de recuperação de um servidor não está associado à caixa de correio original de nenhuma maneira.
  
Para recuperar para um banco de dados de recuperação, seu aplicativo deve chamar o [método SetRestoreOptions](https://msdn.microsoft.com/library/windows/desktop/aa382856%28v=vs.85%29.aspx) e fornecer um documento XML que indica as GUIDs de banco de dados de origem e de destino. Os GUIDs de origem devem corresponder aos do conjunto de backup e os GUIDs de destino devem corresponder às entradas de banco de dados de destino no AD DS. O aplicativo de backup também deve chamar o [método AddNewTarget](https://msdn.microsoft.com/library/windows/desktop/aa382648%28v=vs.85%29.aspx) para especificar o caminho do diretório para o qual os arquivos são restaurados. Se os arquivos de banco de dados precisarem ser renomeados, o Exchange de dados renomeará o banco de dados durante a [operação OnPostRestore.](https://msdn.microsoft.com/library/windows/desktop/aa381566%28v=vs.85%29.aspx) Exchange requer que os arquivos de log de transação sejam restaurados para uma subpasta ( **_restoredLogs**) no caminho do arquivo de log de transação atual. Se os arquivos de log são restaurados para qualquer outro local, o Exchange escritor retornará um erro. Como os bancos de dados que estão sendo montados como o banco de dados de recuperação não são restaurados para o local original, eles precisam ser levados para o estado de desligamento limpo antes de serem montados. Por padrão, o Exchange de dados levará todos os bancos de dados restaurados para um estado de desligamento limpo durante a pós-restauração. Se o aplicativo de backup chamar o [método SetAdditionalRestores,](https://msdn.microsoft.com/library/windows/desktop/aa382829%28v=vs.85%29.aspx) o Exchange não repetirá os arquivos de log e o administrador ou seu aplicativo de backup precisará colocar o banco de dados em um estado de desligamento limpo antes de montar o banco de dados. 
  
## <a name="restoring-exchange-databases-to-a-recovery-server"></a>Restaurando Exchange de dados para um servidor de recuperação
<a name="bk_RecoveryServer"> </a>

Em alguns cenários, talvez seja necessário recuperar um conjunto de backup para outro servidor; Por exemplo, talvez seja necessário recuperar de uma falha catastrófica do servidor portando o banco de dados de caixa de correio para outro servidor Exchange 2013 na mesma organização do Exchange ou restaurar para um servidor dedicado fora do ambiente de produção para recuperar dados de caixa de correio e pasta pública. 
  
Nesses cenários, os caminhos de arquivo para o banco de dados de destino, bem como seus GUIDs de objeto são diferentes dos do banco de dados original. Portanto, seu aplicativo precisa chamar o [método SetRestoreOptions](https://msdn.microsoft.com/library/windows/desktop/aa382856%28v=vs.85%29.aspx) com um documento XML que indica as informações de banco de dados de origem e de destino e chamar o [método AddNewTarget](https://msdn.microsoft.com/library/windows/desktop/aa382648%28v=vs.85%29.aspx) para especificar os caminhos de diretório para os quais restaurar os arquivos de backup. Para o Exchange, essa restauração é o mesmo que restaurar para um banco de dados de recuperação. Para obter mais informações, consulte [Restaurando Exchange bancos](restoring-exchange-2013-databases.md#bk_RecoveryDatabase) de dados para um banco de dados de recuperação anteriormente neste artigo. 
  
## <a name="see-also"></a>Confira também
<a name="bk_AdditionalResources"> </a>

- [Tipos de operações de backup para Exchange 2013](types-of-backup-operations-for-exchange-2013.md)
    
- [Criar aplicativos de backup e restauração para Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
    
- [Conceitos de backup e restauração para Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    
- [Referência da classe CChkSGFiles](cchksgfiles-class-reference.md)
    

