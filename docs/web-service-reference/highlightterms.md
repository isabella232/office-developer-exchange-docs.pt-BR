---
title: HighlightTerms
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: ce4a2978-fd0c-41a4-ae65-aa6f5dc9a0f9
description: O elemento HighlightTerms identifica os termos realçados retornados em uma operação FindItem e uma resposta de operação FindConversation.
ms.openlocfilehash: 058c283ab4114f14b5bbffe20c6e953bd877f1e0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511541"
---
# <a name="highlightterms"></a>HighlightTerms

O **elemento HighlightTerms** identifica os termos realçados retornados em uma operação **FindItem** e uma resposta de operação **FindConversation.** 
  
```XML
<HighlightTerms>
   <Term/>
</HighlightTerms>
```

 **ArrayOfHighlightTermsType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Termo
  
### <a name="parent-elements"></a>Elementos pai

[FindConversationResponse](findconversationresponse.md)  |  [FindItemResponseMessage](finditemresponsemessage.md)
  
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
   

