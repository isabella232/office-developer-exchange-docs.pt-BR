---
title: Exchange escritor no Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: ec126433-9f0a-46ec-a685-ff4af2f97bc1
description: Encontre informações sobre o Exchange no Exchange 2013 para operações de backup e restauração.
ms.openlocfilehash: 7c50c2aa014308b05bdbc1acf0f2a91e33717ed6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516234"
---
# <a name="exchange-writer-in-exchange-2013"></a>Exchange escritor no Exchange 2013

Encontre informações sobre o Exchange no Exchange 2013 para operações de backup e restauração. 
  
**Aplica-se a:** Exchange Server 2013 
  
O Exchange é responsável pelo backup e restauração de bancos de dados Exchange Server 2013 ativos. O Exchange também oferece suporte à funcionalidade de backup para um banco de dados selecionado em que a cópia de sombra é tomada em relação à instância replicada dos arquivos de log de transações e de banco de dados. 
  
## <a name="overview-of-the-exchange-writer"></a>Visão geral do Exchange escritor
<a name="bk_Overview"> </a>

Exchange 2013 inclui recursos de mobilidade de banco de dados, que permitem que os bancos de dados sejam replicados entre diferentes servidores Exchange para melhorar a disponibilidade do banco de dados e a resiliência do site. As outras cópias de banco de dados em um Grupo de Disponibilidade de Banco de Dados (DAG) oferecem uma oportunidade valiosa para que os backups Exchange usem os recursos extras disponíveis no local da cópia. Além disso, como a cópia em vez do mestre do banco de dados ativo é backup, a cópia pode ficar indisponível durante o backup por um período maior de tempo. 
  
O Exchange writer coordena com os serviços Exchange (operando em nome do solicitante) para preparar os arquivos de banco de dados para backups, congelar a atividade de IO resultante de transações de Exchange antes de fazer o backup do banco de dados e, em seguida, descongelar e truncar arquivos de log após a conclusão do backup.
  
Durante uma restauração, seu aplicativo de backup e restauração instrui o Exchange a coordenar com o armazenamento do Exchange (operando em nome do solicitante) para verificar os destinos de restauração, renomear o arquivo de banco de dados se necessário e, em seguida, repetir os logs de transação conforme necessário. O Exchange é compatível com backups e restaurações.
  
O Exchange está disponível em qualquer servidor Exchange que tenha a função de servidor de Caixa de Correio instalada. 
  
## <a name="exchange-writer-configuration-settings"></a>Exchange configurações de escritor
<a name="bk_ExchangeWriterConfig"> </a>

O Exchange para VSS usa uma variedade de configurações e valores que devem ser definidos corretamente e preservados durante operações de backup e restauração. Essas configurações são armazenadas no documento Exchange de metadados do escritor. Se o aplicativo de backup não preservar essas configurações, você poderá ter erros inesperados ao tentar fazer o backup de seus bancos de dados Exchange dados. 
  
A tabela a seguir lista as interfaces VSS que expõem metadados sobre os componentes do backup do banco de dados. Essas interfaces são necessárias para obter o documento de metadados do Exchange de Exchange que é usado para executar um backup do Exchange store.
  
**Tabela 1. Interfaces VSS**

