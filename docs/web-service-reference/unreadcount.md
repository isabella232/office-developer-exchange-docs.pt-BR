---
title: UnreadCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UnreadCount
api_type:
- schema
ms.assetid: 53b22647-1453-4707-9ea0-6a8369748d56
description: O elemento UnreadCount contém a contagem de itens não lidos em uma pasta.
ms.openlocfilehash: b4be48eae8037f5bbffaa120e71024102e7a108f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515030"
---
# <a name="unreadcount"></a>UnreadCount

O **elemento UnreadCount** contém a contagem de itens não lidos em uma pasta. 
  
```XML
<UnreadCount/>
```

 **xs:int**
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
|[Folder](folder.md) <br/> |Representa uma pasta em uma caixa de correio.  <br/> |
|[ModifiedEvent](modifiedevent.md) <br/> |Representa um evento em que um item ou pasta é modificado.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Representa uma pasta de pesquisa em uma caixa de correio.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Representa uma pasta de tarefas em uma caixa de correio.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa um valor inteiro. Essa propriedade é somente leitura.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

