---
title: EmailAddress (NonEmptyStringType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- EmailAddress
api_type:
- schema
ms.assetid: c0c708d1-b016-4902-a294-9af44aea2050
description: O elemento EmailAddress define o endereço SMTP principal de um usuário de caixa de correio.
ms.openlocfilehash: fcc3e650d5fc32344022ed6f015d4096a4461f63
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463129"
---
# <a name="emailaddress-nonemptystringtype"></a>EmailAddress (NonEmptyStringType)

O elemento **EmailAddress** define o endereço SMTP principal de um usuário de caixa de correio. 
  
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
|[Agindo](actingas.md) <br/> |Identifica quem o chamador está enviando como.  <br/> |
|[Caixa de Correio](mailbox.md) <br/> | Identifica um endereço de email totalmente resolvido.  <br/><br/>A seguir estão algumas expressões XPath para este elemento:<br/><br/>`/CreateItem/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`/CreateFolder/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`CreateItem/Items/AcceptItem/ToRecipients/Mailbox`<br/><br/>`SyncFolderItemsResponseMessage/Changes/Create/CalendarItem/ConflictingMeetings/AcceptItem/CcRecipients/Mailbox`<br/><br/>Estes são os elementos pai adicionais do elemento de caixa de correio:<br/><br/>- [BccRecipients](bccrecipients.md) <br/>- [ReplyTo](replyto.md) <br/>- [Enviou](sender.md) <br/>- [De](from.md) <br/>- [Organizador](organizer.md) <br/>- [DistinguishedFolderId](distinguishedfolderid.md) <br/>- [Solução](resolution.md) <br/>- [DLExpansion](dlexpansion.md) <br/>- [Tende](attendee.md) <br/> |
|[RoomList](roomlist.md) <br/> |Identifica uma lista de salas de reunião por endereço de email.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto que representa um endereço SMTP é necessário.
  
## <a name="remarks"></a>Comentários

O elemento **EmailAddress** pode representar endereços distintos SMTP ou herdados do Exchange (também conhecidos como DN). O elemento **EmailAddress** é o único elemento de [caixa de correio](mailbox.md) necessário. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |Falso  <br/> |
   

