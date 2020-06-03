---
title: Restauração de bancos de dados do Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e0804bb1-fd66-448a-b2cb-9ae2726ae888
description: Encontre informações sobre as diferentes maneiras de restaurar os bancos de dados do Exchange 2013.
ms.openlocfilehash: 9fe417bda5dc728af619da02d62ada6e920f731d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528668"
---
# <a name="restoring-exchange-2013-databases"></a>Restauração de bancos de dados do Exchange 2013

Encontre informações sobre as diferentes maneiras de restaurar os bancos de dados do Exchange 2013. 
  
**Aplica-se a:** Exchange Server 2013 
  
O gravador do Exchange incluído no Exchange Server 2013 permite alguma flexibilidade na forma como você restaura os bancos de dados do Exchange. Usando o gravador do Exchange no Exchange 2013, você pode restaurar seus backups de cópia de sombra para os seguintes locais:
  
- O banco de dados original, independentemente se a configuração de caminho do arquivo de log de transações ou banco de dados foi modificada.
    
- Um banco de dados de recuperação.
    
- Qualquer banco de dados de produção, independentemente se o nome de exibição do banco de dados corresponder ao nome em um conjunto de backup VSS.
    
Quando o aplicativo de restauração restaura informações para o banco de dados original, os arquivos de log devem ser restaurados para o caminho de diretório especificado nos serviços de domínio do Active Directory (AD DS) desse banco de dados. Se o aplicativo restaura um banco de dados para um local diferente, os arquivos de log devem ser restaurados para uma pasta chamada **_restoredLogs** que esteja localizada dentro do diretório do arquivo de log do banco de dados. 
  
