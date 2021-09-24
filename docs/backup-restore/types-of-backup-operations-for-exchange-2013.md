---
title: Tipos de operações de backup para Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 70510902-9583-4177-be3d-afbf757a1ec0
description: Encontre informações sobre os diferentes tipos de backups que você pode executar em seus bancos de dados de armazenamento Exchange 2013, incluindo backups completos, de cópia, incremental e diferenciais.
ms.openlocfilehash: 79fcdaa40409ee7cac4df44711c1551946b85ca1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520252"
---
# <a name="types-of-backup-operations-for-exchange-2013"></a>Tipos de operações de backup para Exchange 2013

Encontre informações sobre os diferentes tipos de backups que você pode executar em seus bancos de dados de armazenamento Exchange 2013, incluindo backups completos, de cópia, incremental e diferenciais.
  
**Aplica-se a:** Exchange Server 2013 
  
Este artigo fornece informações sobre os diferentes tipos de backups que você pode executar em bancos de dados Exchange Server 2013 e como esses backups afetam os arquivos de banco de dados. 
  
Os aplicativos de backup e restauração que usam o VsS (Serviço de Cópia de Sombra de Volume) e o Exchange de Exchange podem executar os tipos de backups listados na tabela a seguir.
  
**Tabela 1. Tipos de operações de backup**

