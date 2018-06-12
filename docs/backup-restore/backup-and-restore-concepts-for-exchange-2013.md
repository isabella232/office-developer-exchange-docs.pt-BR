---
title: Conceitos de backup e restauração do Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9a1c4709-9313-4ccf-9f8a-673a51d51f23
description: Encontre informações sobre bancos de dados do Exchange que ajudarão você a criar o backup e restaurar aplicativos para o Exchange 2013.
ms.openlocfilehash: 5fa62c3d34ffbe8f0bab852c6d41c49220e2883a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750635"
---
# <a name="backup-and-restore-concepts-for-exchange-2013"></a><span data-ttu-id="80484-103">Conceitos de backup e restauração do Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="80484-103">Backup and restore concepts for Exchange 2013</span></span>

<span data-ttu-id="80484-104">Encontre informações sobre bancos de dados do Exchange que ajudarão você a criar o backup e restaurar aplicativos para o Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="80484-104">Find information about Exchange databases that will help you create your backup and restore applications for Exchange 2013.</span></span>
  
<span data-ttu-id="80484-105">Antes de criar um backup e restaurar aplicativos para o Exchange Server 2013, você deve estar familiarizado com a estrutura de arquivos de banco de dados do Exchange.</span><span class="sxs-lookup"><span data-stu-id="80484-105">Before you create backup and restore applications for Exchange Server 2013, you should be familiar with the Exchange database file structure.</span></span> <span data-ttu-id="80484-106">Usando os arquivos de banco de dados de repositório do Exchange, você pode fazer backup dos dados no seu armazenamento e restaurá-lo mais tarde conforme necessário.</span><span class="sxs-lookup"><span data-stu-id="80484-106">By using the Exchange store database files, you can back up the data in your store and restore it at a later time as needed.</span></span> <span data-ttu-id="80484-107">Se você está limitado a espaço em disco, o administrador pode implementar o log circular e isso afetará sua capacidade de fazer backup do banco de dados.</span><span class="sxs-lookup"><span data-stu-id="80484-107">If you are limited on disk space, your administrator might implement circular logging, and this will affect your ability to back up the database.</span></span> <span data-ttu-id="80484-108">Você também pode tirar proveito do recurso de mobilidade de banco de dados no Exchange 2013 para fazer backup e restaurar dados do Exchange.</span><span class="sxs-lookup"><span data-stu-id="80484-108">You can also take advantage of the database mobility feature in Exchange 2013 to back up and restore Exchange data.</span></span> <span data-ttu-id="80484-109">Mobilidade de banco de dados, em combinação com o seu aplicativo de backup e restauração, é uma boa medida de redundância para recuperação de desastres.</span><span class="sxs-lookup"><span data-stu-id="80484-109">Database mobility, in combination with your backup and restore application, is a good measure of redundancy for disaster recovery.</span></span>

<span data-ttu-id="80484-110"><a name="bk_exchangedatabases"> </a></span><span class="sxs-lookup"><span data-stu-id="80484-110"></span></span>

## <a name="exchange-store-database-files"></a><span data-ttu-id="80484-111">Arquivos de banco de dados de repositório do Exchange</span><span class="sxs-lookup"><span data-stu-id="80484-111">Exchange store database files</span></span>

<span data-ttu-id="80484-112">Exchange 2013 inclui o suporte para até 100 bancos de dados.</span><span class="sxs-lookup"><span data-stu-id="80484-112">Exchange 2013 includes support for up to 100 databases.</span></span> <span data-ttu-id="80484-113">Cada banco de dados do Exchange 2013 contém os arquivos listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="80484-113">Each Exchange 2013 database contains the files listed in the following table.</span></span> 
  
<span data-ttu-id="80484-114">**Tabela 1. Arquivos de banco de dados do Exchange 2013**</span><span class="sxs-lookup"><span data-stu-id="80484-114">**Table 1. Exchange 2013 database files**</span></span>

