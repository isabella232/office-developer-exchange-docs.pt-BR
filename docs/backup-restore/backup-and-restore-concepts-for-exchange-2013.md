---
title: Conceitos de backup e restauração para o Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9a1c4709-9313-4ccf-9f8a-673a51d51f23
description: Encontre informações sobre os bancos de dados do Exchange que irão ajudá-lo a criar seus aplicativos de backup e restauração para o Exchange 2013.
ms.openlocfilehash: fd35699839af105dd3fe285776b071c1d03d58dd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44437981"
---
# <a name="backup-and-restore-concepts-for-exchange-2013"></a>Conceitos de backup e restauração para o Exchange 2013

Encontre informações sobre os bancos de dados do Exchange que irão ajudá-lo a criar seus aplicativos de backup e restauração para o Exchange 2013.
  
Antes de criar aplicativos de backup e restauração para o Exchange Server 2013, você deve estar familiarizado com a estrutura de arquivos do banco de dados do Exchange. Usando os arquivos de banco de dados do repositório do Exchange, você pode fazer o backup dos dados em sua loja e restaurá-los mais tarde, conforme necessário. Se você estiver limitado no espaço em disco, o administrador poderá implementar o registro em log circular, e isso afetará a capacidade de fazer backup do banco de dados. Você também pode aproveitar o recurso de mobilidade de banco de dados no Exchange 2013 para fazer o backup e restaurar dados do Exchange. Mobilidade de banco de dados, em combinação com seu aplicativo de backup e restauração, é uma boa medida de redundância para recuperação de desastres.

<a name="bk_exchangedatabases"> </a>

## <a name="exchange-store-database-files"></a>Arquivos de banco de dados do repositório do Exchange

O Exchange 2013 inclui suporte para até 100 bancos de dados. Cada banco de dados do Exchange 2013 contém os arquivos listados na tabela a seguir. 
  
**Tabela 1. Arquivos de banco de dados do Exchange 2013**

|Tipo de arquivo|Extensão|Descrição|
|:-----|:-----|:-----|
|Arquivo de banco de dados  <br/> |\*. edb  <br/> |Registra todas as alterações que foram confirmadas no banco de dados de memória.  <br/> |
|Fluxo do log de transações  <br/> |\*. log  <br/> |Operações de registros, como a criação ou a modificação de uma mensagem, que serão confirmadas no banco de dados. Limitado em tamanho de 1 MB cada.  <br/> |
|Arquivo de ponto de verificação  <br/> |\*. chk  <br/> |Registros que transações registradas foram gravadas nos arquivos de banco de dados de disco.  <br/> |
   
O Exchange 2013 mantém um único conjunto de arquivos de log de transações para cada banco de dados. Os logs de transação são importantes para operações de backup e recuperação. Ao criar um aplicativo de backup e restauração que usa o serviço de cópias de sombra de volume (VSS), você deve lidar com esses logs corretamente. Para obter mais informações, consulte [logs de transações e arquivos de ponto de verificação para backup e restauração no Exchange 2013](transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange.md). Para fazer o backup de um banco de dados e seu fluxo de logs, você deve fazer backup de todo o volume que contém o banco de dados e os logs. O truncamento de log ocorrerá somente após uma conclusão bem-sucedida de um backup completo de um volume ou de pastas que contenham um banco de dados do Exchange.
  
