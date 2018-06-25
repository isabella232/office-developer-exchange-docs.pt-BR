---
title: Status (HoldStatusType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fee3f1f9-e868-49fa-a554-7ff096964718
description: O elemento de Status Especifica o status de retenção para uma caixa de correio.
ms.openlocfilehash: c40dc865d2b305ac86fa40d536e2d516a14260ab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825579"
---
# <a name="status-holdstatustype"></a>Status (HoldStatusType)

O elemento de **Status** Especifica o status de retenção para uma caixa de correio. 
  
```XML
<Status> NotOnHold | Pending | OnHold | PartialHold | Failed </Status>
```

 **HoldStatusType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[MailboxHoldStatus](mailboxholdstatus.md)
  
## <a name="text-value"></a>Text value

O valor de texto do elemento de **Status** é o status de retenção de uma caixa de correio. O elemento de **Status** pode ter os valores na lista a seguir. 
  
> NotOnHold - a caixa de correio não está em espera.
    
> Pendente - a caixa de correio é pendentes que estão sendo colocados ou lançados em espera. 
    
> OnHold - isenção foi aplicada com êxito à caixa de correio. 
    
> PartialHold - isenção foi aplicada com êxito a algumas caixas de correio, mas não para todas as caixas de correio.
    
> Isenção falha - falha aplicar à caixa de correio.
    
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