Ao restaurar para um servidor ou banco de dados que é diferente do banco de dados original, o aplicativo de restauração deve garantir que os caminhos de diretório de banco de dados fornecidos ao VSS correspondam aos do AD DS. Você pode usar o cmdlet [Get-MailboxDatabase](https://technet.microsoft.com/library/bb124924%28v=exchg.150%29.aspx)do Shell de gerenciamento do Exchange para obter informações sobre os bancos de dados existentes. Para obter mais informações sobre o Shell de gerenciamento do Exchange, consulte [Exchange Server PowerShell (Shell de gerenciamento do Exchange)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps). 
  
A figura a seguir mostra a sequência de eventos em uma restauração típica de um banco de dados do Exchange que é gerenciado pelo serviço de cópias de sombra de volume (VSS).
  
**Figura 1. Sequência de eventos para restauração de bancos de dados**

![A diagram that shows the sequence of events for the restore process. The sequence begins with the Exchange store startup, and then continues through many steps between the Exchange writer, VSS, and the client application.](media/VSS_StoreWriterRestore.gif)
  
## <a name="restoring-exchange-databases-to-the-original-location"></a>Restaurar os bancos de dados do Exchange para o local original
<a name="bk_OriginalLocation"> </a>

O gravador do Exchange permite que os aplicativos restaurem os bancos de dados e os arquivos de log de transações em seus locais originais no servidor Exchange. Por padrão, o gravador do Exchange repete os arquivos de log de transações depois que o solicitante confirmar que a restauração foi concluída durante a operação [OnPostRestore](https://msdn.microsoft.com/library/windows/desktop/aa381566%28v=vs.85%29.aspx) . O aplicativo de restauração deve usar o método VSS [SetAdditionalRestores](https://msdn.microsoft.com/library/windows/desktop/aa382829%28v=vs.85%29.aspx) para evitar que os arquivos de log sejam reproduzidos. Os arquivos de log podem ser repetidos posteriormente quando o administrador do Exchange ou seu aplicativo remonta o banco de dados restaurado. 
  
Ao restaurar bancos de dados de volta para seus objetos de banco de dados originais (de modo que os GUIDs de destino do banco de dados correspondam àqueles no conjunto de backup), mas a caminhos de arquivo diferentes, o aplicativo deve determinar os caminhos de arquivo atuais e restaurar os arquivos de backup para os caminhos de arquivo correspondentes especificados nas propriedades do banco de dados. O solicitante deve chamar o método [AddNewTarget](https://msdn.microsoft.com/library/windows/desktop/aa382648%28v=vs.85%29.aspx) para se comunicar com o gravador do Exchange o local onde os arquivos são restaurados antes que o gravador possa continuar com o restante do processo de restauração. Se **AddNewTarget** não for chamado, o gravador do Exchange assumirá que os backups são restaurados para os caminhos de arquivo especificados no documento de metadados de backup. 
  
Normalmente, o aplicativo não precisa especificar um novo caminho para backups executados de uma cópia do DAG (grupo de disponibilidade de banco de dados). Os administradores do Exchange normalmente não alteram os caminhos do arquivo de log ou do banco de dados. No entanto, em uma configuração do DAG, o aplicativo de backup pode ter que especificar o banco de dados ativo e os caminhos de log, porque os caminhos de cópia do DAG são sempre diferentes desses caminhos.
  
Observe que o Exchange 2013 não oferece suporte à restauração de cópias de banco de dados inativas do DAG. As cópias do DAG podem ser restauradas de dados de backup somente quando a cópia do banco de dados ativo é restaurada. O uso de conjuntos de dados de backup diferentes ou a tentativa de restaurar um subconjunto das cópias de banco de dados pode fazer com que o banco de dados se torne não montável. Os aplicativos de backup não precisam chamar a função [Setrestore](https://msdn.microsoft.com/library/windows/desktop/aa382856%28v=vs.85%29.aspx) , neste caso, porque os backups são restaurados para os objetos de banco de dados originais para os quais foram criados. No entanto, se o aplicativo de backup chamar **setrestore** e o documento de metadados XML tiver os parâmetros corretos, o resultado não será um erro. 
  
## <a name="restoring-exchange-databases-to-a-recovery-database"></a>Restaurar bancos de dados do Exchange para um banco de dados de recuperação
<a name="bk_RecoveryDatabase"> </a>

O gravador do Exchange permite que você restaure os dados diretamente para um banco de dados de recuperação. A montagem dos dados recuperados como um banco de dados de recuperação permite que o administrador do Exchange restaure caixas de correio individuais e até mesmo itens individuais em uma caixa de correio.
  
Se um banco de dados de recuperação já existir, seu aplicativo pode desmontar o banco de dados, restaurar os dados para o banco de dados de recuperação e arquivos de log e, em seguida, remontar o banco de dados.
  
Cada servidor Exchange 2013 permite que apenas um banco de dados de recuperação seja montado por vez. O servidor pode conter tantos bancos de dados recuperados quanto o espaço em disco permite, mas apenas um pode ser montado como o banco de dados de recuperação. O banco de dados montado como o banco de dados de recuperação é contado no número máximo de bancos de dados que podem ser montados de cada vez. Um banco de dados recuperado montado como um banco de dados de recuperação do servidor não está associado à caixa de correio original de nenhuma forma.
  
Para recuperar para um banco de dados de recuperação, seu aplicativo deve chamar o método [setrestore](https://msdn.microsoft.com/library/windows/desktop/aa382856%28v=vs.85%29.aspx) e fornecer um documento XML que indica os GUIDs de banco de dados de origem e destino. Os GUIDs de origem devem corresponder àqueles do conjunto de backup e os GUIDs de destino devem corresponder às entradas do banco de dados de destino no AD DS. O aplicativo de backup também deve chamar o método [AddNewTarget](https://msdn.microsoft.com/library/windows/desktop/aa382648%28v=vs.85%29.aspx) para especificar o caminho do diretório no qual os arquivos são restaurados. Se os arquivos de banco de dados precisam ser renomeados, o gravador do Exchange renomeará o banco de dados durante a operação [OnPostRestore](https://msdn.microsoft.com/library/windows/desktop/aa381566%28v=vs.85%29.aspx) . O Exchange exige que os arquivos de log de transações sejam restaurados para uma subpasta ( **_restoredLogs**) no caminho do arquivo de log de transações atual. Se os arquivos de log forem restaurados para qualquer outro local, o gravador do Exchange retornará um erro. Como os bancos de dados que estão sendo montados como o banco de dados de recuperação não são restaurados para o local original, eles precisam ser colocados no estado de desligamento normal antes de serem montados. Por padrão, o gravador do Exchange trará todos os bancos de dados restaurados para um estado de desligamento normal durante o post-Restore. Se o aplicativo de backup chamar o método [SetAdditionalRestores](https://msdn.microsoft.com/library/windows/desktop/aa382829%28v=vs.85%29.aspx) , o gravador do Exchange não repetirá os arquivos de log e o administrador ou o aplicativo de backup precisará trazer o banco de dados para um estado de desligamento normal antes de montar o banco de dados. 
  
## <a name="restoring-exchange-databases-to-a-recovery-server"></a>Restaurar os bancos de dados do Exchange para um servidor de recuperação
<a name="bk_RecoveryServer"> </a>

Em alguns cenários, talvez seja necessário recuperar um conjunto de backup para outro servidor; Por exemplo, talvez você precise se recuperar de uma falha catastrófica no servidor ao portar o banco de dados de caixa de correio para outro servidor Exchange 2013 na mesma organização do Exchange ou restaurar para um servidor dedicado fora do ambiente de produção para recuperar os dados de caixa de correio e pasta pública. 
  
Nesses cenários, os caminhos de arquivo para o banco de dados de destino, bem como seus GUIDs de objeto, são diferentes daqueles para o banco de dados original. Portanto, o aplicativo deve chamar o método [setrestore](https://msdn.microsoft.com/library/windows/desktop/aa382856%28v=vs.85%29.aspx) com um documento XML que indica as informações de banco de dados de origem e destino e chamar o método [AddNewTarget](https://msdn.microsoft.com/library/windows/desktop/aa382648%28v=vs.85%29.aspx) para especificar os caminhos de diretório para os quais os arquivos de backup serão restaurados. Para o gravador do Exchange, essa restauração é a mesma que a restauração para um banco de dados de recuperação. Para obter mais informações, consulte [restaurando bancos de dados do Exchange para um banco de dados de recuperação](restoring-exchange-2013-databases.md#bk_RecoveryDatabase) , anteriormente neste artigo. 
  
## <a name="see-also"></a>Confira também
<a name="bk_AdditionalResources"> </a>

- [Tipos de operações de backup para o Exchange 2013](types-of-backup-operations-for-exchange-2013.md)
    
- [Criar aplicativos de backup e restauração para o Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
    
- [Conceitos de backup e restauração para o Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    
- [Referência de classe função cchksgfiles](cchksgfiles-class-reference.md)
    

