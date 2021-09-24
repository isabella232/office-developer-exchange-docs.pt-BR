---
title: EmailAddress (NonEmptyStringType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- EmailAddress
api_type:
- schema
ms.assetid: c0c708d1-b016-4902-a294-9af44aea2050
description: O elemento EmailAddress define o endereço SMTP principal de um usuário de caixa de correio.
ms.openlocfilehash: 8740f6f7f67269de86aaa7383a7ad8f3cdf07a4a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512993"
---
# <a name="emailaddress-nonemptystringtype"></a>EmailAddress (NonEmptyStringType)

O **elemento EmailAddress** define o endereço SMTP principal de um usuário de caixa de correio. 
  
```XML
<EmailAddress/>
```

 **NonEmptyStringType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ActingAs](actingas.md) <br/> |Identifica quem o chamador está enviando como.  <br/> |
|[Caixa de Correio](mailbox.md) <br/> | Identifica um endereço de email totalmente resolvido.  <br/><br/>Veja a seguir algumas expressões XPath para este elemento:<br/><br/>`/CreateItem/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`/CreateFolder/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`CreateItem/Items/AcceptItem/ToRecipients/Mailbox`<br/><br/>`SyncFolderItemsResponseMessage/Changes/Create/CalendarItem/ConflictingMeetings/AcceptItem/CcRecipients/Mailbox`<br/><br/>Veja a seguir elementos pai adicionais do elemento Mailbox:<br/><br/>- [BccRecipients](bccrecipients.md) <br/>- [ReplyTo](replyto.md) <br/>- [Remetente](sender.md) <br/>- [De](from.md) <br/>- [Organizer](organizer.md) <br/>- [DistinguishedFolderId](distinguishedfolderid.md) <br/>- [Resolução](resolution.md) <br/>- [DLExpansion](dlexpansion.md) <br/>- [Participante](attendee.md) <br/> |
|[RoomList](roomlist.md) <br/> |Identifica uma lista de salas de reunião por endereço de email.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto que representa um endereço SMTP é necessário.
  
## <a name="remarks"></a>Comentários

O **elemento EmailAddress** pode representar endereços SMTP ou Exchange nome diferenciado (também conhecido como DN). O **elemento EmailAddress** é o único elemento [de Caixa](mailbox.md) de Correio necessário. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |Falso  <br/> |
   

