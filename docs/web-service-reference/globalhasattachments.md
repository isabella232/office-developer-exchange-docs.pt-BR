---
title: GlobalHasAttachments
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GlobalHasAttachments
api_type:
- schema
ms.assetid: 3d075e93-14bc-479d-957f-9b7873d1db39
description: O elemento GlobalHasAttachments contém um valor que indica se pelo menos um item de conversa em uma caixa de correio tem um anexo.
ms.openlocfilehash: a5a12290e9eee4fb29ce7b5f24e9a24c44d8179e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525874"
---
# <a name="globalhasattachments"></a>GlobalHasAttachments

O **elemento GlobalHasAttachments** contém um valor que indica se pelo menos um item de conversa em uma caixa de correio tem um anexo. 
  
[FindConversationResponse](findconversationresponse.md)
  
[Conversas](conversations-ex15websvcsotherref.md)
  
[Conversation (ConversationType)](conversation-conversationtype.md)
  
[GlobalHasAttachments](globalhasattachments.md)
  
```XML
<GlobalHasAttachments/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Conversation (ConversationType)](conversation-conversationtype.md) <br/> |Representa uma única conversa.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor do **elemento GlobalHasAttachments** indica se pelo menos um item de conversa em uma caixa de correio tem um anexo. Um valor de texto que representa um valor Boolean é necessário. Um valor verdadeiro **significa** que a conversa tem pelo menos um anexo visível. Um valor false **significa** que a conversa não tem anexos ou tem apenas anexos ocultos. 
  
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services. Esse elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação FindConversation](findconversation-operation.md)
  
[Operação ApplyConversationAction](applyconversationaction-operation.md)


[Conversas no EWS](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

