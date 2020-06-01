---
title: Gravador do Exchange no Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ec126433-9f0a-46ec-a685-ff4af2f97bc1
description: Encontre informações sobre o gravador do Exchange no Exchange 2013 para operações de backup e restauração.
ms.openlocfilehash: 44270a87c38b08d274d389fa6e46f3864da13ed2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44452885"
---
# <a name="exchange-writer-in-exchange-2013"></a>Gravador do Exchange no Exchange 2013

Encontre informações sobre o gravador do Exchange no Exchange 2013 para operações de backup e restauração. 
  
**Aplica-se a:** Exchange Server 2013 
  
O gravador do Exchange é responsável pelo backup e pela restauração dos bancos de dados ativos do Exchange Server 2013. O gravador do Exchange também oferece suporte à funcionalidade de backup para um banco de dados selecionado em que a cópia de sombra é realizada em relação à instância replicada dos arquivos de log de transação e banco de dados. 
  
## <a name="overview-of-the-exchange-writer"></a>Visão geral do gravador do Exchange
<a name="bk_Overview"> </a>

O Exchange 2013 inclui recursos de mobilidade de banco de dados, que permitem que os bancos de dados sejam replicados entre diferentes servidores do Exchange para melhorar a disponibilidade do banco de dados e a resiliência do site. As outras cópias de banco de dados em um grupo de disponibilidade de banco de dados (DAG) fornecem uma oportunidade valiosa para que os backups do Exchange usem os recursos extras disponíveis no local da cópia. Além disso, como é feito o backup da cópia em vez do mestre do banco de dados ativo, a cópia pode não estar disponível durante o backup por um período de tempo mais longo. 
  
O gravador do Exchange coordena com os serviços do Exchange (operando em nome do solicitante) para preparar os arquivos de banco de dados para backups, congelar a atividade de e/s resultante de transações do Exchange antes de fazer backup do banco de dados e descongelar e truncar arquivos de log depois que o backup for concluído.
  
Durante uma restauração, o aplicativo de backup e restauração instrui o gravador do Exchange a coordenar com o repositório do Exchange (operando em nome do solicitante) para verificar os destinos de restauração, renomear o arquivo de banco de dados, se necessário, e repetir os logs de transação, conforme necessário. O gravador do Exchange suporta backups e restaurações.
  
O gravador do Exchange está disponível em qualquer servidor do Exchange que tenha a função de servidor caixa de Correio instalada. 
  
## <a name="exchange-writer-configuration-settings"></a>Definições de configuração do Exchange Writer
<a name="bk_ExchangeWriterConfig"> </a>

O gravador do Exchange para VSS usa uma variedade de configurações e valores que devem ser definidos corretamente e preservados durante as operações de backup e restauração. Essas definições de configuração são armazenadas no documento de metadados do gravador do Exchange. Se o aplicativo de backup não preservar essas configurações, você poderá experimentar erros inesperados ao tentar fazer o backup de seus bancos de dados do Exchange. 
  
A tabela a seguir lista as interfaces VSS que expõem metadados sobre os componentes do backup do banco de dados. Essas interfaces são necessárias para obter o documento de metadados do gravador do Exchange que é usado para executar um backup do repositório do Exchange.
  
**Tabela 1. Interfaces VSS**

