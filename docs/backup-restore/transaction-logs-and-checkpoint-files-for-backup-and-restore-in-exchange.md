---
title: Logs de transações e arquivos de ponto de verificação para backup e restauração Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 80e04b9f-87c7-4acf-89b1-aa66ffaf7e53
description: Encontre informações sobre logs de transação e arquivos de ponto de verificação e como eles são usados para fazer backup e restaurar Exchange dados de 2013.
ms.openlocfilehash: ae47c7757a1001f28c467ea58ec87b4ddbc5a5c4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513259"
---
# <a name="transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange"></a>Logs de transações e arquivos de ponto de verificação para backup e restauração Exchange

Encontre informações sobre logs de transação e arquivos de ponto de verificação e como eles são usados para fazer backup e restaurar Exchange dados de 2013.
  
**Aplica-se a:** Exchange Server 2013 
  
Este artigo descreve como o Exchange Server 2013 usa logs de transação e arquivos de ponto de verificação para ajudar a evitar a perda de dados. É importante estar ciente dessas informações ao desenvolver aplicativos de backup e restauração que usam o VsS (Serviço de Cópia de Sombra de Volume) em versões do Windows Server a partir do Windows Server 2008.
  
## <a name="transaction-logs-in-exchange-2013"></a>Logs de transação no Exchange 2013

Exchange 2013 mantém um único conjunto de arquivos de log de transações para cada banco de dados. Uma transação é definida como qualquer operação que altera o estado ou o conteúdo do banco de dados. Os arquivos de log de transação para um banco de dados individual registram todas as transações realizadas no banco de dados. Os registros das transações são gravados nos logs de transação antes de serem feitos no próprio banco de dados, para garantir que todas as transações comprometidas possam ser recuperadas em caso de falha no banco de dados. Exchange logs de transações de banco de dados 2013 são armazenados em disco antes que as transações sejam comprometidas com o arquivo de banco de dados. 
  
A gravação das transações antes da atualização do banco de dados é chamada de log de gravação antecipada. Para ajudar a garantir que o banco de dados seja corretamente trazido de volta ao estado adequado, o Exchange 2013 grava dados nos arquivos de banco de dados usando gravações e pontos de verificação baseados em página. Durante operações regulares, o Exchange primeiro registra alterações no banco de dados nos logs de transação e, em seguida, faz essas alterações em uma cópia na memória do banco de dados. Os logs de transação registram o início e o final de cada transação. Isso garante que informações suficientes estão disponíveis para desfazer ou reverter operações posteriores no banco de dados.
  
Ao recuperar de erros nos quais o arquivo de banco de dados no disco está danificado, mas os logs de transação estão intactos, seu aplicativo de restauração deve primeiro restaurar uma boa cópia conhecida do arquivo de banco de dados.
  
O Exchange armazena as transações dos logs de transação anteriormente armazenados e, em seguida, replay quaisquer transações restantes dos arquivos de log de transações no disco. Observe que, às vezes, as transações podem ser perdidas se o sistema falhar entre quando as transações são registradas nos logs de transação e quando elas são gravadas nos arquivos de banco de dados. 
  
Periodicamente, o Exchange verifica a imagem do banco de dados na memória e determina quais páginas foram alteradas. O Exchange store combina as alterações pendentes e grava essas páginas no arquivo de banco de dados no disco.
  
## <a name="checkpoint-files-in-exchange-2013"></a>Arquivos de ponto de verificação Exchange 2013

Um arquivo de ponto de verificação registra que as transações registradas foram registradas nos arquivos de banco de dados em disco. O ponto de verificação é avançado quando todas as páginas de banco de dados que foram modificadas por entradas nos logs de transação são gravados com êxito no disco. Como o arquivo de ponto de verificação registra quais transações já estão na imagem do banco de dados em disco, o Exchange armazenamento só precisa repetir as transações que ocorreram após o ponto de verificação. Dependendo do período de tempo entre backups, isso pode diminuir bastante o número de transações que devem ser replayadas no banco de dados se ocorrer uma falha no sistema.
  
## <a name="see-also"></a>Confira também

- [Conceitos de backup e restauração para Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
- [Tipos de operações de backup para Exchange 2013](types-of-backup-operations-for-exchange-2013.md)
- [Restaurando Exchange bancos de dados 2013](restoring-exchange-2013-databases.md)
    

