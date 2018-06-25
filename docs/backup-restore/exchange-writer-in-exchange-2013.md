---
title: Gravador do Exchange no Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ec126433-9f0a-46ec-a685-ff4af2f97bc1
description: Encontre informações sobre o autor do Exchange no Exchange 2013 para backup e restauração das operações.
ms.openlocfilehash: a4dc5963ab24a83969efc6e425b38a35276f3aa3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750626"
---
# <a name="exchange-writer-in-exchange-2013"></a>Gravador do Exchange no Exchange 2013

Encontre informações sobre o autor do Exchange no Exchange 2013 para backup e restauração das operações. 
  
**Aplica-se a:** Exchange Server 2013 
  
O gravador do Exchange é responsável pelo backup e restauração de bancos de dados ativos do Exchange Server 2013. O gravador do Exchange também dá suporte à funcionalidade de backup para um banco de dados selecionado, onde a cópia de sombra é colocada em relação à instância replicada do banco de dados e transações arquivos de log. 
  
## <a name="overview-of-the-exchange-writer"></a>Visão geral do gravador do Exchange
<a name="bk_Overview"> </a>

Exchange 2013 inclui recursos de mobilidade de banco de dados, que permitem a bancos de dados a serem replicadas entre os servidores Exchange diferentes para melhorar a disponibilidade de banco de dados e resiliência do site. As outras cópias de banco de dados em um grupo de disponibilidade do banco de dados (DAG) fornecem uma oportunidade valiosa para fazer backups do Exchange usar os recursos adicionais que estão disponíveis no local da cópia. Além disso, porque a cópia em vez do mestre de banco de dados ativo é feita o backup, a cópia pode ser indisponível durante o backup para um período de tempo maior. 
  
O gravador do Exchange coordena com os serviços do Exchange (operacional em nome do solicitante) para preparar os arquivos de banco de dados para fazer backups, congelar a atividade de e/s resultante de transações do Exchange antes do backup do banco de dados e descongelar e truncar arquivos de log após o backup for concluído.
  
Durante uma recuperação, o seu aplicativo de backup e restauração instrui o gravador do Exchange para coordenar com o repositório do Exchange (operacional em nome do solicitante) para verificar os destinos de restauração, renomeie o arquivo de banco de dados, se necessário e, em seguida, repetição durante a transação logs conforme necessário. O gravador do Exchange oferece suporte a backups e restaurações.
  
O gravador do Exchange está disponível em qualquer servidor do Exchange que possui a função de servidor de caixa de correio instalada. 
  
## <a name="exchange-writer-configuration-settings"></a>Definições de configuração do Exchange gravador
<a name="bk_ExchangeWriterConfig"> </a>

O gravador VSS do Exchange usa uma variedade de configurações e valores que devem ser definidos corretamente e preservados durante operações de backup e restauração. Essas definições de configuração são armazenadas no documento de metadados do gravador do Exchange. Se seu aplicativo de backup não preservar a essas configurações, você pode sofrer erros inesperados quando você tenta fazer backup de seus bancos de dados do Exchange. 
  
A tabela a seguir lista as interfaces VSS que exponham metadados sobre os componentes do seu backup do banco de dados. Essas interfaces são necessárias para obter o gravador do Exchange documento de metadados que é usado para realizar um backup do repositório do Exchange.
  
**Tabela 1. Interfaces VSS**

