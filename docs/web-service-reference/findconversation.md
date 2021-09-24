---
title: FindConversation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FindConversation
api_type:
- schema
ms.assetid: 94b7083c-60cf-478b-a9af-a88f7acb30fb
description: O elemento FindConversation define uma solicitação para encontrar conversas em uma caixa de correio.
ms.openlocfilehash: e48e0d9fd71dac12fe6848031b2c056ea9a913ce
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59535167"
---
# <a name="findconversation"></a>FindConversation

O **elemento FindConversation** define uma solicitação para encontrar conversas em uma caixa de correio. 
  
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
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

****

|**Atributo**|**Descrição**|
|:-----|:-----|
|Traversal  <br/> |Identifica os tipos de sub-árvore atravessada. Esse atributo é opcional.  <br/> |
|ViewFilter  <br/> |Identifica os filtros de exibição de tipos. Esse atributo é opcional.  <br/> |
   
#### <a name="traversal-attribute-values"></a>Valores do atributo traversal

****

|**Valor**|**Descrição**|
|:-----|:-----|
|Superficial  <br/> |Indica uma rota superficial.  <br/> |
|Deep  <br/> |Indica uma profunda rotação.  <br/> |
   
#### <a name="viewfilter-attribute-values"></a>Valores de atributo ViewFilter

****

|**Valor**|**Descrição**|
|:-----|:-----|
|Todos  <br/> |Encontre todas as conversas.  <br/> |
|Sinalizado  <br/> |Encontre conversas sinalizadas.  <br/> |
|HasAttachment  <br/> |Encontre conversas com anexos.  <br/> |
|ToOrCcMe  <br/> |Encontre conversas endereçadas ou cc'd para mim.  <br/> |
|Unread  <br/> |Encontre conversas não lidas.  <br/> |
|TaskActive  <br/> |Encontre tarefas ativas.  <br/> |
|TaskOverdue  <br/> |Encontre tarefas atrasadas.  <br/> |
|TaskCompleted  <br/> |Encontre tarefas concluídas.  <br/> |
|NoClutter  <br/> |Apenas para uso interno.  <br/> |
|Email secundário  <br/> |Apenas para uso interno.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[IndexedPageItemView](indexedpageitemview.md) <br/> |Descreve como as informações de conversa com páginas são retornadas.  <br/> |
|[SeekToConditionPageItemView](seektoconditionpageitemview.md) <br/> |Especifica a condição usada para identificar o final de uma pesquisa, o índice inicial de uma pesquisa, as entradas máximas a retornar e as instruções de pesquisa para uma pesquisa **FindItem** ou **FindConversation.**  <br/> |
|[SortOrder](sortorder.md) <br/> |Define como os itens são classificação em uma solicitação de operação [FindConversation.](findconversation-operation.md) A **propriedade conversation:LastDeliveryTime** é a única propriedade com suporte para classificação quando a **operação FindConversation** é usada.  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> |Identifica a pasta para pesquisar conversas.  <br/> |
|[MailboxScope](mailboxscope.md) <br/> |Especifica se uma pesquisa ou busca para uma conversa deve abranger a caixa de correio principal, a caixa de correio de arquivo morto ou a caixa de correio principal e de arquivo morto.  <br/> |
|[QueryString (QueryStringType)](querystring-querystringtype.md) <br/> |Especifica uma cadeia de caracteres de consulta de caixa de correio com base na Sintaxe de Consulta Avançada (AQS).  <br/> |
|[ConversationShape](conversationshape.md) <br/> |Identifica o conjunto de propriedades a ser retornada em uma resposta de [operação FindConversation.](findconversation-operation.md)  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services. Esse elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação FindConversation](findconversation-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Conversas no EWS](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

