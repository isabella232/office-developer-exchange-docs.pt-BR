---
title: SetTeamMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 5d6ee7cc-8f88-4de2-ae5c-cabf2f2193d0
description: O elemento SetTeamMailbox contém uma solicitação para definir uma caixa de correio de site.
ms.openlocfilehash: 99b6edb891c593d7f686fbe1bceb1c0668d9251e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540472"
---
# <a name="setteammailbox"></a>SetTeamMailbox

O **elemento SetTeamMailbox** contém uma solicitação para definir uma caixa de correio de site. 
  
```XML
<SetTeamMailbox>
   <EmailAddress/>
   <SharePointSiteUrl/>
   <State/>
</SetTeamMailbox>
```

 **SetTeamMailboxRequestType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

[EmailAddress (EmailAddressType)](emailaddress-emailaddresstype.md)  |  [SharePointSiteUrl](sharepointsiteurl.md)  |  [Estado (TeamMailboxLifecycleStateType)](state-teammailboxlifecyclestatetype.md)
  
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

