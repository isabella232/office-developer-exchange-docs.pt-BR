---
title: ConversationAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConversationAction
api_type:
- schema
ms.assetid: 9ecea41a-3860-4569-8e9b-284b451fc4e0
description: O elemento ConversationAction contém uma única ação a ser aplicada a uma única conversa.
ms.openlocfilehash: 04af68b4ad8442160792fd3aa9f3259058a0f3a4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531103"
---
# <a name="conversationaction"></a>ConversationAction

O **elemento ConversationAction** contém uma única ação a ser aplicada a uma única conversa. 
  
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
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Action (ConversationActionTypeType)](action-conversationactiontypetype.md) <br/> |Contém a ação a ser feita na conversa especificada pelo [elemento ConversationId.](conversationid.md) Esse elemento deve estar presente.  <br/> |
|[ConversationId](conversationid.md) <br/> |Contém o identificador da conversa que terá a ação especificada pelo elemento [Action (ConversationActionTypeType)](action-conversationactiontypetype.md) aplicado a itens na conversa. Esse elemento deve estar presente.  <br/> |
|[ContextFolderId](contextfolderid.md) <br/> |Indica a pasta direcionada para ações que usam pastas. Esse elemento deve estar presente ao copiar, excluir, mover e definir o estado de leitura em itens de conversa em uma pasta de destino.  <br/> |
|[ConversationLastSyncTime](conversationlastsynctime.md) <br/> |Contém a data e a hora em que uma conversa foi sincronizada pela última vez. Esse elemento deve estar presente ao tentar excluir todos os itens de uma conversa que foram recebidos até o horário especificado.  <br/> |
|[ProcessRightAway](processrightaway.md) <br/> |Indica se a resposta é enviada assim que a ação inicia o processamento no servidor ou se a resposta é enviada após a conclusão da ação. Esse elemento deve estar presente para que a resposta seja enviada assíncrona à ação solicitada.  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |Indica a pasta de destino para copiar e mover ações.  <br/> |
|[Categories](categories-ex15websvcsotherref.md) <br/> |Contém uma coleção de cadeias de caracteres que identificam as categorias às quais os itens de uma conversa pertencem.  <br/> |
|[EnableAlwaysDelete](enablealwaysdelete.md) <br/> |Especifica um sinalizador que permite a exclusão de todos os novos itens em uma conversa.  <br/> |
|[IsRead](isread.md) <br/> |Indica se uma mensagem foi lida.  <br/> |
|[DeleteType](deletetype.md) <br/> |Indica como os itens em uma conversa são excluídos.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ConversationActions](conversationactions.md) <br/> |Contém uma coleção de conversas e as ações a aplicar a elas.  <br/> |
   
## <a name="text-value"></a>Valor de texto

**Valores de texto do elemento ConversationAction**

|**Valor**|**Descrição**|
|:-----|:-----|
|AlwaysCategorize  <br/> |Sempre categorize a conversa.  <br/> |
|AlwaysDelete  <br/> |Sempre exclua a conversa.  <br/> |
|AlwaysMove  <br/> |Sempre mova a conversa.  <br/> |
|Excluir  <br/> |Exclua a conversa.  <br/> |
|Mover  <br/> |Mova a conversa.  <br/> |
|Copiar  <br/> |Copie a conversa.  <br/> |
|SetReadState  <br/> |De definir o estado de leitura da conversa.  <br/> |
|SetRetentionPolicy  <br/> |De definir a política de retenção para a conversa.  <br/> |
   
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

