---
title: Tipos de operações de backup para o Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 70510902-9583-4177-be3d-afbf757a1ec0
description: Encontre informações sobre os diferentes tipos de backups que você pode executar em seus bancos de dados de repositório do Exchange 2013, incluindo backups completos, de cópia, incrementais e diferenciais.
ms.openlocfilehash: dd07226acb3a3bb055e98f861a5c01375ee50dda
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456281"
---
# <a name="types-of-backup-operations-for-exchange-2013"></a>Tipos de operações de backup para o Exchange 2013

Encontre informações sobre os diferentes tipos de backups que você pode executar em seus bancos de dados de repositório do Exchange 2013, incluindo backups completos, de cópia, incrementais e diferenciais.
  
**Aplica-se a:** Exchange Server 2013 
  
Este artigo fornece informações sobre os diferentes tipos de backups que você pode executar em bancos de dados do Exchange Server 2013 e como esses backups afetam os arquivos de banco de dados. 
  
Os aplicativos de backup e restauração que usam o serviço de cópias de sombra de volume (VSS) e o gravador do Exchange podem executar os tipos de backup listados na tabela a seguir.
  
**Tabela 1. Tipos de operações de backup**

|**Tipo de backup**|**Descrição**|
|:-----|:-----|
|[Backups completos](types-of-backup-operations-for-exchange-2013.md#bk_FullBackups) <br/> |Faz backup dos bancos de dados ( \* . edb), dos logs de transações ( \* . log), dos arquivos de ponto de verificação ( \* . chk) e trunca os logs de transação de um banco de dados específico.  <br/> |
|[Copiar backups](types-of-backup-operations-for-exchange-2013.md#bk_CopyBackups) <br/> |Faz backup do banco de dados, dos logs de transações e dos arquivos de ponto de verificação. Os backups de cópia não truncam os logs de transação para o banco de dados.  <br/> |
|[Backups incrementais](types-of-backup-operations-for-exchange-2013.md#bk_IncrementalBackups) <br/> |Faz backup dos logs de transação para registrar alterações desde o último backup completo ou incremental e, em seguida, trunca os logs de transação.  <br/> |
|[Backups diferenciais](types-of-backup-operations-for-exchange-2013.md#bk_DifferentialBackups) <br/> |Faz backup dos logs de transação para registrar alterações desde o último backup completo ou incremental e não trunca os logs de transação.  <br/> |
   
Os componentes ou os arquivos de banco de dados, definidos pelo gravador do Exchange representam os arquivos de banco de dados e os logs de transações nos bancos de dados do Exchange 2013. Isso permite que o aplicativo de backup e restauração exiba os nomes dos componentes dentro de um banco de dados do Exchange 2013 durante operações de backup. No entanto, seu aplicativo de backup não pode fazer backup de componentes de banco de dados individuais; Só é possível fazer backup de bancos de dados inteiros. 
  
O gravador do Exchange padroniza os caminhos lógicos do componente de banco de dados, que são especificados nos metadados do gravador do Exchange. O gravador do Exchange retorna os caminhos lógicos para seu aplicativo de backup e restauração, conforme necessário.
  
O gravador do Exchange fornece caminhos lógicos no formato: 
  
 `logicalPath = "Exchange Server\Microsoft Information Store\<Server name>"`
  
Os componentes do servidor e do banco de dados são componentes de grupo de arquivos, mas não têm arquivos associados. Eles têm subcomponentes que especificam os arquivos individuais. Um banco de dados contém apenas um componente de log, chamado logs. Os nomes de componente dos componentes de banco de dados individuais são os GUIDs dos bancos de dados, exibidos como cadeias de caracteres. 
  
O gravador do Exchange lista os bancos de dados que podem ser copiados com base nas diretrizes da estrutura do VSS. Os bancos de dados montados como o banco de dados de recuperação do Exchange 2013, bem como os bancos de dados não montados, não podem ser copiados e, portanto, não são listados nos metadados do gravador do Exchange.
  
A figura a seguir mostra o processo de backup do gravador do Exchange. 
  
**Figura 1. Sequência de eventos para o processo de backup**

![A diagram that shows the sequence of events for the backup process. The sequence begins with the Exchange store startups, and then continues through many steps between the Exchange writer, VSS, and the client application.](media/VSS_StoreWriterBackup.gif)
  
## <a name="full-backups"></a>Backups completos
<a name="bk_FullBackups"> </a>

Um backup completo de um banco de dados do Exchange envolve a criação e o armazenamento de uma cópia do arquivo de banco de dados, logs de transações e arquivos de ponto de verificação. Um banco de dados do Exchange 2013 tem um conjunto de arquivos de log de transação dedicados.
  
Após o backup do banco de dados, os arquivos de log de transações no disco são truncados para que apenas as alterações de banco de dados que ocorreram depois que o backup foi feito permanecerão. Durante esse processo, o gravador do Exchange exclui todas as entradas de log até o ponto de verificação, com base na suposição de que o backup dos bancos de dados já foi feito em um estado consistente que contém todas as alterações até o ponto de verificação mais recente. 
  
Se o banco de dados que está sendo armazenado em backup estiver desmontado durante a operação de backup, o Exchange 2013 não truncará os logs de transação e o resultado será o equivalente a uma operação de backup de cópia, não uma operação de backup completo. 
  
Quando um backup completo é concluído, os cabeçalhos do banco de dados montado ativo são atualizados com as informações de backup atuais. Em implantações replicadas, essas informações serão confirmadas em um arquivo de log de transações e replicadas para as outras cópias do DAG do banco de dados. Os cabeçalhos das cópias de banco de dados são atualizados, pois esse arquivo de log de transações é reproduzido na cópia do banco de dados.
  
Um backup completo de cópia de sombra é necessário para executar backups de cópia de sombra incremental ou diferencial. Os backups completos podem ser feitos de qualquer cópia, desde que seja um backup de cópia de sombra.
  
Os backups completos são usados nos seguintes cenários:
  
- Um banco de dados é corrompido ou perdido, mas os arquivos de log de transações no disco estão intactos. Neste cenário, os arquivos de banco de dados afetados podem ser restaurados do backup completo e, em seguida, recuperados por meio da repetição dos logs de transação que ainda estão no disco. 
    
- Arquivos de log de transações, bem como o arquivo de banco de dados no disco, são perdidos. Neste cenário, os arquivos de log de transações que foram copiados no momento do backup completo são restaurados junto com o banco de dados.
    
No Exchange 2013, os logs podem ser restaurados sem a necessidade de restaurar o banco de dados aplicável a partir de um conjunto de backup completo. Essa opção permite que um backup completo anterior seja restaurado e combinado com os arquivos de log de transações do backup completo mais recente para frente.
  
Quando a enumeração [VSS_BACKUP_TYPE](https://msdn.microsoft.com/library/windows/desktop/aa384679%28v=vs.85%29.aspx) no VSS estiver definida como **VSS_BT_FULL** quando o gravador do Exchange executar um backup, os seguintes componentes serão incluídos no backup: 
  
- Um banco de dados com o caminho lógico Exchange Server\Microsoft Information Store \\<nome do servidor \> \\<GUID do banco de dados\> 
    
- Um arquivo de log com o caminho lógico Exchange Server\Microsoft Information Store \\<nome do servidor \> \\<GUID do banco de dados\> 
    
## <a name="copy-backups"></a>Copiar backups
<a name="bk_CopyBackups"> </a>

Um backup de cópia de um banco de dados do Exchange envolve a criação e o armazenamento dos mesmos elementos que estão incluídos em um backup completo. No entanto, ao contrário de um backup completo, os arquivos de log de transações no disco não são truncados quando o backup é concluído. Os backups de cópia não se destinam a fins de recuperação de dados. Em vez disso, os backups de cópia fornecem uma imagem dos dados para uso em testes, diagnóstico de problemas ou para propagação de uma réplica.
  
Por exemplo, um administrador do Exchange 2013 que está tendo problemas com o repositório do Exchange pode fazer um backup de cópia para uso em um ambiente de teste sem afetar o sistema de produção. Os backups copiados não afetam os agendamentos regulares de backup; no entanto, como um backup de cópia também coloca o armazenamento do Exchange em um estado de backup em andamento, bloqueia outros backups agendados para prosseguir até que o backup da cópia seja concluído ou anulado. 
  
Quando a enumeração [VSS_BACKUP_TYPE](https://msdn.microsoft.com/library/windows/desktop/aa384679%28v=vs.85%29.aspx) no VSS é definida como **VSS_BT_COPY**, os seguintes componentes são incluídos em um backup de cópia: 
  
- Um banco de dados com o caminho lógico Exchange Server\Microsoft Information Store \\<nome do servidor \> \\<GUID do banco de dados\> 
    
- Um componente de arquivo de log com o caminho lógico Exchange Server\Microsoft Information Store \\<nome do servidor \> \\<GUID do banco de dados\>
    
## <a name="incremental-backups"></a>Backups incrementais
<a name="bk_IncrementalBackups"> </a>

Um backup incremental de um banco de dados do Exchange 2013 salva as alterações no banco de dados que ocorreram desde o último backup completo ou incremental. Quando todos os arquivos de banco de dados e arquivos de log são restaurados no sistema, eles podem ser recuperados para o estado em que estavam no momento do último backup incremental. Os dados armazenados em um backup incremental incluem apenas os arquivos de log de transações até o momento atual. 
  
Quando o backup for concluído, o servidor do Exchange truncará os arquivos de log e marcará o tempo de backup nos cabeçalhos do banco de dados. O uso de um backup incremental para recuperar um banco de dados requer pelo menos dois conjuntos de dados a serem restaurados: o último backup completo e, em seguida, cada backup incremental feito após o último backup completo. A vantagem de usar backups incrementais é que os backups individuais são muito menores do que um backup completo e backups incrementais individuais são frequentemente menores do que os backups diferenciais. 
  
A desvantagem de usar backups incrementais é que, se vários backups incrementais foram feitos entre backups completos, a recuperação do repositório do Exchange pode envolver a recuperação de vários backups incrementais. O Exchange não permite que um backup incremental ocorra quando não existir nenhum backup completo anterior para estabelecer o ponto de partida para as alterações incrementais. 
  
Um backup completo obtido de um local de cópia do DAG pode ser seguido por um backup incremental do local ativo e vice-versa. Uma restrição para ter em mente é que o último estado de backup é mantido no cabeçalho do banco de dados ativo, e as alterações no cabeçalho do banco de dados são gravadas nos logs de transações, replicadas e reproduzidas no local do banco de dados de cópia, assim como todos os outros logs de transações em implantações do DAG. Como backups e restaurações de interoperabilidade, os aplicativos de backup podem fornecer a funcionalidade para executar backups exclusivamente em um nó DAG específico, independentemente de o nó estar ativo ou passivo, bem como para executar backups exclusivamente do nó passivo ou exclusivamente a partir do nó ativo.
  
Quando a enumeração [VSS_BACKUP_TYPE](https://msdn.microsoft.com/library/windows/desktop/aa384679%28v=vs.85%29.aspx) no VSS é definida como **VSS_BT_INCREMENTAL**, os seguintes componentes são incluídos em um backup incremental: 
  
- Um banco de dados com o caminho lógico Exchange Server\Microsoft Information Store \\<nome do servidor \> \\<GUID do banco de dados\> 
    
- Um arquivo de log com o caminho lógico Exchange Server\Microsoft Information Store \\<nome do servidor \> \\<GUID do banco de dados\>
    
## <a name="differential-backups"></a>Backups diferenciais
<a name="bk_DifferentialBackups"> </a>

Um backup diferencial de um banco de dados do Exchange 2013 salva as alterações no banco de dados que ocorreram desde o último backup completo ou incremental. Quando os arquivos de banco de dados e os arquivos de log são restaurados pelo sistema, eles podem ser recuperados para o estado em que estavam no último backup diferencial. 
  
Os dados armazenados em um backup diferencial incluem apenas os arquivos de log de transações até o ponto de verificação atual. Backups diferenciais não excluem ou alteram os arquivos de log ou alteram os cabeçalhos de banco de dados. Para usar um backup diferencial para recuperar um banco de dados, você só precisa restaurar dois conjuntos de dados: o último backup completo e, em seguida, o backup diferencial mais recente. 
  
A desvantagem de usar backups diferenciais é que os backups diferenciais duplicam os dados de backup em cada backup até que um backup completo seja realizado. Se vários backups diferenciais forem feitos entre backups completos, o espaço de armazenamento necessário pode exceder o necessário pelo mesmo número de backups incrementais. O Exchange não permite que um backup diferencial ocorra quando não houve um backup completo ou incremental para estabelecer o ponto de partida para backups diferenciais.
  
Um backup completo obtido do local de cópia pode ser seguido por um backup diferencial do local ativo e vice-versa. Uma restrição para ter em mente é que o último estado de backup é mantido no cabeçalho do banco de dados ativo, e as alterações no cabeçalho do banco de dados são gravadas nos logs de transações, replicadas e reproduzidas no local do banco de dados de cópia, assim como todos os outros logs de transações em implantações do DAG. Como backups e restaurações de interoperabilidade, os aplicativos de backup fornecem a funcionalidade para executar todos os backups exclusivamente em um nó DAG específico, independentemente se o nó está ativo ou passivo, bem como para executar backups exclusivamente do nó passivo ou exclusivamente a partir do nó ativo.
  
Quando a enumeração [VSS_BACKUP_TYPE](https://msdn.microsoft.com/library/windows/desktop/aa384679%28v=vs.85%29.aspx) no VSS é definida como **VSS_BT_DIFFERENTIAL**, os seguintes componentes estão incluídos em um backup diferencial: 
  
- Um banco de dados com o caminho lógico Exchange Server\Microsoft Information Store \\<nome do servidor \> \\<GUID do banco de dados\> 
    
- Um arquivo de log com o caminho lógico Exchange Server\Microsoft Information Store \\<nome do servidor \> \\<GUID do banco de dados\>
    
## <a name="see-also"></a>Confira também
<a name="bk_AdditionalResources"> </a>

- [Criar aplicativos de backup e restauração para o Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
    
- [Conceitos de backup e restauração para o Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    
- [Restauração de bancos de dados do Exchange 2013](restoring-exchange-2013-databases.md)
    
- [Validar a integridade do backup usando a API CHKSGFILES no Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md)
    
- [Validar a integridade do backup usando a ferramenta Eseutil no Exchange 2013](how-to-validate-backup-integrity-by-using-the-eseutil-tool-in-exchange-2013.md)
    