|**Interface VSS**|**Descrição**|
|:-----|:-----|
|IVssWMComponent  <br/> |Permite o acesso a informações de componente armazenadas no Exchange.  <br/> |
|IVssExamineWriterMetadata  <br/> |Permite que o aplicativo de backup e restauração solicite examinar os metadados do Exchange. O documento de metadados do Exchange de escritor contém valores e parâmetros específicos do Exchange 2013 que o aplicativo de backup e restauração requer para que ele possa especificar corretamente os componentes apropriados para backup.  <br/> |
|IVssComponent  <br/> |Contém métodos para examinar e modificar informações sobre componentes contidos no Documento de Componentes de Backup de um solicitante. Os objetos só podem ser obtidos para os componentes que foram adicionados explicitamente a este documento pelo [método IVssBackupComponents::AddComponent.](https://msdn.microsoft.com/library/windows/desktop/aa382646%28v=vs.85%29.aspx)  <br/> |
|IVssBackupComponents  <br/> |Usado pelo aplicativo de backup e restauração solicitando para sondar o Exchange sobre o status do arquivo e executar operações de backup e restauração. O [método IVssBackupComponents::SetBackupState ](https://msdn.microsoft.com/library/windows/desktop/aa382833%28v=vs.85%29.aspx) define se a operação de backup é um backup completo, cópia, incremental ou diferencial. O [método IVssBackupComponents::AddRestoreSubcomponent](https://msdn.microsoft.com/library/windows/desktop/aa382649%28v=vs.85%29.aspx) define os subcomponentes de um banco de dados Exchange 2013 que pode ser selecionado para uma operação de restauração.  <br/> |
   
No sistema de arquivos Windows Server, um banco de dados Exchange 2013 é armazenado como um único arquivo de banco de dados com uma *extensão .edb.* O Exchange do Exchange expõe o .edb como o componente do banco de dados, enquanto os logs de transação (.log) e os arquivos de ponto de verificação (.chk) são combinados em um único componente, conhecido como componente de log. Para obter mais informações sobre Exchange de banco de dados, consulte Conceitos de backup e restauração para Exchange [2013](backup-and-restore-concepts-for-exchange-2013.md).
  
## <a name="interactions-between-the-exchange-writer-vss-and-vss-requesters"></a>Interações entre o Exchange, vss e solicitadores VSS
<a name="bk_interactions"> </a>

A interação de alto nível entre o VSS, o Exchange de Exchange 2013 durante operações de backup é a seguinte:
  
1. O programa de backup (ou agente) executa um trabalho agendado. 
    
2. O solicitante VSS no aplicativo de backup e restauração envia um comando ao VSS para fazer uma cópia de sombra dos bancos de dados Exchange 2013 selecionados. 
    
3. O VSS se comunica com o Exchange para se preparar para um backup de instantâneo. Exchange 2013 proíbe ações administrativas contra bancos de dados, verifica dependências de volume e suspende todas as operações de gravação para a instância selecionada do banco de dados e arquivos de log de transação, permitindo o acesso somente leitura. 
    
4. O VSS se comunica com o provedor de armazenamento apropriado para criar uma cópia de sombra do volume de armazenamento que contém os bancos de dados Exchange 2013. 
    
5. As versões vss Exchange 2013 para retomar operações comuns. 
    
6. O solicitante VSS verifica a consistência física do conjunto de backup antes de sinalizar que o backup foi bem-sucedido. Exchange 2013 trunca os logs de transação (se o banco de dados faz parte de um DAG, a truncamento de log é replicada entre todas as cópias) e registra a hora do último backup do banco de dados.
    
VSS serializa a interação dos solicitantes com o Exchange a partir do [método OnPrepareBackup](https://msdn.microsoft.com/library/windows/desktop/aa381571%28v=vs.85%29.aspx) e termina com o [método OnPostSnapshot.](https://msdn.microsoft.com/library/windows/desktop/aa381568%28v=vs.85%29.aspx) Normalmente, a maior parte do tempo que o Exchange passa trabalhando com a cópia de sombra ocorre após o método **OnPostSnapshot,** quando a consistência da cópia de sombra é verificada antes da conclusão dos backups. O Exchange dá suporte a backups paralelos entre **OnPostSnapshot** [e OnBackupComplete](https://msdn.microsoft.com/library/windows/desktop/aa381557%28v=vs.85%29.aspx).
  
Exchange 2013 não permite backups simultâneos do mesmo banco de dados. Somente um trabalho de backup pode ser executado em um determinado banco de dados ao mesmo tempo. Quando o backup está em execução, o Exchange o armazenamento coloca o banco de dados em um estado de backup em andamento. Esse estado na memória é limpo na conclusão do processo de backup ou quando o serviço é reiniciado. O estado de backup em andamento na memória e seus dados associados são perdidos quando o serviço que hospeda o Exchange é reiniciado, quando o sistema operacional é reiniciado ou quando ocorre um failover de cluster. Qualquer um desses eventos fará com que o trabalho de backup falhe.
  
A truncamento de arquivo de log de transações iniciada pelo backup é disparada com base no tipo de backup a ser executado. Em configurações que não são do DAG, o Exchange truncará os arquivos de log de transações na conclusão de backups completos ou incrementais bem-sucedidos. Em configurações replicadas do DAG, a truncamento de log será adiada pelo serviço de replicação até que todos os arquivos de log necessários sejam reproduzidos em todas as outras cópias. O serviço de replicação excluirá os arquivos de log de backup dos caminhos de arquivo de log ativo e de log de cópia depois de verificar se os arquivos de log foram aplicados com êxito ao banco de dados de cópia e o banco de dados ativo e o ponto de verificação de cópias de banco de dados passou os arquivos de log a serem excluídos.
  
## <a name="see-also"></a>Confira também

- [Logs de transações e arquivos de ponto de verificação para backup e restauração no Exchange 2013](transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange.md)
    
- [Conceitos de backup e restauração para Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    

