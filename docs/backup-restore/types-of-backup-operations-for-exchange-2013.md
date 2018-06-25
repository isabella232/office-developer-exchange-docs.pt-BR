---
title: Tipos de operações de backup para o Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 70510902-9583-4177-be3d-afbf757a1ec0
description: Encontre informações sobre os diferentes tipos de backups que você pode executar em seu Exchange 2013 armazenar bancos de dados, incluindo completa, cópia, incremental e os backups diferenciais.
ms.openlocfilehash: 588bc0ffe896f286258006f7f123cf09d28b218c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750674"
---
# <a name="types-of-backup-operations-for-exchange-2013"></a>Tipos de operações de backup para o Exchange 2013

Encontre informações sobre os diferentes tipos de backups que você pode executar em seu Exchange 2013 armazenar bancos de dados, incluindo completa, cópia, incremental e os backups diferenciais.
  
**Aplica-se a:** Exchange Server 2013 
  
Este artigo fornece informações sobre os diferentes tipos de backups que você pode executar em bancos de dados do Exchange Server 2013, e como esses backups afetam os arquivos de banco de dados. 
  
Aplicativos de backup e restauração que usam o serviço de cópia de sombra de Volume (VSS) e o gravador do Exchange podem executar os tipos de backups listados na tabela a seguir.
  
**Tabela 1. Tipos de operações de backup**

