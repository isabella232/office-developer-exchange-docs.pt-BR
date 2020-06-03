---
title: Conversation
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
description: O elemento Conversation contém uma única ação a ser aplicada a uma única conversa.
ms.openlocfilehash: cb7d874f787b105d5185749dfaf1e940d2411d89
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529249"
---
# <a name="conversationaction"></a>Conversation

O elemento **Conversation** contém uma única ação a ser aplicada a uma única conversa. 
  
[ApplyConversationAction](applyconversationaction.md)
  
[ConversationActions](conversationactions.md)
  
[Conversation](conversationaction.md)
  
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
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Ação (ConversationActionTypeType)](action-conversationactiontypetype.md) <br/> |Contém a ação a ser executada na conversa especificada pelo elemento [Conversation](conversationid.md) . Esse elemento deve estar presente.  <br/> |
|[ConversationId](conversationid.md) <br/> |Contém o identificador da conversa que terá a ação especificada pelo elemento [Action (ConversationActionTypeType)](action-conversationactiontypetype.md) aplicada a itens na conversa. Esse elemento deve estar presente.  <br/> |
|[ContextFolderId](contextfolderid.md) <br/> |Indica a pasta que é direcionada para ações que usam pastas. Esse elemento deve estar presente ao copiar, excluir, mover e definir o estado de leitura em itens de conversa em uma pasta de destino.  <br/> |
|[ConversationLastSyncTime](conversationlastsynctime.md) <br/> |Contém a data e hora em que uma conversa foi sincronizada pela última vez. Esse elemento deve estar presente ao tentar excluir todos os itens em uma conversa que foram recebidos até o momento especificado.  <br/> |
|[ProcessRightAway](processrightaway.md) <br/> |Indica se a resposta é enviada assim que a ação começa o processamento no servidor ou se a resposta é enviada após a conclusão da ação. Esse elemento deve estar presente para que a resposta seja enviada de assíncrono para a ação solicitada.  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |Indica a pasta de destino para ações de copiar e mover.  <br/> |
|[Categorias](categories-ex15websvcsotherref.md) <br/> |Contém uma coleção de cadeias de caracteres que identificam as categorias às quais os itens em uma conversa pertencem.  <br/> |
|[EnableAlwaysDelete](enablealwaysdelete.md) <br/> |Especifica um sinalizador que permite a exclusão de todos os novos itens em uma conversa.  <br/> |
|[IsRead](isread.md) <br/> |Indica se uma mensagem foi lida.  <br/> |
|[DeleteType](deletetype.md) <br/> |Indica como os itens em uma conversa são excluídos.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ConversationActions](conversationactions.md) <br/> |Contém uma coleção de conversas e as ações a serem aplicadas a elas.  <br/> |
   
## <a name="text-value"></a>Valor de texto

**Valores de texto do elemento de conversaaction**

|**Valor**|**Descrição**|
|:-----|:-----|
|AlwaysCategorize  <br/> |Sempre categorizar a conversa.  <br/> |
|AlwaysDelete  <br/> |Sempre excluir a conversa.  <br/> |
|AlwaysMove  <br/> |Sempre mover a conversa.  <br/> |
|Excluir  <br/> |Exclua a conversa.  <br/> |
|Mover  <br/> |Mover a conversa.  <br/> |
|Copiar  <br/> |Copie a conversa.  <br/> |
|Setreadstate  <br/> |Definir o estado de leitura da conversa.  <br/> |
|SetRetentionPolicy  <br/> |Defina a política de retenção da conversa.  <br/> |
   
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

