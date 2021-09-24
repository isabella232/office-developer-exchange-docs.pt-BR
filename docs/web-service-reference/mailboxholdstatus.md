---
title: MailboxHoldStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 92608b77-8aa4-403b-a4de-01e3a60af3e0
description: O elemento MailboxHoldStatus especifica o status de espera da caixa de correio.
ms.openlocfilehash: de63acb14862e9f8cefded7130318c7f8cbd685f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540766"
---
# <a name="mailboxholdstatus"></a>MailboxHoldStatus

O **elemento MailboxHoldStatus** especifica o status de espera da caixa de correio. 
  
```XML
<MailboxHoldStatus>
   <Mailbox/>
   <Status/>
   <AdditionalInfo/>
</MailboxHoldStatus>
```

**MailboxHoldStatusType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

[Caixa de correio (cadeia de caracteres)](mailbox-string.md)  |  [Status (HoldStatusType)](status-holdstatustype.md)  |  [AdditionalInfo](additionalinfo.md)
  
### <a name="parent-elements"></a>Elementos pai

[MailboxHoldStatuses](mailboxholdstatuses.md)
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

