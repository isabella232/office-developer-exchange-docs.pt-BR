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
description: O elemento FindConversation define uma solicitação para localizar conversas em uma caixa de correio.
ms.openlocfilehash: 98d692132ed9375d981c95d24600b0e2c4b1d8c1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462644"
---
# <a name="findconversation"></a>FindConversation

O elemento **FindConversation** define uma solicitação para localizar conversas em uma caixa de correio. 
  
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
|Passagem  <br/> |Identifica os tipos de travessia da subárvore. Esse atributo é opcional.  <br/> |
|ViewFilter  <br/> |Identifica os filtros de exibição de tipos. Esse atributo é opcional.  <br/> |
   
#### <a name="traversal-attribute-values"></a>Valores de atributos de passagem

****

|**Valor**|**Descrição**|
|:-----|:-----|
|Superficial  <br/> |Indica uma passagem superficial.  <br/> |
|Detalhadas  <br/> |Indica uma passagem detalhada.  <br/> |
   
#### <a name="viewfilter-attribute-values"></a>Valores de atributo ViewFilter

****

|**Valor**|**Descrição**|
|:-----|:-----|
|Todos  <br/> |Encontre todas as conversas.  <br/> |
|Indicado  <br/> |Encontre conversas sinalizadas.  <br/> |
|HasAttachment  <br/> |Encontre conversas com anexos.  <br/> |
|ToOrCcMe  <br/> |Encontre conversas endereçadas ou CC para mim.  <br/> |
|Unread  <br/> |Localizar conversas não lidas.  <br/> |
|TaskActive  <br/> |Encontre tarefas ativas.  <br/> |
|TaskOverdue  <br/> |Encontre tarefas atrasadas.  <br/> |
|TaskCompleted  <br/> |Localizar tarefas concluídas.  <br/> |
|Desorganização  <br/> |Apenas para uso interno.  <br/> |
|Email secundário  <br/> |Apenas para uso interno.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[IndexedPageItemView](indexedpageitemview.md) <br/> |Descreve como as informações de conversa paginadas são retornadas.  <br/> |
|[SeekToConditionPageItemView](seektoconditionpageitemview.md) <br/> |Especifica a condição usada para identificar o final de uma pesquisa, o índice inicial de uma pesquisa, o número máximo de entradas a serem retornadas e as direções de pesquisa para uma pesquisa do **FindItem** ou do **FindConversation** .  <br/> |
|[SortOrder](sortorder.md) <br/> |Define como os itens são classificados em uma solicitação de [operação FindConversation](findconversation-operation.md) . A propriedade **Conversation: LastDeliveryTime** é a única propriedade que tem suporte para a classificação quando a operação **FindConversation** é usada.  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> |Identifica a pasta na qual as conversas serão pesquisadas.  <br/> |
|[MailboxScope](mailboxscope.md) <br/> |Especifica se uma pesquisa ou busca de uma conversa deve abranger a caixa de correio principal, a caixa de correio de arquivo morto ou a caixa de correio principal e de arquivo morto.  <br/> |
|[QueryString (QueryStringtype)](querystring-querystringtype.md) <br/> |Especifica uma cadeia de caracteres de consulta de caixa de correio baseada na sintaxe de consulta avançada (AQS).  <br/> |
|[ConversationShape](conversationshape.md) <br/> |Identifica o conjunto de propriedades a ser retornado em uma resposta de [operação FindConversation](findconversation-operation.md) .  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
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

