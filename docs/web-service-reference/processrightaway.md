---
title: ProcessRightAway
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ProcessRightAway
api_type:
- schema
ms.assetid: f6bba68b-ae4f-41c1-b3e7-c8a31cdb1b0c
description: O elemento ProcessRightAway indica se a resposta é enviada assim que a ação inicia o processamento no servidor ou se a resposta é enviada após a conclusão da ação. Esse elemento deve estar presente para que a resposta seja enviada assíncrona à ação solicitada.
ms.openlocfilehash: 5546bbff4e1e1ef17eee94f1f42492fbf070fe59
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542992"
---
# <a name="processrightaway"></a>ProcessRightAway

O **elemento ProcessRightAway** indica se a resposta é enviada assim que a ação inicia o processamento no servidor ou se a resposta é enviada após a conclusão da ação. Esse elemento deve estar presente para que a resposta seja enviada assíncrona à ação solicitada. 
  
[ApplyConversationAction](applyconversationaction.md)
  
[ConversationActions](conversationactions.md)
  
[ConversationAction](conversationaction.md)
  
[ProcessRightAway](processrightaway.md)
  
```XML
<ProcessRightAway/>
```

 **xs:boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ConversationAction](conversationaction.md) <br/> |Contém uma única ação a ser aplicada a uma única conversa.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto **true** indica que a resposta é enviada assim que a ação inicia o processamento no servidor. Um valor de texto **false** indica que a resposta é enviada após a conclusão da ação. 
  
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services. Esse elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação ApplyConversationAction](applyconversationaction-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

