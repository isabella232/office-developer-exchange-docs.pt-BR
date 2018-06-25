---
title: Restaurando bancos de dados do Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e0804bb1-fd66-448a-b2cb-9ae2726ae888
description: Encontre informações sobre as diferentes maneiras que você pode restaurar os bancos de dados do Exchange 2013.
ms.openlocfilehash: d3ca3a884b0ad30f7d7968a9ed435b02aaf205e1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750659"
---
# <a name="restoring-exchange-2013-databases"></a>Restaurando bancos de dados do Exchange 2013

Encontre informações sobre as diferentes maneiras que você pode restaurar os bancos de dados do Exchange 2013. 
  
**Aplica-se a:** Exchange Server 2013 
  
O gravador do Exchange que está incluído no Exchange Server 2013 permite alguma flexibilidade em como você restaura seus bancos de dados do Exchange. Usando o gravador do Exchange no Exchange 2013, você pode restaurar os backups de cópia de sombra nos seguintes locais:
  
- Banco de dados original, independentemente se a configuração de caminho de arquivo de log de transação ou de banco de dados foi modificada.
    
- Um banco de dados de recuperação.
    
- Qualquer produção banco de dados, independentemente se o nome de exibição do banco de dados corresponde ao nome de um conjunto de backup do VSS.
    
Quando seu aplicativo de restauração restaura as informações no banco de dados original, os arquivos de log devem ser restaurados para o caminho do diretório especificado nos serviços de domínio Active Directory (AD DS) para esse banco de dados. Se seu aplicativo restaura um banco de dados para um local diferente, os arquivos de log devem ser restaurados para uma pasta denominada **_restoredLogs** que está localizada dentro do diretório de arquivos de log do banco de dados. 
  
