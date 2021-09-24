---
title: Status (HoldStatusType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: fee3f1f9-e868-49fa-a554-7ff096964718
description: O elemento Status especifica o status de espera de uma caixa de correio.
ms.openlocfilehash: a055dde61ae52c266f2349036c881d2b00557171
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521232"
---
# <a name="status-holdstatustype"></a>Status (HoldStatusType)

O **elemento Status** especifica o status de espera de uma caixa de correio. 
  
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

O valor de texto do elemento **Status** é o status de espera de uma caixa de correio. O **elemento Status** pode ter os valores na lista a seguir. 
  
> NotOnHold - A caixa de correio não está em espera.
    
> Pendente - A caixa de correio está pendente sendo colocada ou liberada em espera. 
    
> OnHold - A espera foi aplicada com êxito à caixa de correio. 
    
> PartialHold - A bloqueio foi aplicada com êxito a algumas caixas de correio, mas não a todas as caixas de correio.
    
> Falha - Falha na aplicação da espera à caixa de correio.
    
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
   

