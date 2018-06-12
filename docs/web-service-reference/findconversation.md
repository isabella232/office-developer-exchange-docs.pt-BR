---
title: FindConversation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindConversation
api_type:
- schema
ms.assetid: 94b7083c-60cf-478b-a9af-a88f7acb30fb
description: O elemento de FindConversation define uma solicitação para localizar conversas em uma caixa de correio.
ms.openlocfilehash: 990e15f468f836d51977329c524acb439014da95
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752265"
---
# <a name="findconversation"></a>FindConversation

O elemento de **FindConversation** define uma solicitação para localizar conversas em uma caixa de correio. 
  
[FindConversation](findconversation.md)
  
```XML
<FindConversation Traversal="" ViewFilter="">
   <IndexedPageItemView/>
   <SeekToConditionPageItemView/>
   <SortOrder/>
   <ParentFolderId/>
   <MailboxScope/>
   <QueryString/>
   <ConversationShape/>
</FindConversation>
```

 **FindConversationType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

****

|**Attribute**|**Descrição**|
|:-----|:-----|
|Passagem  <br/> |Identifica os tipos de passagem subárvore. Este atributo é opcional.  <br/> |
|ViewFilter  <br/> |Identifica os filtros de exibição de tipos. Este atributo é opcional.  <br/> |
   
#### <a name="traversal-attribute-values"></a>Valores de atributos de passagem

****

|**Valor**|**Descrição**|
|:-----|:-----|
|Raso  <br/> |Indica uma passagem superficial.  <br/> |
|Profundo  <br/> |Indica um percurso profundo.  <br/> |
   
#### <a name="viewfilter-attribute-values"></a>Valores de atributo ViewFilter

****

|**Valor**|**Descrição**|
|:-----|:-----|
|Todos  <br/> |Encontre todas as conversas.  <br/> |
|Sinalizado  <br/> |Localize conversas sinalizadas.  <br/> |
|HasAttachment  <br/> |Localize conversas com anexos.  <br/> |
|ToOrCcMe  <br/> |Localize conversas endereçada ou cc seria para mim.  <br/> |
|Não lidas  <br/> |Localize conversas não lidas.  <br/> |
|TaskActive  <br/> |Encontre as tarefas ativas.  <br/> |
|TaskOverdue  <br/> |Encontre tarefas atrasadas.  <br/> |
|TaskCompleted  <br/> |Encontre tarefas concluídas.  <br/> |
|NoClutter  <br/> |Apenas para uso interno.  <br/> |
|Desorganização  <br/> |Apenas para uso interno.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[IndexedPageItemView](indexedpageitemview.md) <br/> |Descreve como paginada conversa a informação é retornada.  <br/> |
|[SeekToConditionPageItemView](seektoconditionpageitemview.md) <br/> |Especifica a condição que é usada para identificar o final de uma pesquisa, o índice inicial de uma pesquisa, as entradas máxima para retornar e as instruções de pesquisa para uma pesquisa **FindItem** ou **FindConversation** .  <br/> |
|[SortOrder](sortorder.md) <br/> |Define como os itens são classificados em uma solicitação de [operação FindConversation](findconversation-operation.md) . A propriedade de **Conversa: LastDeliveryTime** é a única propriedade que tem suporte para a classificação quando a operação **FindConversation** é usada.  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> |Identifica a pasta para procurar conversas.  <br/> |
|[MailboxScope](mailboxscope.md) <br/> |Especifica se uma pesquisa ou fetch para uma conversa deve abranger a caixa de correio primária, caixa de correio de arquivo morto ou ambos os primário e arquivar caixas de correio.  <br/> |
|[QueryString (QueryStringType)](querystring-querystringtype.md) <br/> |Especifica uma cadeia de caracteres de consulta de caixa de correio com base na sintaxe de consulta avançada (AQS).  <br/> |
|[ConversationShape](conversationshape.md) <br/> |Identifica a propriedade definida para retornar em uma resposta de [operação FindConversation](findconversation-operation.md) .  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação FindConversation](findconversation-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Conversas no EWS](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

