---
title: SortOrder (ConversationNodeSortOrder)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f9c4295c-8089-4533-b92f-2051eae9afeb
description: O elemento SortOrder especifica a ordem de classificação usada para o resultado de uma solicitação GetConversationItems.
ms.openlocfilehash: 0091968f1359b0cf744525139b5c6a8cf1687d81
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544672"
---
# <a name="sortorder-conversationnodesortorder"></a>SortOrder (ConversationNodeSortOrder)

O **elemento SortOrder** especifica a ordem de classificação usada para o resultado de uma **solicitação GetConversationItems.** 
  
```XML
<SortOrder>TreeOrderAscending | TreeOrderDescending | DateOrderAscending | DateOrderDescending</SortOrder>
```

 **ConversationNodeSortOrder**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[GetConversationItems](getconversationitems.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do **elemento SortOrder** é a ordem na qual as conversas foram ordenadas. Um valor de texto **de TreeOrderAscending** indica que as conversas são ordenadas de acordo com a árvore de conversa em ordem crescente. Um valor de texto **de TreeOrderDescending** indica que as conversas são ordenadas de acordo com a árvore de conversa em ordem decrescente. Um valor de texto **de DateOrderAscending** indica que as conversas são ordenadas de acordo com a data da conversa em ordem crescente. Um valor de texto **de DateOrderDescending** indica que as conversas são ordenadas de acordo com a data da conversa em ordem decrescente. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

