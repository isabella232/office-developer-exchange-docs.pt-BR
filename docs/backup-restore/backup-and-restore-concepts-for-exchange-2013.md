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
# <a name="backup-and-restore-concepts-for-exchange-2013"></a>Conceitos de backup e restauração do Exchange 2013

Encontre informações sobre bancos de dados do Exchange que ajudarão você a criar o backup e restaurar aplicativos para o Exchange 2013.
  
Antes de criar um backup e restaurar aplicativos para o Exchange Server 2013, você deve estar familiarizado com a estrutura de arquivos de banco de dados do Exchange. Usando os arquivos de banco de dados de repositório do Exchange, você pode fazer backup dos dados no seu armazenamento e restaurá-lo mais tarde conforme necessário. Se você está limitado a espaço em disco, o administrador pode implementar o log circular e isso afetará sua capacidade de fazer backup do banco de dados. Você também pode tirar proveito do recurso de mobilidade de banco de dados no Exchange 2013 para fazer backup e restaurar dados do Exchange. Mobilidade de banco de dados, em combinação com o seu aplicativo de backup e restauração, é uma boa medida de redundância para recuperação de desastres.

<a name="bk_exchangedatabases"> </a>

## <a name="exchange-store-database-files"></a>Arquivos de banco de dados de repositório do Exchange

Exchange 2013 inclui o suporte para até 100 bancos de dados. Cada banco de dados do Exchange 2013 contém os arquivos listados na tabela a seguir. 
  
**Tabela 1. Arquivos de banco de dados do Exchange 2013**

|Tipo de arquivo|Extensão|Descrição|
|:-----|:-----|:-----|
|Arquivo de banco de dados  <br/> |\*. edb  <br/> |Registra todas as alterações que foram confirmadas no banco de dados na memória.  <br/> |
|Fluxo de log de transação  <br/> |\*. log  <br/> |Operações de registros, como a criação ou modificação de uma mensagem, que serão confirmada no banco de dados. Limite de tamanho para 1 MB.  <br/> |
|Arquivo de verificação  <br/> |\*. chk  <br/> |Registros que conectado transações tem sido escritos para os arquivos de banco de dados no disco.  <br/> |
   
Exchange 2013 mantém um único conjunto de arquivos de log de transações para cada banco de dados. Os logs de transações são importantes para operações de backup e recuperação. Quando você cria um backup e restaurar o aplicativo que usa o serviço de cópia de sombra de Volume (VSS), certifique-se de que você manipule esses logs corretamente. Para obter mais informações, consulte os [logs de transações e arquivos de ponto de verificação de backup e restauração no Exchange 2013](transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange.md). Para fazer backup de um banco de dados e seu fluxo de log, você deve fazer backup de todo o volume que contém o banco de dados e logs. Truncamento de log ocorrerá apenas após a conclusão bem-sucedida de um backup completo de um volume ou pastas que contêm um banco de dados do Exchange.
  
Em cada servidor do Exchange, você pode montá apenas um banco de dados de recuperação por vez. Você pode acessar o banco de dados de recuperação usando cmdlets do Shell de gerenciamento do Exchange como **New-MailboxRestoreRequest**. Para obter mais informações sobre bancos de dados do Exchange recuperação, consulte [Recovery Databases](http://technet.microsoft.com/en-us/library/dd876954%28v=exchg.150%29.aspx) no TechNet. Para obter mais informações sobre os cmdlets do Shell de gerenciamento do Exchange, consulte [Os Cmdlets do Exchange 2013](http://technet.microsoft.com/en-us/library/bb124413.aspx) no TechNet. 
  
## <a name="circular-logging"></a>Log circular
<a name="bk_circularlogging"> </a>

Se a capacidade de armazenamento é um problema, o administrador pode habilitar log circular. Quando o log circular estiver habilitado, o Exchange grava os logs de transação como de costume, mas quando um arquivo de ponto de verificação é avançado, a parte inativa do log de transação será truncada. O administrador não deve configurar os bancos de dados do Exchange 2013 para usar o log circular, se você planeja usar o VSS para habilitar o seu backup personalizado e operações de restauração. O log circular cria as seguintes restrições: 
  
- Se for habilitada durante a operação de backup ou a operação de recuperação, você não pode restaurar bancos de dados individuais.
    
- Somente as operações de recuperação point-in-time são possíveis. Quando o log circular está habilitado, você pode excluir os logs de transações no mesmo diretório quando um banco de dados é restaurado, embora esses logs podem ser parte de um banco de dados diferente do Exchange 2013. 
    
- Você não pode executar operações de backup incrementais ou diferenciais. Para obter mais informações sobre esses tipos de backups, consulte [tipos de operações de backup para o Exchange 2013](types-of-backup-operations-for-exchange-2013.md).
    
Se o log circular estiver ativa, o administrador deve desabilitar assim que possível para garantir que seus backups VSS não falharem. Para obter mais informações, confira a postagem no blog [Backups de VSS e o registro em log Circular do Exchange](http://blogs.technet.com/b/exchange/archive/2010/08/18/3410672.aspx). 
  
## <a name="exchange-database-mobility"></a>Mobilidade de banco de dados do Exchange
<a name="bk_exchangedatabasemobility"> </a>

Exchange 2013 permite a mobilidade de banco de dados melhorar a disponibilidade e a confiabilidade de caixa de correio. Mobilidade de banco de dados permite que você faça cópias do seu banco de dados de repositório do Exchange, desconecte o banco de dados do servidor e armazená-lo em outro servidor. Em um Exchange 2013 banco de dados de disponibilidade de grupo (DAG), várias cópias do banco de dados são armazenadas em computadores diferentes. Quando uma ou mais cópias do banco de dados são perdidas por hardware ou outra falha do sistema, informações das outras cópias podem ser usadas para propagar novamente o banco de dados por meio de operações de replicação normal.
  
Para operações de backup, se os bancos de dados do Exchange 2013 que estão incluídos no backup estão configurados em um DAG, o aplicativo de backup pode evitar mais interferência entre o instantâneo e o desempenho do servidor ativo de acordo com o instantâneo em um do inativa cópias de banco de dados. Como as cópias de banco de dados estão sincronizadas na maioria das vezes, o aplicativo de backup pode tirar instantâneos de diferentes cópias do banco de dados e reconstrui-lo mais tarde das partes.
  
O único método suportado de restauração de bancos de dados do DAG dados de backup é restaurar todas as cópias do banco de dados, usando os mesmos dados de backup. Como os arquivos de log do banco de dados podem ser um pouco diferentes entre as cópias, restaurar cópias de banco de dados individuais usando dados diferentes pode causar o banco de dados para se tornar não montado.
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_inthissection"> </a>

- [Logs de transações e arquivos de ponto de verificação de backup e restauração no Exchange 2013](transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange.md)
    
- [Gravador do Exchange no Exchange 2013](exchange-writer-in-exchange-2013.md)
    
## <a name="see-also"></a>Confira também

- [Exchange Online e o desenvolvimento do Exchange](../exchange-server-development.md) 
- [Tipos de operações de backup para o Exchange 2013](types-of-backup-operations-for-exchange-2013.md)
- [Restaurando bancos de dados do Exchange 2013](restoring-exchange-2013-databases.md)
    

