---
title: SortOrder (ConversationNodeSortOrder)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9c4295c-8089-4533-b92f-2051eae9afeb
description: O elemento SortOrder especifica a ordem de classificação usada para o resultado de uma solicitação GetConversationItems.
ms.openlocfilehash: 69d362b9f769749bcc9692825b64ff486e8b60a0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530962"
---
# <a name="sortorder-conversationnodesortorder"></a>SortOrder (ConversationNodeSortOrder)

O elemento **SortOrder** especifica a ordem de classificação usada para o resultado de uma solicitação **GetConversationItems** . 
  
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

O valor de texto do elemento **SortOrder** é a ordem na qual as conversas foram solicitadas. Um valor de texto de **TreeOrderAscending** indica que as conversas são ordenadas de acordo com a árvore de conversa em ordem crescente. Um valor de texto de **TreeOrderDescending** indica que as conversas são ordenadas de acordo com a árvore de conversa em ordem decrescente. Um valor de texto de **DateOrderAscending** indica que as conversas são ordenadas de acordo com a data da conversa em ordem crescente. Um valor de texto de **DateOrderDescending** indica que as conversas são ordenadas de acordo com a data da conversa em ordem decrescente. 
  
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
   