|**Tipo de backup**|**Descrição**|
|:-----|:-----|
|[Backups completos](types-of-backup-operations-for-exchange-2013.md#bk_FullBackups) <br/> |Faz o backup dos bancos de dados (\*. edb), logs de transações (\*. log), os arquivos de ponto de verificação (\*. chk) e então trunca os logs de transação para um banco de dados específico.  <br/> |
|[Copiar backups](types-of-backup-operations-for-exchange-2013.md#bk_CopyBackups) <br/> |Faz backup do banco de dados, logs de transações e arquivos de ponto de verificação. Backups de cópia não truncam os logs de transações do banco de dados.  <br/> |
|[Backups incrementais](types-of-backup-operations-for-exchange-2013.md#bk_IncrementalBackups) <br/> |Faz o backup dos logs de transações para registrar as alterações desde o último backup completo ou incremental e, em seguida, trunca os logs de transação.  <br/> |
|[Backups diferenciais](types-of-backup-operations-for-exchange-2013.md#bk_DifferentialBackups) <br/> |Faz o backup dos logs de transações para registrar as alterações desde o último backup completo ou incremental e não trunca os logs de transação.  <br/> |
   
Os componentes, ou os arquivos de banco de dados, definidos pelo gravador do Exchange representam os arquivos de banco de dados e os logs de transação nos bancos de dados do Exchange 2013. Isso permite que o seu aplicativo de backup e restauração para exibir os nomes dos componentes dentro de um banco de dados do Exchange 2013 durante operações de backup. Os aplicativos de backup não permitem backup componentes do banco de dados individual, no entanto; ela só pode fazer backup de bancos de dados inteiros. 
  
O gravador do Exchange padroniza caminhos de lógica de componente banco de dados, que são especificados nos metadados do gravador do Exchange. O gravador do Exchange retorna os caminhos lógicos ao seu aplicativo de backup e restauração, conforme necessário.
  
O gravador do Exchange oferece caminhos lógicos no formato: 
  
 `logicalPath = "Exchange Server\Microsoft Information Store\<Server name>"`
  
Os componentes de servidor e o banco de dados são componentes do grupo de arquivos, mas não têm quaisquer arquivos associados. Eles têm subcomponentes que especificam os arquivos individuais. Um banco de dados contém apenas um componente de log, denominado Logs. Os nomes de componente dos componentes individuais do banco de dados são os GUIDs dos bancos de dados, mostrados como sequências de caracteres. 
  
O gravador do Exchange lista apenas os bancos de dados que podem ser feitos backup, com base nas diretrizes de estrutura VSS. Bancos de dados que são montados como o banco de dados de recuperação Exchange 2013, bem como bancos de dados que não estão montados, não é possível fazer backup e, portanto, não são listados em metadados do gravador do Exchange.
  
A figura a seguir mostra o gravador do Exchange processo de backup. 
  
**Figura 1. Sequência de eventos para o processo de backup**

![A diagram that shows the sequence of events for the backup process. The sequence begins with the Exchange store startups, and then continues through many steps between the Exchange writer, VSS, and the client application.](media/VSS_StoreWriterBackup.gif)
  
## <a name="full-backups"></a>Backups completos
<a name="bk_FullBackups"> </a>

Um backup completo de um banco de dados do Exchange envolve a criação e o armazenamento de uma cópia do arquivo de banco de dados, logs de transações e arquivos de ponto de verificação. Um banco de dados do Exchange 2013 tem um conjunto de arquivos de log de transação dedicado.
  
Depois que o banco de dados foi realizado o backup, os arquivos de log de transação no disco são truncados para que apenas as alterações do banco de dados que ocorreu após o backup foi feito permanecerá inalterado. Durante esse processo, o gravador do Exchange exclui todas as entradas de log até o ponto de verificação, com base na pressuposição de que os bancos de dados agora sofreram backup em um estado consistente que contém todas as alterações de backup para o ponto de verificação mais recente. 
  
Se o banco de dados durante o backup for desmontado durante a operação de backup, Exchange 2013 não irá truncar os logs de transação e o resultado será o equivalente a uma operação de backup de cópia, não uma operação de backup completo. 
  
Quando um backup completo for concluído, os cabeçalhos do banco de dados montado ativo são atualizados com a informação de backup atual. Nas implantações replicadas, essa informação será o compromisso de um arquivo de log de transação e replicada para as outras cópias do banco de dados DAG. Cabeçalhos das cópias do banco de dados são atualizados conforme esse arquivo de log de transação é copiado para a cópia do banco de dados.
  
Um backup de cópia de sombra completo é necessário para poder executar backups de cópia de sombra incremental ou diferencial. Os backups completos podem ser retirados qualquer cópia desde que ela seja uma cópia de sombra backup.
  
Backups completos são usados nos seguintes cenários:
  
- Um banco de dados for corrompido ou é perdido, mas os arquivos de log de transação no disco estão intactos. Neste cenário, os arquivos de banco de dados afetado podem ser restaurados a partir do backup completo e recuperados, em seguida, repetindo os logs de transações que ainda estão no disco. 
    
- Arquivos de log de transações, bem como o arquivo de banco de dados no disco, é perdido. Neste cenário, os arquivos de log de transação que foram feitos o backup no momento do backup completo são restaurados em conjunto com o banco de dados.
    
No Exchange 2013, os logs podem ser restaurados sem precisar restaurar o banco de dados aplicável de um conjunto de backup completo. Essa opção possibilita que um backup completo anterior a ser restaurado e combinado com os arquivos de log de transação do backup completo mais recente para rolar para frente.
  
Quando a enumeração [VSS_BACKUP_TYPE](http://msdn.microsoft.com/en-us/library/windows/desktop/aa384679%28v=vs.85%29.aspx) no VSS estiver definida como **VSS_BT_FULL** quando o escritor Exchange realiza um backup, os seguintes componentes são incluídos no backup: 
  
- Um banco de dados com o repositório de informações do Exchange Server\Microsoft de caminho lógico\\< nome do servidor\>\\< GUID do banco de dados\> 
    
- Um arquivo de log com o repositório de informações do Exchange Server\Microsoft de caminho lógico\\< nome do servidor\>\\< GUID do banco de dados\> 
    
## <a name="copy-backups"></a>Copiar backups
<a name="bk_CopyBackups"> </a>

Uma cópia de backup de um banco de dados do Exchange envolve a criação e armazenar os mesmos elementos incluídos em um backup completo. No entanto, ao contrário com um backup completo, os arquivos de log de transação no disco não são truncados quando o backup for concluído. Backups de cópia não servem para fins de recuperação de dados. Em vez disso, os backups de cópia fornecem uma imagem dos dados para uso em testes de diagnóstico de problemas, ou para uma réplica de propagação.
  
Por exemplo, um administrador do Exchange 2013 que está tendo problemas com o repositório do Exchange pode fazer uma cópia de backup para uso em um ambiente de teste sem afetar o sistema de produção. Backups de cópia não afetam as programações de backup regulares; No entanto, porque uma cópia de backup também coloca o armazenamento do Exchange em um estado de backup em andamento, ele bloqueia outros backups agendados para Avançar até que o backup de cópia é concluído ou cancelado. 
  
Quando a enumeração [VSS_BACKUP_TYPE](http://msdn.microsoft.com/en-us/library/windows/desktop/aa384679%28v=vs.85%29.aspx) no VSS estiver definida como **VSS_BT_COPY**, os seguintes componentes são incluídos em uma cópia de backup: 
  
- Um banco de dados com o repositório de informações do Exchange Server\Microsoft de caminho lógico\\< nome do servidor\>\\< GUID do banco de dados\> 
    
- Um componente do arquivo de log com o repositório de informações do Exchange Server\Microsoft de caminho lógico\\< nome do servidor\>\\< GUID do banco de dados\>
    
## <a name="incremental-backups"></a>Backups incrementais
<a name="bk_IncrementalBackups"> </a>

Um backup incremental de um banco de dados do Exchange 2013 salva alterações no banco de dados que ocorreram desde o último backup completo ou incremental. Quando todos os arquivos de banco de dados e arquivos de log são restaurados no sistema, eles podem ser recuperados para o estado em que estavam no momento do último backup incremental. Os dados armazenados em um backup incremental incluem somente os arquivos de log de transação até a hora atual. 
  
Quando o backup for concluído, o Exchange server trunca os arquivos de log e marca o tempo de backup nos cabeçalhos do banco de dados. Usando um backup incremental para recuperar um banco de dados requer pelo menos dois conjuntos de dados a ser restaurado: o último backup completo e, em seguida, cada backup incremental tomada após o último backup. A vantagem de usar backups incrementais é que os backups individuais são muito menores do que um backup completo e backups incrementais individuais são frequentemente menores do que os backups diferenciais. 
  
As desvantagens de usar backups incrementais é que se muitos backups incrementais feitos entre backups completos, recuperar o armazenamento do Exchange pode envolver recuperando muitos backups incrementais. Exchange não permite um backup incremental ocorra quando não existe nenhum backup completo anterior para estabelecer o ponto de partida para que as alterações incrementais. 
  
Um backup completo tirado de um local de cópia do DAG pode ser seguido de um backup incremental do local ativo e vice-versa. Uma restrição deve ter em mente é que o último estado de backup é mantido no cabeçalho do banco de dados ativo, e as alterações para o cabeçalho de banco de dados são gravadas logs de transações, replicado e reproduzida no local de banco de dados da cópia, assim como todas as outras transações registra em implantações do DAG. Porque os backups e restaurações interoperam, aplicativos de backup podem fornecer a funcionalidade para executar backups exclusivamente em um nó específico do DAG, independentemente se o nó é ativo ou passivo, bem como executar backups exclusivamente a partir do nó passivo ou exclusivamente a partir do nó ativo.
  
Quando a enumeração [VSS_BACKUP_TYPE](http://msdn.microsoft.com/en-us/library/windows/desktop/aa384679%28v=vs.85%29.aspx) no VSS estiver definida como **VSS_BT_INCREMENTAL**, os seguintes componentes são incluídos em um backup incremental: 
  
- Um banco de dados com o repositório de informações do Exchange Server\Microsoft de caminho lógico\\< nome do servidor\>\\< GUID do banco de dados\> 
    
- Um arquivo de log com o repositório de informações do Exchange Server\Microsoft de caminho lógico\\< nome do servidor\>\\< GUID do banco de dados\>
    
## <a name="differential-backups"></a>Backups diferenciais
<a name="bk_DifferentialBackups"> </a>

Um backup diferencial do banco de dados do Exchange 2013 salva alterações no banco de dados que ocorreram desde o último backup completo ou incremental. Quando os arquivos de banco de dados e arquivos de log são restaurados pelo sistema, podem ser recuperados para o estado em que estavam no último backup diferencial. 
  
Os dados armazenados em um backup diferencial incluem somente os arquivos de log de transação até o ponto de verificação atual. Backups diferenciais não excluir ou alterar os arquivos de log ou alterar os cabeçalhos de banco de dados. Para usar um backup diferencial para recuperar um banco de dados, você só precisa restaurar dois conjuntos de dados: o último backup completo e, em seguida, o backup diferencial mais recente. 
  
As desvantagens de usar backups diferenciais é que os backups diferenciais duplicar os quais foi feito backup dos dados em cada backup até que um backup completo é executado. Se muitos backups diferenciais são colocados entre backups completos, o espaço de armazenamento necessário pode exceder exigidos pelo mesmo número de backups incrementais. Exchange não permite um backup diferencial ocorra quando não houve um backup completo ou incremental para estabelecer o ponto de partida para backups diferenciais.
  
Um backup completo extraído do local a cópia pode ser seguido por um backup diferencial do local ativo e vice-versa. Uma restrição deve ter em mente é que o último estado de backup é mantido no cabeçalho do banco de dados ativo, e as alterações para o cabeçalho de banco de dados são gravadas logs de transações, replicado e reproduzida no local de banco de dados da cópia, assim como todas as outras transações registra em implantações do DAG. Porque os backups e restaurações interoperam, aplicativos de backup fornecem a funcionalidade para executar todos os backups exclusivamente em um nó específico do DAG, independentemente se o nó é ativo ou passivo, bem como executar backups exclusivamente a partir do nó passivo ou exclusivamente a partir do nó ativo.
  
Quando a enumeração [VSS_BACKUP_TYPE](http://msdn.microsoft.com/en-us/library/windows/desktop/aa384679%28v=vs.85%29.aspx) no VSS estiver definida como **VSS_BT_DIFFERENTIAL**, os seguintes componentes são incluídos em um backup diferencial: 
  
- Um banco de dados com o repositório de informações do Exchange Server\Microsoft de caminho lógico\\< nome do servidor\>\\< GUID do banco de dados\> 
    
- Um arquivo de log com o repositório de informações do Exchange Server\Microsoft de caminho lógico\\< nome do servidor\>\\< GUID do banco de dados\>
    
## <a name="see-also"></a>Confira também
<a name="bk_AdditionalResources"> </a>

- [Criar um backup e restaurar aplicativos para o Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
    
- [Conceitos de backup e restauração do Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    
- [Restaurando bancos de dados do Exchange 2013](restoring-exchange-2013-databases.md)
    
- [Validar a integridade do backup, usando a API CHKSGFILES no Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md)
    
- [Validar a integridade do backup, usando a ferramenta Eseutil no Exchange 2013](how-to-validate-backup-integrity-by-using-the-eseutil-tool-in-exchange-2013.md)
    