|<span data-ttu-id="80484-115">Tipo de arquivo</span><span class="sxs-lookup"><span data-stu-id="80484-115">File type</span></span>|<span data-ttu-id="80484-116">Extensão</span><span class="sxs-lookup"><span data-stu-id="80484-116">Extension</span></span>|<span data-ttu-id="80484-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="80484-117">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="80484-118">Arquivo de banco de dados</span><span class="sxs-lookup"><span data-stu-id="80484-118">Database file</span></span>  <br/> |<span data-ttu-id="80484-119">\*. edb</span><span class="sxs-lookup"><span data-stu-id="80484-119">\*.edb</span></span>  <br/> |<span data-ttu-id="80484-120">Registra todas as alterações que foram confirmadas no banco de dados na memória.</span><span class="sxs-lookup"><span data-stu-id="80484-120">Records all the changes that have been committed to the in-memory database.</span></span>  <br/> |
|<span data-ttu-id="80484-121">Fluxo de log de transação</span><span class="sxs-lookup"><span data-stu-id="80484-121">Transaction log stream</span></span>  <br/> |<span data-ttu-id="80484-122">\*. log</span><span class="sxs-lookup"><span data-stu-id="80484-122">\*.log</span></span>  <br/> |<span data-ttu-id="80484-123">Operações de registros, como a criação ou modificação de uma mensagem, que serão confirmada no banco de dados.</span><span class="sxs-lookup"><span data-stu-id="80484-123">Records operations, such as the creation or modification of a message, that will be committed to the database.</span></span> <span data-ttu-id="80484-124">Limite de tamanho para 1 MB.</span><span class="sxs-lookup"><span data-stu-id="80484-124">Limited in size to 1 MB each.</span></span>  <br/> |
|<span data-ttu-id="80484-125">Arquivo de verificação</span><span class="sxs-lookup"><span data-stu-id="80484-125">Checkpoint file</span></span>  <br/> |<span data-ttu-id="80484-126">\*. chk</span><span class="sxs-lookup"><span data-stu-id="80484-126">\*.chk</span></span>  <br/> |<span data-ttu-id="80484-127">Registros que conectado transações tem sido escritos para os arquivos de banco de dados no disco.</span><span class="sxs-lookup"><span data-stu-id="80484-127">Records which logged transactions have been written to the on-disk database files.</span></span>  <br/> |
   
