---
title: SortOrder (ConversationNodeSortOrder)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9c4295c-8089-4533-b92f-2051eae9afeb
description: O elemento SortOrder Especifica a ordem de classificação usada para o resultado de uma solicitação de GetConversationItems.
ms.openlocfilehash: 397aead62d32e72f991af783bff02e79a6e4b0fb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825520"
---
# <a name="sortorder-conversationnodesortorder"></a>SortOrder (ConversationNodeSortOrder)

O elemento **SortOrder** Especifica a ordem de classificação usada para o resultado de uma solicitação de **GetConversationItems** . 
  
```XML
<SortOrder>TreeOrderAscending | TreeOrderDescending | DateOrderAscending | DateOrderDescending</SortOrder>
```

 **ConversationNodeSortOrder**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[GetConversationItems](getconversationitems.md)
  
## <a name="text-value"></a>Text value

O valor de texto do elemento **SortOrder** é a ordem na qual as conversas ordenadas. Um valor de texto de **TreeOrderAscending** indica que as conversas são ordenadas de acordo com a árvore de conversa em ordem crescente. Um valor de texto de **TreeOrderDescending** indica que as conversas são ordenadas de acordo com a árvore de conversa em ordem decrescente. Um valor de texto de **DateOrderAscending** indica que as conversas são ordenadas de acordo com a data de conversa em ordem crescente. Um valor de texto de **DateOrderDescending** indica que as conversas são ordenadas de acordo com a data de conversa em ordem decrescente. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

