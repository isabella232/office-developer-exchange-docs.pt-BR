---
title: ProcessRightAway
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ProcessRightAway
api_type:
- schema
ms.assetid: f6bba68b-ae4f-41c1-b3e7-c8a31cdb1b0c
description: O elemento ProcessRightAway indica se a resposta é enviada assim que a ação começa o processamento no servidor ou se a resposta é enviada após a conclusão da ação. Esse elemento deve estar presente para que a resposta seja enviada de assíncrono para a ação solicitada.
ms.openlocfilehash: 58d2b926c48db5e7395df64e1f8ee9d6a8f0e73c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44434068"
---
# <a name="processrightaway"></a>ProcessRightAway

O elemento **ProcessRightAway** indica se a resposta é enviada assim que a ação começa o processamento no servidor ou se a resposta é enviada após a conclusão da ação. Esse elemento deve estar presente para que a resposta seja enviada de assíncrono para a ação solicitada. 
  
[ApplyConversationAction](applyconversationaction.md)
  
[ConversationActions](conversationactions.md)
  
[Conversation](conversationaction.md)
  
[ProcessRightAway](processrightaway.md)
  
```XML
<ProcessRightAway/>
```

 **xs: Boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Conversation](conversationaction.md) <br/> |Contém uma única ação a ser aplicada a uma única conversa.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor **true** indica que a resposta é enviada assim que a ação começa o processamento no servidor. Um valor **false** indica que a resposta é enviada após a conclusão da ação. 
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação ApplyConversationAction](applyconversationaction-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