<span data-ttu-id="80484-128">Exchange 2013 mantém um único conjunto de arquivos de log de transações para cada banco de dados.</span><span class="sxs-lookup"><span data-stu-id="80484-128">Exchange 2013 maintains a single set of transaction log files for each database.</span></span> <span data-ttu-id="80484-129">Os logs de transações são importantes para operações de backup e recuperação.</span><span class="sxs-lookup"><span data-stu-id="80484-129">The transaction logs are important for backup and recovery operations.</span></span> <span data-ttu-id="80484-130">Quando você cria um backup e restaurar o aplicativo que usa o serviço de cópia de sombra de Volume (VSS), certifique-se de que você manipule esses logs corretamente.</span><span class="sxs-lookup"><span data-stu-id="80484-130">When you create a backup and restore application that uses the Volume Shadow Copy Service (VSS), you must ensure that you handle these logs correctly.</span></span> <span data-ttu-id="80484-131">Para obter mais informações, consulte os [logs de transações e arquivos de ponto de verificação de backup e restauração no Exchange 2013](transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="80484-131">For more information, see [Transaction logs and checkpoint files for backup and restore in Exchange 2013](transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange.md).</span></span> <span data-ttu-id="80484-132">Para fazer backup de um banco de dados e seu fluxo de log, você deve fazer backup de todo o volume que contém o banco de dados e logs.</span><span class="sxs-lookup"><span data-stu-id="80484-132">To back up a database and its log stream, you must back up the entire volume that contains the database and logs.</span></span> <span data-ttu-id="80484-133">Truncamento de log ocorrerá apenas após a conclusão bem-sucedida de um backup completo de um volume ou pastas que contêm um banco de dados do Exchange.</span><span class="sxs-lookup"><span data-stu-id="80484-133">Log truncation will occur only after a successful completion of a full backup of a volume or folders that contain an Exchange database.</span></span>
  
<span data-ttu-id="80484-134">Em cada servidor do Exchange, você pode montá apenas um banco de dados de recuperação por vez.</span><span class="sxs-lookup"><span data-stu-id="80484-134">On each Exchange server, you can mount only one recovery database at a time.</span></span> <span data-ttu-id="80484-135">Você pode acessar o banco de dados de recuperação usando cmdlets do Shell de gerenciamento do Exchange como **New-MailboxRestoreRequest**.</span><span class="sxs-lookup"><span data-stu-id="80484-135">You can access the recovery database by using Exchange Management Shell cmdlets such as **New-MailboxRestoreRequest**.</span></span> <span data-ttu-id="80484-136">Para obter mais informações sobre bancos de dados do Exchange recuperação, consulte [Recovery Databases](http://technet.microsoft.com/en-us/library/dd876954%28v=exchg.150%29.aspx) no TechNet.</span><span class="sxs-lookup"><span data-stu-id="80484-136">For more information about Exchange recovery databases, see [Recovery Databases](http://technet.microsoft.com/en-us/library/dd876954%28v=exchg.150%29.aspx) on TechNet.</span></span> <span data-ttu-id="80484-137">Para obter mais informações sobre os cmdlets do Shell de gerenciamento do Exchange, consulte [Os Cmdlets do Exchange 2013](http://technet.microsoft.com/en-us/library/bb124413.aspx) no TechNet.</span><span class="sxs-lookup"><span data-stu-id="80484-137">For more information about Exchange Management Shell cmdlets, see [Exchange 2013 Cmdlets](http://technet.microsoft.com/en-us/library/bb124413.aspx) on TechNet.</span></span> 
  
## <a name="circular-logging"></a><span data-ttu-id="80484-138">Log circular</span><span class="sxs-lookup"><span data-stu-id="80484-138">Circular logging</span></span>
<span data-ttu-id="80484-139"><a name="bk_circularlogging"> </a></span><span class="sxs-lookup"><span data-stu-id="80484-139"></span></span>

<span data-ttu-id="80484-140">Se a capacidade de armazenamento é um problema, o administrador pode habilitar log circular.</span><span class="sxs-lookup"><span data-stu-id="80484-140">If storage capacity is an issue, your administrator might enable circular logging.</span></span> <span data-ttu-id="80484-141">Quando o log circular estiver habilitado, o Exchange grava os logs de transação como de costume, mas quando um arquivo de ponto de verificação é avançado, a parte inativa do log de transação será truncada.</span><span class="sxs-lookup"><span data-stu-id="80484-141">When circular logging is enabled, Exchange writes transaction logs as usual, but when a checkpoint file is advanced, the inactive portion of the transaction log is truncated.</span></span> <span data-ttu-id="80484-142">O administrador não deve configurar os bancos de dados do Exchange 2013 para usar o log circular, se você planeja usar o VSS para habilitar o seu backup personalizado e operações de restauração.</span><span class="sxs-lookup"><span data-stu-id="80484-142">Your administrator should not configure Exchange 2013 databases to use circular logging if you also plan to use VSS to enable your custom backup and restore operations.</span></span> <span data-ttu-id="80484-143">O log circular cria as seguintes restrições:</span><span class="sxs-lookup"><span data-stu-id="80484-143">Circular logging creates the following restrictions:</span></span> 
  
- <span data-ttu-id="80484-144">Se for habilitada durante a operação de backup ou a operação de recuperação, você não pode restaurar bancos de dados individuais.</span><span class="sxs-lookup"><span data-stu-id="80484-144">If enabled during the backup operation or the recovery operation, you cannot restore individual databases.</span></span>
    
- <span data-ttu-id="80484-145">Somente as operações de recuperação point-in-time são possíveis.</span><span class="sxs-lookup"><span data-stu-id="80484-145">Only point-in-time recovery operations are possible.</span></span> <span data-ttu-id="80484-146">Quando o log circular está habilitado, você pode excluir os logs de transações no mesmo diretório quando um banco de dados é restaurado, embora esses logs podem ser parte de um banco de dados diferente do Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="80484-146">When circular logging is enabled, you can delete transaction logs in the same directory when a database is restored, although those logs might be part of a different Exchange 2013 database.</span></span> 
    
- <span data-ttu-id="80484-147">Você não pode executar operações de backup incrementais ou diferenciais.</span><span class="sxs-lookup"><span data-stu-id="80484-147">You cannot perform incremental or differential backup operations.</span></span> <span data-ttu-id="80484-148">Para obter mais informações sobre esses tipos de backups, consulte [tipos de operações de backup para o Exchange 2013](types-of-backup-operations-for-exchange-2013.md).</span><span class="sxs-lookup"><span data-stu-id="80484-148">For more information about these types of backups, see [Types of backup operations for Exchange 2013](types-of-backup-operations-for-exchange-2013.md).</span></span>
    
<span data-ttu-id="80484-149">Se o log circular estiver ativa, o administrador deve desabilitar assim que possível para garantir que seus backups VSS não falharem.</span><span class="sxs-lookup"><span data-stu-id="80484-149">If circular logging is enables, your administrator should disable it as soon as possible to ensure that your VSS backups don't fail.</span></span> <span data-ttu-id="80484-150">Para obter mais informações, confira a postagem no blog [Backups de VSS e o registro em log Circular do Exchange](http://blogs.technet.com/b/exchange/archive/2010/08/18/3410672.aspx).</span><span class="sxs-lookup"><span data-stu-id="80484-150">For more information, check out the blog post [Exchange Circular Logging and VSS Backups](http://blogs.technet.com/b/exchange/archive/2010/08/18/3410672.aspx).</span></span> 
  
## <a name="exchange-database-mobility"></a><span data-ttu-id="80484-151">Mobilidade de banco de dados do Exchange</span><span class="sxs-lookup"><span data-stu-id="80484-151">Exchange database mobility</span></span>
<span data-ttu-id="80484-152"><a name="bk_exchangedatabasemobility"> </a></span><span class="sxs-lookup"><span data-stu-id="80484-152"></span></span>

<span data-ttu-id="80484-153">Exchange 2013 permite a mobilidade de banco de dados melhorar a disponibilidade e a confiabilidade de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="80484-153">Exchange 2013 allows for database mobility to improve mailbox reliability and availability.</span></span> <span data-ttu-id="80484-154">Mobilidade de banco de dados permite que você faça cópias do seu banco de dados de repositório do Exchange, desconecte o banco de dados do servidor e armazená-lo em outro servidor.</span><span class="sxs-lookup"><span data-stu-id="80484-154">Database mobility enables you to make copies of your Exchange store database, disconnect the database from the server, and store it on another server.</span></span> <span data-ttu-id="80484-155">Em um Exchange 2013 banco de dados de disponibilidade de grupo (DAG), várias cópias do banco de dados são armazenadas em computadores diferentes.</span><span class="sxs-lookup"><span data-stu-id="80484-155">In an Exchange 2013 Database Availability Group (DAG), multiple copies of the database are stored on different computers.</span></span> <span data-ttu-id="80484-156">Quando uma ou mais cópias do banco de dados são perdidas por hardware ou outra falha do sistema, informações das outras cópias podem ser usadas para propagar novamente o banco de dados por meio de operações de replicação normal.</span><span class="sxs-lookup"><span data-stu-id="80484-156">When one or more copies of the database are lost due to hardware or other system failure, information from the other copies can be used to reseed the database via normal replication operations.</span></span>
  
<span data-ttu-id="80484-157">Para operações de backup, se os bancos de dados do Exchange 2013 que estão incluídos no backup estão configurados em um DAG, o aplicativo de backup pode evitar mais interferência entre o instantâneo e o desempenho do servidor ativo de acordo com o instantâneo em um do inativa cópias de banco de dados.</span><span class="sxs-lookup"><span data-stu-id="80484-157">For backup operations, if the Exchange 2013 databases that are to be backed up are configured in a DAG, the backup application can better prevent interference between the snapshot and the active server's performance by taking the snapshot on one of the inactive database copies.</span></span> <span data-ttu-id="80484-158">Como as cópias de banco de dados estão sincronizadas na maioria das vezes, o aplicativo de backup pode tirar instantâneos de diferentes cópias do banco de dados e reconstrui-lo mais tarde das partes.</span><span class="sxs-lookup"><span data-stu-id="80484-158">Because the database copies are for the most part synchronized, the backup application can take snapshots from different copies of the database, and later reconstruct it from the pieces.</span></span>
  
<span data-ttu-id="80484-159">O único método suportado de restauração de bancos de dados do DAG dados de backup é restaurar todas as cópias do banco de dados, usando os mesmos dados de backup.</span><span class="sxs-lookup"><span data-stu-id="80484-159">The only supported method of restoring DAG databases from backup data is to restore all copies of the database by using the same backup data.</span></span> <span data-ttu-id="80484-160">Como os arquivos de log do banco de dados podem ser um pouco diferentes entre as cópias, restaurar cópias de banco de dados individuais usando dados diferentes pode causar o banco de dados para se tornar não montado.</span><span class="sxs-lookup"><span data-stu-id="80484-160">Because the database log files might be slightly different between the copies, restoring individual database copies using different data can cause the database to become unmountable.</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="80484-161">Nesta seção</span><span class="sxs-lookup"><span data-stu-id="80484-161">In this section</span></span>
<span data-ttu-id="80484-162"><a name="bk_inthissection"> </a></span><span class="sxs-lookup"><span data-stu-id="80484-162"></span></span>

- [<span data-ttu-id="80484-163">Logs de transações e arquivos de ponto de verificação de backup e restauração no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="80484-163">Transaction logs and checkpoint files for backup and restore in Exchange 2013</span></span>](transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange.md)
    
- [<span data-ttu-id="80484-164">Gravador do Exchange no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="80484-164">Exchange writer in Exchange 2013</span></span>](exchange-writer-in-exchange-2013.md)
    
## <a name="see-also"></a><span data-ttu-id="80484-165">Confira também</span><span class="sxs-lookup"><span data-stu-id="80484-165">See also</span></span>

- [<span data-ttu-id="80484-166">Exchange Online e o desenvolvimento do Exchange</span><span class="sxs-lookup"><span data-stu-id="80484-166">Exchange Online and Exchange development</span></span>](../exchange-server-development.md) 
- [<span data-ttu-id="80484-167">Tipos de operações de backup para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="80484-167">Types of backup operations for Exchange 2013</span></span>](types-of-backup-operations-for-exchange-2013.md)
- [<span data-ttu-id="80484-168">Restaurando bancos de dados do Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="80484-168">Restoring Exchange 2013 databases</span></span>](restoring-exchange-2013-databases.md)
    
