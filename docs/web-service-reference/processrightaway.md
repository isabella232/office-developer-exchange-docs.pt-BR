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
description: O elemento ProcessRightAway indica se a resposta é enviada assim que a ação inicia o processamento no servidor ou se a resposta é enviada depois que a ação foi concluída. Este elemento deve estar presente para a resposta a ser enviado assíncrona para a ação solicitada.
ms.openlocfilehash: 940f8e8fa0a53801ce1c3a45c3aecf1bdb6f519d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824898"
---
# <a name="processrightaway"></a>ProcessRightAway

O elemento **ProcessRightAway** indica se a resposta é enviada assim que a ação inicia o processamento no servidor ou se a resposta é enviada depois que a ação foi concluída. Este elemento deve estar presente para a resposta a ser enviado assíncrona para a ação solicitada. 
  
[ApplyConversationAction](applyconversationaction.md)
  
[ConversationActions](conversationactions.md)
  
[ConversationAction](conversationaction.md)
  
[ProcessRightAway](processrightaway.md)
  
```XML
<ProcessRightAway/>
```

 **xs:Boolean**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ConversationAction](conversationaction.md) <br/> |Contém uma única ação a ser aplicado a uma única conversa.  <br/> |
   
## <a name="text-value"></a>Text value

Um valor de texto de **true** indica que a resposta é enviada assim que a ação inicia o processamento no servidor. Um valor de texto de **false** indica que a resposta é enviada depois que a ação foi concluída. 
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação ApplyConversationAction](applyconversationaction-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

