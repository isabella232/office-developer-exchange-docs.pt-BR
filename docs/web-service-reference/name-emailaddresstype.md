---
title: Nome (EmailAddresstype)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Name
api_type:
- schema
ms.assetid: 98c58c53-9acc-4e89-9fcf-03f1b05abee1
description: O elemento name representa o nome de um usuário de caixa de correio.
ms.openlocfilehash: db6eb547b5c848dc31bbaa377692989b16771673
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44466924"
---
# <a name="name-emailaddresstype"></a>Nome (EmailAddresstype)

O elemento **Name** representa o nome de um usuário de caixa de correio. 
  
```xml
<Name/>
```

**cadeia de caracteres**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Caixa de Correio](mailbox.md) <br/> |Identifica um endereço de email totalmente resolvido.  <br/> |
|[RoomList](roomlist.md) <br/> |Identifica uma lista de salas de reunião.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto que representa uma cadeia de caracteres será necessário se esse elemento for usado.
  
## <a name="remarks"></a>Comentários

Este elemento é opcional. O elemento **Name** existe nos tipos **AttachmentType**, **EmailAddressType**e **EmailAddress** . O elemento **Name** no tipo **EmailAddress** é descrito no tópico do elemento [Name (EmailAddress)](name-emailaddress.md) . 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

