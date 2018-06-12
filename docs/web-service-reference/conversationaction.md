---
title: ConversationAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationAction
api_type:
- schema
ms.assetid: 9ecea41a-3860-4569-8e9b-284b451fc4e0
description: O elemento ConversationAction contém uma única ação a ser aplicado a uma única conversa.
ms.openlocfilehash: 45cd6df3aba94062bd5aa0ddf9367e8cf118dc6b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751521"
---
# <a name="conversationaction"></a>ConversationAction

O elemento **ConversationAction** contém uma única ação a ser aplicado a uma única conversa. 
  
[ApplyConversationAction](applyconversationaction.md)
  
[ConversationActions](conversationactions.md)
  
[ConversationAction](conversationaction.md)
  
```XML
<ConversationAction>
   <Action/>
   <ConversationId/>
   <ContextFolderId/>
   <ConversationLastSyncTime/>
   <ProcessRightAway/>
   <DestinationFolderId/>
   <Categories/>
   <EnableAlwaysDelete/>
   <IsRead/>
   <DeleteType/>
</ConversationAction>
```

 **ConversationActionType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Ação (ConversationActionTypeType)](action-conversationactiontypetype.md) <br/> |Contém a ação a ser executada a conversa especificada pelo elemento [ConversationId](conversationid.md) . Este elemento deve estar presente.  <br/> |
|[ConversationId](conversationid.md) <br/> |Contém o identificador da conversa que terá a ação especificada pelo elemento [Action (ConversationActionTypeType)](action-conversationactiontypetype.md) aplicado aos itens da conversa. Este elemento deve estar presente.  <br/> |
|[ContextFolderId](contextfolderid.md) <br/> |Indica a pasta que está programada para ações que usam pastas. Este elemento deve estar presente quando copiar, excluir, mover e definindo o estado lido em itens da conversa em uma pasta de destino.  <br/> |
|[ConversationLastSyncTime](conversationlastsynctime.md) <br/> |Contém a data e hora da última sincronização uma conversa. Este elemento deve estar presente durante a tentativa de excluir todos os itens em uma conversa que foram recebidos do período especificado.  <br/> |
|[ProcessRightAway](processrightaway.md) <br/> |Indica se a resposta é enviada assim que a ação inicia o processamento no servidor ou se a resposta é enviada depois que a ação foi concluída. Este elemento deve estar presente para a resposta a ser enviado assíncrona para a ação solicitada.  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |Indica a pasta de destino para cópia e mover ações.  <br/> |
|[Categorias](categories-ex15websvcsotherref.md) <br/> |Contém uma coleção de cadeias de caracteres que identificam as categorias às quais os itens em uma conversa pertencem.  <br/> |
|[EnableAlwaysDelete](enablealwaysdelete.md) <br/> |Especifica um sinalizador que permite a exclusão de todos os novos itens em uma conversa.  <br/> |
|[Foi lido](isread.md) <br/> |Indica se uma mensagem foi lido.  <br/> |
|[DeleteType](deletetype.md) <br/> |Indica como os itens em uma conversa são excluídos.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ConversationActions](conversationactions.md) <br/> |Contém uma coleção de conversas e as ações a serem aplicadas a eles.  <br/> |
   
## <a name="text-value"></a>Text value

**Valores de texto do elemento ConversationAction**

|**Valor**|**Descrição**|
|:-----|:-----|
|AlwaysCategorize  <br/> |Sempre categorize a conversa.  <br/> |
|AlwaysDelete  <br/> |Exclua sempre a conversa.  <br/> |
|AlwaysMove  <br/> |Sempre mover a conversa.  <br/> |
|Excluir  <br/> |Exclua a conversa.  <br/> |
|Mover  <br/> |Mova a conversa.  <br/> |
|Cópia  <br/> |Copie a conversa.  <br/> |
|SetReadState  <br/> |Defina o estado de leitura da conversa.  <br/> |
|SetRetentionPolicy  <br/> |Defina a política de retenção para a conversa.  <br/> |
   
## <a name="remarks"></a>Coment�rios

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