|**Tipo de backup**|**Descrição**|
|:-----|:-----|
|[Backups completos](types-of-backup-operations-for-exchange-2013.md#bk_FullBackups) <br/> |Faz o back up dos bancos de dados ( .edb), logs de transação ( .log), arquivos de ponto de verificação \* \* ( .chk) e, em seguida, trunca os logs de transação para \* um banco de dados específico.  <br/> |
|[Copiar backups](types-of-backup-operations-for-exchange-2013.md#bk_CopyBackups) <br/> |Faz o back up do banco de dados, logs de transações e arquivos de ponto de verificação. Copiar backups não truncar os logs de transação do banco de dados.  <br/> |
|[Backups incrementais](types-of-backup-operations-for-exchange-2013.md#bk_IncrementalBackups) <br/> |Faz backup dos logs de transação para registrar alterações desde o último backup completo ou incremental e, em seguida, trunca os logs de transação.  <br/> |
|[Backups diferenciais](types-of-backup-operations-for-exchange-2013.md#bk_DifferentialBackups) <br/> |Faz backup dos logs de transação para registrar alterações desde o último backup completo ou incremental e não trunca os logs de transação.  <br/> |
   
Os componentes, ou arquivos de banco de dados, definidos pelo Exchange representam os arquivos de banco de dados e os logs de transação em Exchange bancos de dados 2013. Isso permite que seu aplicativo de backup e restauração exibe os nomes dos componentes em um banco de dados Exchange 2013 durante operações de backup. No entanto, seu aplicativo de backup não pode fazer backup de componentes de banco de dados individuais; ele só pode fazer o back up de bancos de dados inteiros. 
  
O Exchange padroniza os caminhos lógicos do componente de banco de dados, que são especificados nos metadados Exchange de escritor. O Exchange retorna os caminhos lógicos para seu aplicativo de backup e restauração, conforme necessário.
  
O Exchange de dados fornece caminhos lógicos no formulário: 
  
 `logicalPath = "Exchange Server\Microsoft Information Store\<Server name>"`
  
Os componentes do servidor e do banco de dados são componentes do grupo de arquivos, mas não têm arquivos associados. Eles têm subcomponentes que especificam os arquivos individuais. Um banco de dados contém apenas um componente de log, chamado Logs. Os nomes de componentes dos componentes individuais do banco de dados são os GUIDs dos bancos de dados, mostrados como cadeias de caracteres. 
  
O Exchange lista apenas bancos de dados que podem ser backup, com base nas diretrizes da estrutura VSS. Bancos de dados que são montados como o banco de dados de recuperação do Exchange 2013, bem como bancos de dados que não são montados, não podem ser backup e, portanto, não estão listados nos metadados do Exchange do escritor.
  
A figura a seguir mostra o Exchange de backup do escritor. 
  
**Figura 1. Sequência de eventos para o processo de backup**

![A diagram that shows the sequence of events for the backup process. The sequence begins with the Exchange store startups, and then continues through many steps between the Exchange writer, VSS, and the client application.](media/VSS_StoreWriterBackup.gif)
  
## <a name="full-backups"></a>Backups completos
<a name="bk_FullBackups"> </a>

Um backup completo de um banco de dados Exchange envolve a criação e o armazenamento de uma cópia do arquivo de banco de dados, logs de transação e arquivos de ponto de verificação. Um Exchange 2013 tem um conjunto de arquivos de log de transações dedicados.
  
Depois que o banco de dados tiver sido feito backup, os arquivos de log de transação no disco serão truncados para que apenas as alterações de banco de dados que ocorreram após o backup sejam feitas permanecerão. Durante esse processo, o Exchange exclui todas as entradas de log até o ponto de verificação, com base na suposição de que os bancos de dados agora foram backup em um estado consistente que contém todas as alterações até o ponto de verificação mais recente. 
  
Se o banco de dados que está sendo feito backup for desmontado durante a operação de backup, o Exchange 2013 não truncará os logs de transação e o resultado será equivalente a uma operação de backup de cópia, não uma operação de backup completo. 
  
Quando um backup completo é concluído, os headers do banco de dados montado ativo são atualizados com as informações de backup atuais. Em implantações replicadas, essas informações serão comprometidas com um arquivo de log de transações e replicadas para outras cópias do DAG do banco de dados. Os headers das cópias do banco de dados são atualizados à medida que esse arquivo de log de transações é replayado na cópia do banco de dados.
  
Um backup de cópia de sombra completa é necessário para executar backups de cópia de sombra incremental ou diferencial. Os backups completos podem ser retirados de qualquer cópia, desde que seja um backup de cópia de sombra.
  
Backups completos são usados nos seguintes cenários:
  
- Um banco de dados é corrompido ou perdido, mas os arquivos de log de transação no disco estão intactos. Nesse cenário, os arquivos de banco de dados afetados podem ser restaurados do backup completo e, em seguida, recuperados ao repetir os logs de transação que ainda estão no disco. 
    
- Os arquivos de log de transações, bem como o arquivo de banco de dados no disco, são perdidos. Nesse cenário, os arquivos de log de transações que foram backup no momento do backup completo são restaurados juntamente com o banco de dados.
    
No Exchange 2013, os logs podem ser restaurados sem a necessidade de restaurar o banco de dados aplicável de um conjunto de backup completo. Essa opção possibilita que um backup completo anterior seja restaurado e combinado com os arquivos de log de transações do backup completo mais recente para avançar.
  
Quando [a enumeração VSS_BACKUP_TYPE](https://msdn.microsoft.com/library/windows/desktop/aa384679%28v=vs.85%29.aspx) no VSS é definida como **VSS_BT_FULL** quando o Exchange executa um backup, os seguintes componentes são incluídos no backup: 
  
- Um banco de dados com o caminho lógico Exchange Server\Microsoft Information Store<Nome do \\ Servidor<GUID do banco de \> \\ dados\> 
    
- Um arquivo de log com o caminho lógico Exchange Server\Microsoft Information Store \\<Nome do Servidor<GUID do banco de \> \\ dados\> 
    
## <a name="copy-backups"></a>Copiar backups
<a name="bk_CopyBackups"> </a>

Um backup de cópia de um banco de dados Exchange envolve a criação e o armazenamento dos mesmos elementos incluídos em um backup completo. No entanto, ao contrário de um backup completo, os arquivos de log de transação no disco não são truncados quando o backup é concluído. Copiar backups não se destina a fins de recuperação de dados. Em vez disso, os backups de cópia fornecem uma imagem dos dados para uso em testes, diagnósticos de problemas ou para a semeação de uma réplica.
  
Por exemplo, um administrador Exchange 2013 que está enfrentando problemas com o Exchange store pode fazer um backup de cópia para uso em um ambiente de teste sem afetar o sistema de produção. Copiar backups não afeta agendamentos de backup regulares; no entanto, como um backup de cópia também coloca o armazenamento Exchange em um estado de backup em andamento, ele impede que outros backups agendados avancem até que o backup da cópia seja concluído ou abortado. 
  
Quando a [VSS_BACKUP_TYPE](https://msdn.microsoft.com/library/windows/desktop/aa384679%28v=vs.85%29.aspx) no VSS é definida como **VSS_BT_COPY**, os seguintes componentes são incluídos em um backup de cópia: 
  
- Um banco de dados com o caminho lógico Exchange Server\Microsoft Information Store<Nome do \\ Servidor<GUID do banco de \> \\ dados\> 
    
- Um componente de arquivo de log com o caminho lógico Exchange Server\Microsoft Information Store \\<Nome do Servidor<GUID do banco de \> \\ dados\>
    
## <a name="incremental-backups"></a>Backups incrementais
<a name="bk_IncrementalBackups"> </a>

Um backup incremental de um banco de dados Exchange 2013 salva alterações no banco de dados que ocorreram desde o último backup completo ou incremental. Quando todos os arquivos de banco de dados e arquivos de log são restaurados para o sistema, eles podem ser recuperados para o estado em que estavam no momento do último backup incremental. Os dados armazenados em um backup incremental incluem apenas os arquivos de log de transações até o momento atual. 
  
Quando o backup é concluído, Exchange servidor trunca os arquivos de log e marca o tempo de backup nos headers do banco de dados. O uso de um backup incremental para recuperar um banco de dados requer pelo menos dois conjuntos de dados a serem restaurados: o último backup completo e, em seguida, cada backup incremental feito após o último backup completo. A vantagem de usar backups incrementais é que os backups individuais são muito menores do que um backup completo e backups incrementais individuais são frequentemente menores do que backups diferenciais. 
  
A desvantagem de usar backups incrementais é que, se muitos backups incrementais foram feitos entre backups completos, recuperar o armazenamento Exchange pode envolver a recuperação de muitos backups incrementais. Exchange permite que um backup incremental ocorra quando não há backup completo anterior para estabelecer o ponto de partida para as alterações incrementais. 
  
Um backup completo feito de um local de cópia do DAG pode ser seguido por um backup incremental do local ativo e vice-versa. Uma restrição a ter em mente é que o último estado de backup é mantido no header do banco de dados ativo, e as alterações no header do banco de dados são escritas em logs de transação, replicados e repetidos no local do banco de dados de cópia, assim como todos os outros logs de transação em implantações do DAG. Como os backups e restaurações interoperam, os aplicativos de backup podem fornecer a funcionalidade para executar backups exclusivamente em um nó DAG específico, independentemente de o nó estar ativo ou passivo, bem como executar backups exclusivamente do nó passivo ou exclusivamente do nó ativo.
  
Quando a [VSS_BACKUP_TYPE](https://msdn.microsoft.com/library/windows/desktop/aa384679%28v=vs.85%29.aspx) no VSS é definida como **VSS_BT_INCREMENTAL**, os seguintes componentes são incluídos em um backup incremental: 
  
- Um banco de dados com o caminho lógico Exchange Server\Microsoft Information Store<Nome do \\ Servidor<GUID do banco de \> \\ dados\> 
    
- Um arquivo de log com o caminho lógico Exchange Server\Microsoft Information Store \\<Nome do Servidor<GUID do banco de \> \\ dados\>
    
## <a name="differential-backups"></a>Backups diferenciais
<a name="bk_DifferentialBackups"> </a>

Um backup diferencial de um banco de dados Exchange 2013 salva alterações no banco de dados que ocorreram desde o último backup completo ou incremental. Quando os arquivos de banco de dados e os arquivos de log são restaurados pelo sistema, eles podem ser recuperados para o estado em que estavam no último backup diferencial. 
  
Os dados armazenados em um backup diferencial incluem apenas os arquivos de log de transações até o ponto de verificação atual. Os backups diferenciais não excluem ou alteram os arquivos de log ou alteram os headers do banco de dados. Para usar um backup diferencial para recuperar um banco de dados, você só precisa restaurar dois conjuntos de dados: o último backup completo e, em seguida, o backup diferencial mais recente. 
  
A desvantagem de usar backups diferenciais é que os backups diferenciais duplicam os dados de backup em cada backup até que um backup completo seja executado. Se muitos backups diferenciais são feitos entre backups completos, o espaço de armazenamento necessário pode exceder o necessário pelo mesmo número de backups incrementais. Exchange permite que um backup diferencial ocorra quando não houver um backup completo ou incremental para estabelecer o ponto de partida para backups diferenciais.
  
Um backup completo retirado do local da cópia pode ser seguido por um backup diferencial do local ativo e vice-versa. Uma restrição a ter em mente é que o último estado de backup é mantido no header do banco de dados ativo, e as alterações no header do banco de dados são escritas em logs de transação, replicados e repetidos no local do banco de dados de cópia, assim como todos os outros logs de transação em implantações do DAG. Como backups e restaurações interoperam, os aplicativos de backup fornecem a funcionalidade para executar todos os backups exclusivamente em um nó DAG específico, independentemente de o nó estar ativo ou passivo, bem como executar backups exclusivamente do nó passivo ou exclusivamente do nó ativo.
  
Quando a [enumeração VSS_BACKUP_TYPE](https://msdn.microsoft.com/library/windows/desktop/aa384679%28v=vs.85%29.aspx) no VSS é definida como **VSS_BT_DIFFERENTIAL**, os seguintes componentes são incluídos em um backup diferencial: 
  
- Um banco de dados com o caminho lógico Exchange Server\Microsoft Information Store<Nome do \\ Servidor<GUID do banco de \> \\ dados\> 
    
- Um arquivo de log com o caminho lógico Exchange Server\Microsoft Information Store \\<Nome do Servidor<GUID do banco de \> \\ dados\>
    
## <a name="see-also"></a>Confira também
<a name="bk_AdditionalResources"> </a>

- [Criar aplicativos de backup e restauração para Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
    
- [Conceitos de backup e restauração para Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    
- [Restaurando Exchange bancos de dados 2013](restoring-exchange-2013-databases.md)
    
- [Validar a integridade do backup usando a API CHKSGFILES no Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md)
    
- [Validar a integridade do backup usando a ferramenta Eseutil no Exchange 2013](how-to-validate-backup-integrity-by-using-the-eseutil-tool-in-exchange-2013.md)
    

