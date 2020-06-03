---
title: Logs de transação e arquivos de ponto de verificação para backup e restauração no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 80e04b9f-87c7-4acf-89b1-aa66ffaf7e53
description: Encontre informações sobre logs de transações e arquivos de ponto de verificação e como eles são usados para fazer backup e restauração de dados do Exchange 2013.
ms.openlocfilehash: 5b01fc6924f82e76943795df877ae84b1fde087b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456385"
---
# <a name="transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange"></a>Logs de transação e arquivos de ponto de verificação para backup e restauração no Exchange

Encontre informações sobre logs de transações e arquivos de ponto de verificação e como eles são usados para fazer backup e restauração de dados do Exchange 2013.
  
**Aplica-se a:** Exchange Server 2013 
  
Este artigo descreve como o Exchange Server 2013 usa logs de transação e arquivos de ponto de verificação para ajudar a evitar a perda de dados. É importante estar ciente dessas informações ao desenvolver aplicativos de backup e restauração que usam o serviço de cópias de sombra de volume (VSS) em versões do Windows Server a partir do Windows Server 2008.
  
## <a name="transaction-logs-in-exchange-2013"></a>Logs de transação no Exchange 2013

O Exchange 2013 mantém um único conjunto de arquivos de log de transações para cada banco de dados. Uma transação é definida como qualquer operação que altere o estado ou o conteúdo do banco de dados. Os arquivos de log de transações de um banco de dados individual registram todas as transações realizadas no banco de dados. Os registros das transações são gravados nos logs de transações antes que sejam feitos no próprio banco de dados, para garantir que todas as transações confirmadas possam ser recuperadas no caso de uma falha no banco de dados. Os logs de transação do banco de dados do Exchange 2013 são armazenados no disco antes de as transações serem confirmadas no arquivo de banco de dados. 
  
A gravação das transações antes da atualização do banco de dados é chamada de registro de write-ahead. Para ajudar a garantir que o banco de dados seja colocado corretamente de volta para o estado apropriado, o Exchange 2013 grava dados nos arquivos de banco de dados usando gravações e pontos de verificação baseados em páginas. Durante as operações regulares, o repositório do Exchange primeiro registra as alterações no banco de dados nos logs de transações e, em seguida, faz essas alterações em uma cópia na memória do banco de dados. Os logs de transação registram o início e o fim de cada transação. Isso garante que as informações suficientes estejam disponíveis para desfazer ou reverter operações posteriormente no banco de dados.
  
Ao se recuperar de erros nos quais o arquivo de banco de dados no disco está danificado, mas os logs de transações estão intactos, o aplicativo de restauração deve primeiro restaurar uma cópia válida conhecida do arquivo de banco de dados.
  
O repositório do Exchange repete as transações dos logs de transação incluídos no backup e, em seguida, repete as transações restantes dos arquivos de log de transações em disco. Observe que às vezes, as transações podem ser perdidas se o sistema falhar quando as transações são registradas nos logs de transação e quando são realmente gravadas nos arquivos do banco de dados. 
  
Periodicamente, o repositório do Exchange verifica a imagem de banco de dados na memória e, em seguida, determina quais páginas foram alteradas. O repositório do Exchange combina as alterações pendentes e, em seguida, grava essas páginas no arquivo de banco de dados no disco.
  
## <a name="checkpoint-files-in-exchange-2013"></a>Arquivos de ponto de verificação no Exchange 2013

Um arquivo de ponto de verificação registra quais transações registradas foram gravadas nos arquivos de banco de dados de disco. O ponto de verificação é avançado quando todas as páginas do banco de dados que foram modificadas por entradas nos logs de transação são gravadas com êxito no disco. Como o arquivo de ponto de verificação registra quais transações já estão na imagem de banco de dados no disco, o repositório do Exchange só precisa repetir as transações que ocorreram após o ponto de verificação. Dependendo do período de tempo entre backups, isso pode diminuir significativamente o número de transações que devem ser repetidas no banco de dados se ocorrer uma falha do sistema.
  
## <a name="see-also"></a>Confira também

- [Conceitos de backup e restauração para o Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
- [Tipos de operações de backup para o Exchange 2013](types-of-backup-operations-for-exchange-2013.md)
- [Restauração de bancos de dados do Exchange 2013](restoring-exchange-2013-databases.md)
    

