---
title: ConversationLastSyncTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConversationLastSyncTime
api_type:
- schema
ms.assetid: 90f8f9e3-5fc6-4a6a-bdfb-fc91fa51f8a2
description: O elemento ConversationLastSyncTime contém a data e a hora em que uma conversa foi sincronizada pela última vez. Esse elemento deve estar presente ao tentar excluir todos os itens de uma conversa que foram recebidos até o horário especificado.
ms.openlocfilehash: d71f455fa00226c84b157ba04b391b80df95f1bd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59536665"
---
# <a name="conversationlastsynctime"></a>ConversationLastSyncTime

O **elemento ConversationLastSyncTime** contém a data e a hora em que uma conversa foi sincronizada pela última vez. Esse elemento deve estar presente ao tentar excluir todos os itens de uma conversa que foram recebidos até o horário especificado. 
  
[ApplyConversationAction](applyconversationaction.md)
  
[ConversationActions](conversationactions.md)
  
[ConversationAction](conversationaction.md)
  
[ConversationLastSyncTime](conversationlastsynctime.md)
  
```XML
<ConversationLastSyncTime/>
```

 **xs:dateTime**
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

O valor de texto **do ConversationLastSyncTime** indica a última vez em que a conversa foi sincronizada. 
  
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