Em cada servidor Exchange, você pode montar apenas um banco de dados de recuperação por vez. Você pode acessar o banco de dados de recuperação usando cmdlets do Shell de gerenciamento do Exchange, como **New-MailboxRestoreRequest**. Para obter mais informações sobre os bancos de dados de recuperação do Exchange, consulte [bancos de dados de recuperação](https://technet.microsoft.com/library/dd876954%28v=exchg.150%29.aspx) no TechNet. Para obter mais informações sobre os cmdlets do Shell de gerenciamento do Exchange, consulte [cmdlets do exchange 2013](https://technet.microsoft.com/library/bb124413.aspx) no TechNet. 
  
## <a name="circular-logging"></a>Log circular
<a name="bk_circularlogging"> </a>

Se a capacidade de armazenamento for um problema, o administrador poderá habilitar o log circular. Quando o registro em log circular está habilitado, o Exchange grava logs de transações como de costume, mas quando um arquivo de ponto de verificação é avançado, a parte inativa do log de transações é truncada. O administrador não deve configurar os bancos de dados do Exchange 2013 para usar o registro em log circular se você também planeja usar o VSS para habilitar suas operações personalizadas de backup e restauração. O log circular cria as seguintes restrições: 
  
- Se habilitada durante a operação de backup ou recuperação, não será possível restaurar bancos de dados individuais.
    
- Só é possível realizar operações de recuperação point-in-time. Quando o registro em log circular está habilitado, você pode excluir logs de transações no mesmo diretório quando um banco de dados é restaurado, embora esses logs possam fazer parte de um banco de dados diferente do Exchange 2013. 
    
- Não é possível realizar operações de backup incrementais ou diferenciais. Para obter mais informações sobre esses tipos de backups, consulte [tipos de operações de backup para o Exchange 2013](types-of-backup-operations-for-exchange-2013.md).
    
Se o registro em log circular estiver habilitada, o administrador deverá desabilitá-lo assim que possível para garantir que seus backups VSS não falhem. Para obter mais informações, confira o registro em log circular de postagens de blog [e backups VSS](https://blogs.technet.com/b/exchange/archive/2010/08/18/3410672.aspx). 
  
## <a name="exchange-database-mobility"></a>Mobilidade de banco de dados do Exchange
<a name="bk_exchangedatabasemobility"> </a>

O Exchange 2013 permite que a mobilidade de banco de dados aprimore a confiabilidade e a disponibilidade da caixa de correio A mobilidade de banco de dados permite fazer cópias do banco de dados do repositório do Exchange, desconectar o banco de dados do servidor e armazená-lo em outro servidor. Em um grupo de disponibilidade de banco de dados (DAG) do Exchange 2013, várias cópias do banco de dados são armazenadas em computadores diferentes. Quando uma ou mais cópias do banco de dados são perdidas devido a uma falha de hardware ou de outro sistema, as informações das outras cópias podem ser usadas para propagar novamente o banco de dados por meio de operações de replicação normais.
  
Para operações de backup, se os bancos de dados do Exchange 2013 que devem ser incluídos no backup estiverem configurados em um DAG, o aplicativo de backup pode impedir melhor interferência entre o instantâneo e o desempenho do servidor ativo ao pegar o instantâneo em uma das cópias de banco de dados inativas. Como as cópias de banco de dados são para a maior parte sincronizada, o aplicativo de backup pode obter instantâneos de diferentes cópias do banco de dados e reconstruí-lo mais tarde das partes.
  
O único método com suporte de restauração de bancos de dados do DAG dos dados de backup é restaurar todas as cópias do banco de dados usando os mesmos dados de backup. Como os arquivos de log do banco de dados podem ser um pouco diferentes entre as cópias, a restauração de cópias de banco de dados individuais usando dados diferentes pode fazer com que o banco de dados se torne não montável.
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_inthissection"> </a>

- [Logs de transação e arquivos de ponto de verificação para backup e restauração no Exchange 2013](transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange.md)
    
- [Gravador do Exchange no Exchange 2013](exchange-writer-in-exchange-2013.md)
    
## <a name="see-also"></a>Também consulte

- [Desenvolvimento do Exchange Online e do Exchange](../exchange-server-development.md) 
- [Tipos de operações de backup para o Exchange 2013](types-of-backup-operations-for-exchange-2013.md)
- [Restauração de bancos de dados do Exchange 2013](restoring-exchange-2013-databases.md)
    