Ao restaurar a um servidor ou o banco de dados que é diferente do banco de dados original, seu aplicativo de restauração deve Certifique-se de que os caminhos do diretório de banco de dados fornecidos ao VSS são iguais da AD DS. Você pode usar o cmdlet do Shell de gerenciamento do Exchange de [get-MailboxDatabase](http://technet.microsoft.com/en-us/library/bb124924%28v=exchg.150%29.aspx)para obter mais informações sobre bancos de dados existentes. Para obter mais informações sobre o Shell de gerenciamento do Exchange, consulte [Exchange Server PowerShell (Shell de gerenciamento do Exchange)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps). 
  
A figura a seguir mostra a sequência de eventos em uma restauração típica de um banco de dados do Exchange que é gerenciado pelo serviço de cópia de sombra de Volume (VSS).
  
**Figura 1. Sequência de eventos para a restauração de bancos de dados**

![A diagram that shows the sequence of events for the restore process. The sequence begins with the Exchange store startup, and then continues through many steps between the Exchange writer, VSS, and the client application.](media/VSS_StoreWriterRestore.gif)
  
## <a name="restoring-exchange-databases-to-the-original-location"></a>Restaurando bancos de dados do Exchange para a localização original
<a name="bk_OriginalLocation"> </a>

O gravador do Exchange permite que os aplicativos restaurar bancos de dados e arquivos de log de transação para as localizações originais no servidor Exchange. Por padrão, o gravador do Exchange repete os arquivos de log de transação após o solicitante confirma que a restauração foi concluída durante a operação [OnPostRestore](http://msdn.microsoft.com/en-us/library/windows/desktop/aa381566%28v=vs.85%29.aspx) . O aplicativo de restauração deve usar o método VSS [SetAdditionalRestores](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382829%28v=vs.85%29.aspx) para evitar que os arquivos de log repetidos. Os arquivos de log podem ser repetidos mais tarde quando o administrador do Exchange ou o seu aplicativo remonta o banco de dados restaurado. 
  
Quando os objetos de restauração de bancos de dados para seu banco de dados original (que os GUIDs de destino no banco de dados corresponder no conjunto de backup) mas para caminhos de arquivo diferente, o aplicativo deve determinar os caminhos de arquivo atual e restaurar os arquivos de backup para o caminhos de arquivo correspondentes especificados nas propriedades do banco de dados. O solicitante deve chamar o método [AddNewTarget](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382648%28v=vs.85%29.aspx) para se comunicar com o gravador do Exchange, o local onde os arquivos são restaurados antes que o escritor possa continuar com o restante do processo de restauração. Se **AddNewTarget** não for chamado, o gravador do Exchange pressupõe que os backups serão restaurados os caminhos de arquivo especificados do documento de metadados de backup. 
  
Geralmente, seu aplicativo não precisa especificar um novo caminho para backups que são executadas a partir de uma cópia do grupo de disponibilidade de banco de dados (DAG). Os administradores do Exchange geralmente não altere os caminhos de arquivo de log ou banco de dados. Em uma configuração de DAG, no entanto, o aplicativo de backup pode precisar especificar o banco de dados ativo e log caminhos, porque os caminhos de cópia DAG sempre são diferentes desses caminhos.
  
Observe que o Exchange 2013 não suporta restaurando inativas cópias de banco de dados do DAG. Cópias do DAG podem ser restauradas a partir de dados de backup somente quando a cópia ativa do banco de dados é restaurada. Usando conjuntos de dados de backup diferentes ou tentando restaurar um subconjunto das cópias do banco de dados pode causar o banco de dados para se tornar não montado. Aplicativos de backup não precisará chamar a função de [SetRestoreOptions](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382856%28v=vs.85%29.aspx) neste caso, porque os backups são restaurados para os objetos de banco de dados originais que foram criados a partir. No entanto, se o aplicativo de backup chama **SetRestoreOptions** e o documento de metadados XML tem os parâmetros corretos, o resultado não for um erro. 
  
## <a name="restoring-exchange-databases-to-a-recovery-database"></a>Restaurando bancos de dados do Exchange para um banco de dados de recuperação
<a name="bk_RecoveryDatabase"> </a>

O gravador do Exchange permite restaurar os dados diretamente para um banco de dados de recuperação. Os dados recuperados como um banco de dados de recuperação de montagem permite que o administrador do Exchange restaurar as caixas de correio individuais e até mesmo individuais itens em uma caixa de correio.
  
Se já existir um banco de dados de recuperação, seu aplicativo pode desmontar o banco de dados, restaure os dados para os arquivos de log e de banco de dados de recuperação e monte o banco de dados novamente.
  
Cada servidor Exchange 2013 permite apenas um banco de dados de recuperação deve ser montado por vez. O servidor pode conter quantos recuperados bancos de dados quanto espaço em disco permitir, mas apenas um pode ser montado como o banco de dados de recuperação. O banco de dados montado como o banco de dados de recuperação é contado o número máximo de bancos de dados que podem ser montados por vez. Um banco de dados recuperado montar o banco de dados de recuperação de um servidor não está associado com a caixa de correio original de nenhuma maneira.
  
Para recuperar um banco de dados de recuperação, seu aplicativo deve chamar o método [SetRestoreOptions](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382856%28v=vs.85%29.aspx) e fornecer um documento XML que indica a fonte e os GUIDs de banco de dados de destino. A fonte de GUIDs deve corresponder do conjunto de backup e o GUIDs de destino deve corresponder às entradas de banco de dados de destino no AD DS. O aplicativo de backup também deve chamar o método [AddNewTarget](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382648%28v=vs.85%29.aspx) para especificar o caminho do diretório onde os arquivos são restaurados. Se os arquivos de banco de dados precisam ser renomeados, o gravador do Exchange será renomear o banco de dados durante a operação [OnPostRestore](http://msdn.microsoft.com/en-us/library/windows/desktop/aa381566%28v=vs.85%29.aspx) . Exchange requer os arquivos de log de transações a serem restaurados para uma subpasta ( **_restoredLogs**) sob o caminho de arquivo de log de transação atual. Se os arquivos de log são restaurados para qualquer outro local, o gravador do Exchange retornará um erro. Porque está sendo montados como o banco de dados de recuperação de bancos de dados não são restaurados em seu local original, elas precisam ser transferidos para o estado de desligamento antes que eles podem ser montados. Por padrão, o gravador do Exchange trará todos os bancos de dados restaurados em um estado de desligamento durante post-restore. Se seu aplicativo de backup chama o método [SetAdditionalRestores](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382829%28v=vs.85%29.aspx) , o gravador do Exchange não serão reproduzidas os arquivos de log e o administrador ou seu aplicativo de backup precisa colocar o banco de dados em um estado de desligamento antes da montagem de banco de dados. 
  
## <a name="restoring-exchange-databases-to-a-recovery-server"></a>Restaurando bancos de dados do Exchange para um servidor de recuperação
<a name="bk_RecoveryServer"> </a>

Em alguns cenários, você talvez precise recuperar um conjunto de backup para outro servidor; Por exemplo, você pode precisar recuperar de uma falha grave no servidor pelo portando o banco de dados de caixa de correio para outro servidor Exchange 2013 na mesma organização do Exchange ou restaurar para um servidor dedicado fora do ambiente de produção para recuperar a caixa de correio e dados de pasta pública. 
  
Nesses cenários, os caminhos de arquivo para o banco de dados de destino, bem como seus GUIDs de objeto são diferentes dos processos de banco de dados original. Portanto, o seu aplicativo tem que chamar o método [SetRestoreOptions](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382856%28v=vs.85%29.aspx) com um documento XML que indica a origem e informações do banco de dados de destino e a chamada do método [AddNewTarget](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382648%28v=vs.85%29.aspx) para especificar os caminhos de diretório para restaurar os arquivos de backup . Para o gravador do Exchange, essa restauração é igual ao restaurar um banco de dados de recuperação. Para obter mais informações, consulte [Exchange restaurando bancos de dados para um banco de dados de recuperação](restoring-exchange-2013-databases.md#bk_RecoveryDatabase) neste artigo. 
  
## <a name="see-also"></a>Confira também
<a name="bk_AdditionalResources"> </a>

- [Tipos de operações de backup para o Exchange 2013](types-of-backup-operations-for-exchange-2013.md)
    
- [Criar um backup e restaurar aplicativos para o Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
    
- [Conceitos de backup e restauração do Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    
- [Referência de classe CChkSGFiles](cchksgfiles-class-reference.md)
    

