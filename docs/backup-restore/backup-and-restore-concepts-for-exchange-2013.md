---
title: Conceitos de backup e restauração para Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 9a1c4709-9313-4ccf-9f8a-673a51d51f23
description: Encontre informações sobre Exchange que ajudarão você a criar seus aplicativos de backup e restauração para Exchange 2013.
ms.openlocfilehash: c0b2e0269c3668779f980bf6984d84aff76573f1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510516"
---
# <a name="backup-and-restore-concepts-for-exchange-2013"></a>Conceitos de backup e restauração para Exchange 2013

Encontre informações sobre Exchange que ajudarão você a criar seus aplicativos de backup e restauração para Exchange 2013.
  
Antes de criar aplicativos de backup e restauração para Exchange Server 2013, você deve estar familiarizado com a estrutura de arquivos Exchange banco de dados. Usando os arquivos Exchange de banco de dados, você pode fazer backup dos dados em seu armazenamento e restaurá-los posteriormente, conforme necessário. Se você estiver limitado ao espaço em disco, o administrador poderá implementar o log circular e isso afetará sua capacidade de fazer backup do banco de dados. Você também pode aproveitar o recurso de mobilidade de banco de dados no Exchange 2013 para fazer backup e restaurar Exchange dados. A mobilidade do banco de dados, em combinação com seu aplicativo de backup e restauração, é uma boa medida de redundância para recuperação de desastres.

<a name="bk_exchangedatabases"> </a>

## <a name="exchange-store-database-files"></a>Exchange armazenar arquivos de banco de dados

Exchange 2013 inclui suporte para até 100 bancos de dados. Cada Exchange 2013 contém os arquivos listados na tabela a seguir. 
  
**Tabela 1. Exchange de banco de dados 2013**

|Tipo de arquivo|Extensão|Descrição|
|:-----|:-----|:-----|
|Arquivo de banco de dados  <br/> |\*.edb  <br/> |Registra todas as alterações que foram comprometidas no banco de dados na memória.  <br/> |
|Fluxo de log de transações  <br/> |\*.log  <br/> |Registra operações, como a criação ou modificação de uma mensagem, que serão comprometidas com o banco de dados. Tamanho limitado a 1 MB cada.  <br/> |
|Arquivo de ponto de verificação  <br/> |\*.chk  <br/> |Registros que registraram transações foram gravados nos arquivos de banco de dados em disco.  <br/> |
   
Exchange 2013 mantém um único conjunto de arquivos de log de transações para cada banco de dados. Os logs de transação são importantes para operações de backup e recuperação. Ao criar um aplicativo de backup e restauração que usa o Serviço de Cópia de Sombra de Volume (VSS), você deve garantir que você lida com esses logs corretamente. Para obter mais informações, consulte Logs de transação e arquivos de ponto de verificação para backup e restauração [Exchange 2013](transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange.md). Para fazer o back up de um banco de dados e seu fluxo de log, você deve fazer o back up de todo o volume que contém o banco de dados e os logs. A truncamento de log ocorrerá somente após a conclusão bem-sucedida de um backup completo de um volume ou pastas que contenham um banco de dados Exchange dados.
  
Em cada Exchange servidor, você pode montar apenas um banco de dados de recuperação por vez. Você pode acessar o banco de dados de recuperação usando Exchange cmdlets do Shell de Gerenciamento, como **New-MailboxRestoreRequest**. Para obter mais informações sobre Exchange de recuperação, consulte [Recovery Databases](https://technet.microsoft.com/library/dd876954%28v=exchg.150%29.aspx) on TechNet. Para obter mais informações sobre Exchange cmdlets do Shell de Gerenciamento, [consulte Exchange Cmdlets 2013](https://technet.microsoft.com/library/bb124413.aspx) no TechNet. 
  
## <a name="circular-logging"></a>Log circular
<a name="bk_circularlogging"> </a>

Se a capacidade de armazenamento for um problema, o administrador poderá habilitar o log circular. Quando o log circular está habilitado, Exchange grava logs de transação como de costume, mas quando um arquivo de ponto de verificação é avançado, a parte inativa do log de transações é truncada. O administrador não deve configurar Exchange bancos de dados 2013 para usar o log circular se você também planeja usar o VSS para habilitar suas operações personalizadas de backup e restauração. O log circular cria as seguintes restrições: 
  
- Se estiver habilitado durante a operação de backup ou a operação de recuperação, não será possível restaurar bancos de dados individuais.
    
- Somente operações de recuperação point-in-time são possíveis. Quando o log circular estiver habilitado, você poderá excluir logs de transação no mesmo diretório quando um banco de dados for restaurado, embora esses logs possam fazer parte de um banco de dados Exchange 2013 diferente. 
    
- Não é possível executar operações de backup incrementais ou diferenciais. Para obter mais informações sobre esses tipos de backups, consulte [Tipos de operações de backup para Exchange 2013](types-of-backup-operations-for-exchange-2013.md).
    
Se o log circular estiver habilitado, o administrador deverá desabilitá-lo assim que possível para garantir que os backups vss não falhem. Para obter mais informações, confira a postagem do blog Exchange [Log Circular e Backups VSS.](https://blogs.technet.com/b/exchange/archive/2010/08/18/3410672.aspx) 
  
## <a name="exchange-database-mobility"></a>Exchange de banco de dados
<a name="bk_exchangedatabasemobility"> </a>

Exchange 2013 permite que a mobilidade do banco de dados melhore a confiabilidade e a disponibilidade da caixa de correio. A mobilidade do banco de dados permite que você faça cópias do banco de dados de armazenamento Exchange, desconecte o banco de dados do servidor e armazene-o em outro servidor. Em um Exchange grupo de disponibilidade de banco de dados (DAG) 2013, várias cópias do banco de dados são armazenadas em computadores diferentes. Quando uma ou mais cópias do banco de dados são perdidas devido a uma falha de hardware ou outra do sistema, as informações das outras cópias podem ser usadas para reassepar o banco de dados por meio de operações de replicação normais.
  
Para operações de backup, se os bancos de dados do Exchange 2013 que devem ser backups estão configurados em um DAG, o aplicativo de backup pode evitar melhor a interferência entre o instantâneo e o desempenho do servidor ativo, capturando o instantâneo em uma das cópias de banco de dados inativas. Como as cópias do banco de dados são para a maior parte sincronizadas, o aplicativo de backup pode tirar instantâneos de diferentes cópias do banco de dados e reconstruí-lo posteriormente das partes.
  
O único método suportado para restaurar bancos de dados do DAG a partir de dados de backup é restaurar todas as cópias do banco de dados usando os mesmos dados de backup. Como os arquivos de log do banco de dados podem ser ligeiramente diferentes entre as cópias, restaurar cópias de banco de dados individuais usando dados diferentes pode fazer com que o banco de dados se torne inconsponível.
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_inthissection"> </a>

- [Logs de transações e arquivos de ponto de verificação para backup e restauração no Exchange 2013](transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange.md)
    
- [Exchange escritor no Exchange 2013](exchange-writer-in-exchange-2013.md)
    
## <a name="see-also"></a>Confira também

- [Desenvolvimento do Exchange Online e do Exchange](../exchange-server-development.md) 
- [Tipos de operações de backup para Exchange 2013](types-of-backup-operations-for-exchange-2013.md)
- [Restaurando Exchange bancos de dados 2013](restoring-exchange-2013-databases.md)
    