|**Interface VSS**|**Descrição**|
|:-----|:-----|
|IVssWMComponent  <br/> |Permite o acesso a informações de componente armazenadas no gravador do Exchange.  <br/> |
|IVssExamineWriterMetadata  <br/> |Permite que o aplicativo solicitante de backup e restauração examine os metadados do gravador do Exchange. O documento de metadados do gravador do Exchange contém valores e parâmetros específicos do Exchange 2013 que o aplicativo solicitante de backup e restauração requer para que possa especificar corretamente os componentes apropriados para o backup.  <br/> |
|IVssComponent  <br/> |Contém métodos para examinar e modificar informações sobre componentes contidos em um documento de componentes de backup do solicitante. Os objetos só podem ser obtidos para os componentes que foram explicitamente adicionados a este documento pelo método [IVssBackupComponents:: addComponent](https://msdn.microsoft.com/library/windows/desktop/aa382646%28v=vs.85%29.aspx) .  <br/> |
|IVssBackupComponents  <br/> |Usado pelo aplicativo solicitante de backup e restauração para sondar o gravador do Exchange sobre o status do arquivo e executar operações de backup e restauração. O método [IVssBackupComponents:: Setbackupstate](https://msdn.microsoft.com/library/windows/desktop/aa382833%28v=vs.85%29.aspx) define se a operação de backup é um backup completo, de cópia, incremental ou diferencial. O método [IVssBackupComponents:: AddRestoreSubcomponent](https://msdn.microsoft.com/library/windows/desktop/aa382649%28v=vs.85%29.aspx) define os subcomponentes de um banco de dados do Exchange 2013 que pode ser selecionado para uma operação de restauração.  <br/> |
   
Dentro do sistema de arquivos do Windows Server, um banco de dados do Exchange 2013 é armazenado como um único arquivo de banco de dados com uma extensão *. edb. O gravador do Exchange expõe o *. edb como o componente de banco de dados, enquanto os logs de transações (*. log) e os arquivos de ponto de verificação (*. chk) são combinados em um único componente, chamado de componente de log. Para obter mais informações sobre os arquivos de banco de dados do Exchange, consulte [conceitos de backup e restauração para o Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md).
  
## <a name="interactions-between-the-exchange-writer-vss-and-vss-requesters"></a>Interações entre o gravador do Exchange, o VSS e os solicitantes VSS
<a name="bk_interactions"> </a>

A interação de alto nível entre o VSS, o gravador do Exchange e o Exchange 2013 durante operações de backup é a seguinte:
  
1. O programa de backup (ou agente) executa um trabalho agendado. 
    
2. O solicitante VSS no aplicativo de backup e restauração envia um comando para o VSS para fazer uma cópia de sombra dos bancos de dados do Exchange 2013 selecionados. 
    
3. O VSS se comunica com o gravador do Exchange para se preparar para um backup de instantâneo. O Exchange 2013 proíbe ações administrativas em relação aos bancos de dados, verifica as dependências de volume e suspende todas as operações de gravação para a instância selecionada dos arquivos de log de transações e bancos de dados, permitindo acesso somente leitura. 
    
4. O VSS se comunica com o provedor de armazenamento apropriado para criar uma cópia de sombra do volume de armazenamento que contém os bancos de dados do Exchange 2013. 
    
5. O VSS lança o Exchange 2013 para retomar as operações comuns. 
    
6. O solicitante VSS verifica a consistência física do conjunto de backup antes de sinalizar que o backup foi bem-sucedido. O Exchange 2013 trunca os logs de transações (se o banco de dados fizer parte de um DAG, o truncamento de log é replicado entre todas as cópias) e registra a hora do último backup do banco de dados.
    
O VSS serializa a interação dos solicitantes com o gravador do Exchange começando com o método [OnPrepareBackup](https://msdn.microsoft.com/library/windows/desktop/aa381571%28v=vs.85%29.aspx) e terminando com o método [OnPostSnapshot](https://msdn.microsoft.com/library/windows/desktop/aa381568%28v=vs.85%29.aspx) . Normalmente, a maior parte do tempo que o gravador do Exchange gasta trabalhando com a cópia de sombra ocorre após o método **OnPostSnapshot** , quando a consistência da cópia de sombra é verificada antes da conclusão dos backups. O gravador do Exchange oferece suporte a backups paralelos entre o **OnPostSnapshot** e o [OnBackupComplete](https://msdn.microsoft.com/library/windows/desktop/aa381557%28v=vs.85%29.aspx).
  
O Exchange 2013 não permite backups simultâneos do mesmo banco de dados. Somente um trabalho de backup pode ser executado em um determinado banco de dados ao mesmo tempo. Quando o backup é executado, o repositório do Exchange coloca o banco de dados em um estado de backup em andamento. Esse estado na memória é apagado na conclusão do processo de backup ou quando o serviço é reiniciado. O estado de backup em andamento na memória e seus dados associados são perdidos quando o serviço que hospeda o gravador do Exchange é reiniciado, quando o sistema operacional é reiniciado ou quando ocorre um failover de cluster. Qualquer um desses eventos causará falha no trabalho de backup.
  
O truncamento do arquivo de log de transação iniciado pelo backup é acionado com base no tipo de backup a ser executado. Em configurações não DAG, o gravador do Exchange truncará os arquivos de log de transações na conclusão de backups completos e incrementais bem-sucedidos. Nas configurações replicadas do DAG, o truncamento de log será atrasado pelo serviço de replicação até que todos os arquivos de log necessários sejam repetidos em todas as outras cópias. O serviço de replicação excluirá os arquivos de log de backup dos caminhos de arquivo de log ativo e de cópia depois de verificar se os arquivos de log foram aplicados com êxito ao banco de dados de cópia e ao banco de dados de cópias de banco de dados e se passaram os arquivos de log para serem excluídos.
  
## <a name="see-also"></a>Também consulte

- [Logs de transação e arquivos de ponto de verificação para backup e restauração no Exchange 2013](transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange.md)
    
- [Conceitos de backup e restauração para o Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    

