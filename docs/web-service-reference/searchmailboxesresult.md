---
title: SearchMailboxesResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: ddb276c4-6c8a-46ef-a2eb-46b6a0bfce09
description: O elemento SearchMailboxesResult contém o resultado da solicitação SearchMailboxes.
ms.openlocfilehash: dee1e12a6d083ca3f8d3ddb509775b454e3e8fc0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59534402"
---
# <a name="searchmailboxesresult"></a>SearchMailboxesResult

O **elemento SearchMailboxesResult** contém o resultado da **solicitação SearchMailboxes.** 
  
```XML
<SearchMailboxesResult>
   <SearchQueries/>
   <ResultType/>
   <ItemCount/>
   <Size/>
   <PageItemCount/>
   <PageItemSize/>
   <KeywordStats/>
   <Items/>
   <FailedMailboxes/>
   <Refiners/>
   <MailboxStats/>
</SearchMailboxesResult>
```

 **SearchMailboxesResultType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

[SearchQueries](searchqueries.md)  |  [ResultType](resulttype.md)  |  [ItemCount](itemcount.md)  |  [Tamanho (longo)](size-long.md)  |  [PageItemCount](pageitemcount.md)  |  [PageItemSize](pageitemsize.md)  |  [KeywordStats](keywordstats.md)  |  [Items (ArrayOfSearchPreviewItemsType)](items-arrayofsearchpreviewitemstype.md)  |  [FailedMailboxes](failedmailboxes.md)  |  [Refinadores](refiners.md)  |  [MailboxStats](mailboxstats.md)
  
### <a name="parent-elements"></a>Elementos pai

[SearchMailboxesResponseMessage](searchmailboxesresponsemessage.md)
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |falso  <br/> |
   

