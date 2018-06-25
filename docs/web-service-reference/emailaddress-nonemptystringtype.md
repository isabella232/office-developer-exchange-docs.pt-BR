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
ms.openlocfilehash: fcf2839c1e2e40a22d6b6a856608f52f2c9c2a1a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751991"
---
# <a name="emailaddress-nonemptystringtype"></a>EmailAddress (NonEmptyStringType)

O elemento **EmailAddress** define o endereço SMTP principal de um usuário de caixa de correio. 
  
```XML
<EmailAddress/>
```

 **NonEmptyStringType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ActingAs](actingas.md) <br/> |Identifica que o chamador está enviando como.  <br/> |
|[Caixa de correio](mailbox.md) <br/> | Identifica um endereço de email totalmente resolvido.  <br/><br/>A seguir estão algumas expressões XPath para esse elemento:<br/><br/>`/CreateItem/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`/CreateFolder/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`CreateItem/Items/AcceptItem/ToRecipients/Mailbox`<br/><br/>`SyncFolderItemsResponseMessage/Changes/Create/CalendarItem/ConflictingMeetings/AcceptItem/CcRecipients/Mailbox`<br/><br/>Estes são os elementos adicionais pai do elemento de caixa de correio:<br/><br/>- [BccRecipients](bccrecipients.md) <br/>- [ReplyTo](replyto.md) <br/>- [Remetente](sender.md) <br/>- [De](from.md) <br/>- [Organizador](organizer.md) <br/>- [DistinguishedFolderId](distinguishedfolderid.md) <br/>- [Resolução](resolution.md) <br/>- [DLExpansion](dlexpansion.md) <br/>- [Participante](attendee.md) <br/> |
|[RoomList](roomlist.md) <br/> |Identifica uma lista de salas de reunião pelo endereço de email.  <br/> |
   
## <a name="text-value"></a>Text value

É necessário um valor de texto que representa um endereço SMTP.
  
## <a name="remarks"></a>Comentários

O elemento **EmailAddress** pode representar SMTP ou herdado do Exchange diferenciados endereços nome (também conhecido como DN). O elemento **EmailAddress** é o único elemento de [caixa de correio](mailbox.md) necessário. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   

