---
title: Logs de transações e arquivos de ponto de verificação de backup e restauração no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 80e04b9f-87c7-4acf-89b1-aa66ffaf7e53
description: Encontre informações sobre logs de transações e arquivos de ponto de verificação e como elas são usadas para fazer backup e restaurar dados do Exchange 2013.
ms.openlocfilehash: 53f128348bb2e8895bc1eefaf62402fa348c81ea
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750656"
---
# <a name="transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange"></a>Logs de transações e arquivos de ponto de verificação de backup e restauração no Exchange

Encontre informações sobre logs de transações e arquivos de ponto de verificação e como elas são usadas para fazer backup e restaurar dados do Exchange 2013.
  
**Aplica-se a:** Exchange Server 2013 
  
Este artigo descreve como o Exchange Server 2013 usa logs de transações e arquivos de ponto de verificação para ajudar a evitar perda de dados. É importante estar ciente dessas informações quando você desenvolver o backup e restaurar aplicativos que usam o serviço de cópia de sombra de Volume (VSS) nas versões do Windows Server, começando com o Windows Server 2008.
  
## <a name="transaction-logs-in-exchange-2013"></a>Os logs de transações no Exchange 2013

Exchange 2013 mantém um único conjunto de arquivos de log de transações para cada banco de dados. Uma transação é definida como qualquer operação que altera o estado ou conteúdo do banco de dados. Os arquivos de log de transação para um registro de banco de dados individual, todas as transações realizadas no banco de dados. Registros das transações serão gravados os logs de transação antes que eles sejam feitos no banco de dados em si, para garantir que todas as transações confirmadas possam ser recuperadas em caso de uma falha de banco de dados. Logs de transações de banco de dados do Exchange 2013 são armazenados no disco antes que as transações sejam confirmadas no arquivo de banco de dados. 
  
A gravação das transações antes que o banco de dados é atualizado é chamada de gravação antecipada log. Para ajudar a garantir que o banco de dados corretamente é trazido de volta para o estado apropriado, Exchange 2013 grava os dados nos arquivos do banco de dados usando os pontos de verificação e gravações baseado em página. Durante as operações normais, o armazenamento do Exchange primeiro registra as alterações do banco de dados nos logs de transação e, em seguida, torna essas alterações em uma cópia na memória do banco de dados. Os logs de transação registram início e no final de cada transação. Isso garante que informações suficientes estão disponíveis para desfazer mais tarde ou reverter operações no banco de dados.
  
Ao recuperar de erros no qual o arquivo de banco de dados em disco estiver danificado, mas os logs de transação estão intactos, seu aplicativo de restauração primeiramente deve restaurar uma cópia de uma boa conhecida do arquivo de banco de dados.
  
O armazenamento do Exchange repete as transações da transação de um backup anterior faz e depois repete todas as transações de restantes dos arquivos de log de transação no disco. Observe que em alguns casos, as transações podem ser perdidas se o sistema falhar entre quando as transações são registradas nos logs de transação e quando eles são gravados na verdade, os arquivos de banco de dados. 
  
Periodicamente, o armazenamento do Exchange verifica a imagem do banco de dados na memória e, em seguida, determina quais páginas foram alteradas. O armazenamento do Exchange combina as alterações pendentes e depois grava essas páginas para o arquivo de banco de dados no disco.
  
## <a name="checkpoint-files-in-exchange-2013"></a>Arquivos de ponto de verificação no Exchange 2013

Registros de arquivo um ponto de verificação que conectado transações tem sido escrito para os arquivos de banco de dados no disco. O ponto de verificação é avançado quando todas as páginas do banco de dados que foram modificadas por entradas nos logs de transação com êxito são gravadas no disco. Porque o arquivo de verificação de registros que transações já estão na imagem do banco de dados no disco, o armazenamento do Exchange só precisa transações que tenham ocorrido após o ponto de verificação de repetição. Dependendo do período de tempo entre backups, isso pode diminuir bastante o número de transações que devem ser repetidos no banco de dados se ocorrer uma falha do sistema.
  
## <a name="see-also"></a>Confira também

- [Conceitos de backup e restauração do Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
- [Tipos de operações de backup para o Exchange 2013](types-of-backup-operations-for-exchange-2013.md)
- [Restaurando bancos de dados do Exchange 2013](restoring-exchange-2013-databases.md)
    

