---
title: Status (HoldStatusType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fee3f1f9-e868-49fa-a554-7ff096964718
description: O elemento status especifica o status de espera para uma caixa de correio.
ms.openlocfilehash: cecfdfaf67b00b6f8cf02188e7a4df7062a732e4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459984"
---
# <a name="status-holdstatustype"></a>Status (HoldStatusType)

O elemento **status** especifica o status de espera para uma caixa de correio. 
  
```XML
<Status> NotOnHold | Pending | OnHold | PartialHold | Failed </Status>
```

 **HoldStatusType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[MailboxHoldStatus](mailboxholdstatus.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do elemento **status** é o status de espera de uma caixa de correio. O elemento **status** pode ter os valores na lista a seguir. 
  
> NotOnHold-a caixa de correio não está em espera.
    
> Pendente-a caixa de correio está pendente que está sendo colocada ou liberada em espera. 
    
> OnHold-a retenção foi aplicada com êxito à caixa de correio. 
    
> PartialHold-a retenção foi aplicada com êxito a algumas caixas de correio, mas não a todas as caixas de correio.
    
> Failed-Falha ao aplicar à caixa de correio.
    
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> ||
   