|**Interface VSS**|**Descrição**|
|:-----|:-----|
|IVssWMComponent  <br/> |Permite o acesso às informações de componente armazenadas no gravador do Exchange.  <br/> |
|IVssExamineWriterMetadata  <br/> |Permite que o aplicativo solicitante de backup e restauração examinar os metadados do gravador do Exchange. O documento de metadados do gravador Exchange contém valores específicos do Exchange 2013 e os parâmetros que requer que o aplicativo de backup e restauração de solicitação para que ele possa especificar corretamente os componentes apropriados para o backup.  <br/> |
|IVssComponent  <br/> |Contém métodos para examinar e modificar informações sobre os componentes contidos no documento de componentes de Backup de um solicitante. Objetos só podem ser obtidos para esses componentes que tenham sido adicionados explicitamente a este documento pelo método [IVssBackupComponents::AddComponent](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382646%28v=vs.85%29.aspx) .  <br/> |
|IVssBackupComponents  <br/> |Usado pelo aplicativo de backup e restauração solicitante para sondar o gravador do Exchange sobre o status do arquivo e para executar o backup e operações de restauração. O método [IVssBackupComponents::SetBackupState](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382833%28v=vs.85%29.aspx) define se a operação de backup é uma cópia completa, incremental, ou o backup diferencial. O método [IVssBackupComponents::AddRestoreSubcomponent](http://msdn.microsoft.com/en-us/library/windows/desktop/aa382649%28v=vs.85%29.aspx) define os subcomponentes de um banco de dados do Exchange 2013 que podem ser selecionados para uma operação de restauração.  <br/> |
   
Dentro do sistema de arquivo do Windows Server, um banco de dados do Exchange 2013 é armazenado como um arquivo de banco de dados único com uma extensão *. edb. O gravador do Exchange expõe a *. edb como o componente de banco de dados, enquanto os logs de transações (*. log) e arquivos de ponto de verificação (*. chk) são combinados em um único componente, conhecido como o componente de log. Para obter mais informações sobre arquivos de banco de dados do Exchange, consulte [conceitos de Backup e restauração do Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md).
  
## <a name="interactions-between-the-exchange-writer-vss-and-vss-requesters"></a>Interações entre o Exchange gravador VSS e VSS solicitantes
<a name="bk_interactions"> </a>

A interação de alto nível entre o VSS, o gravador do Exchange, e Exchange 2013 durante operações de backup é da seguinte maneira:
  
1. O programa de backup (ou agente) executa um trabalho agendado. 
    
2. O solicitante VSS no aplicativo de backup e restauração envia um comando ao VSS para fazer uma cópia de sombra do bancos de dados selecionados do Exchange 2013. 
    
3. VSS se comunica com o gravador do Exchange para se preparar para um backup de instantâneo. Exchange 2013 proíbe ações administrativas contra os bancos de dados, verifica as dependências de volume e suspende todas as operações de gravação para a instância selecionada dos arquivos de log de banco de dados e transações enquanto permite acesso somente leitura. 
    
4. VSS se comunica com o provedor de armazenamento apropriado para criar uma cópia de sombra de volume de armazenamento que contém os bancos de dados do Exchange 2013. 
    
5. VSS libera o Exchange 2013 para retomar as operações comuns. 
    
6. O solicitante VSS verifica a consistência física do conjunto antes que o backup foi bem-sucedida de sinalização de backup. Exchange 2013 trunca os logs de transações (se o banco de dados for parte de um DAG, truncamento de log é replicado entre todas as cópias) e a hora do último backup do banco de dados de registros.
    
VSS serializa a interação dos solicitantes com o gravador do Exchange, começando com o método [OnPrepareBackup](http://msdn.microsoft.com/en-us/library/windows/desktop/aa381571%28v=vs.85%29.aspx) e terminando com o método [OnPostSnapshot](http://msdn.microsoft.com/en-us/library/windows/desktop/aa381568%28v=vs.85%29.aspx) . Normalmente, a maior parte do tempo que o autor do Exchange gasta como trabalhar com a cópia de sombra ocorre após o método **OnPostSnapshot** , quando a consistência da cópia de sombra é verificada antes da conclusão dos backups. O gravador do Exchange oferece suporte a backups paralelos entre **OnPostSnapshot** e [OnBackupComplete](http://msdn.microsoft.com/en-us/library/windows/desktop/aa381557%28v=vs.85%29.aspx).
  
Exchange 2013 não permite backups simultâneos do mesmo banco de dados. Somente um trabalho de backup pode executar em relação a um determinado banco de dados de uma só vez. Quando o backup estiver sendo executado, o armazenamento do Exchange coloca o banco de dados em um estado de backup em andamento. Nesse estado na memória está desmarcado tanto na conclusão do processo de backup ou quando o serviço for reiniciado. O estado de backup em andamento na memória e seus dados associados são perdidas quando o serviço que hospeda o gravador do Exchange for reiniciado, quando o sistema operacional for reiniciado, ou quando ocorre um failover de cluster. Qualquer um desses eventos fará com que o trabalho de backup falha.
  
Truncamento de arquivo de log de transações iniciadas pelo backup é disparado com base no tipo de backup a ser executada. Nas configurações não são DAG, o gravador do Exchange truncará os arquivos de log de transação na conclusão de backups completos ou incrementais bem-sucedidos. No DAG replicado configurações, truncamento de log será adiado pelo serviço de replicação até que todos os arquivos de log necessários serão repetidos em todas as outras cópias. O serviço de replicação excluirá a quais foi feito backup dos arquivos de log, que ambos da ativa e da cópia caminhos de arquivo de log depois que ele verifica se os arquivos de log tiverem sido aplicados com êxito para o banco de dados de cópia e ambos os banco de dados ativo e o ponto de verificação de cópias de banco de dados passou os arquivos de log a ser excluído.
  
## <a name="see-also"></a>Confira também

- [Logs de transações e arquivos de ponto de verificação de backup e restauração no Exchange 2013](transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange.md)
    
- [Conceitos de backup e restauração do Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    

