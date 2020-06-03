---
title: Tempo limite (duração)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bb15f9a7-8ea5-4765-9877-762c3f98bf50
description: O elemento timeout especifica o período de tempo antes de o tempo limite de uma assinatura pull ter expirado pelo servidor.
ms.openlocfilehash: b5b0e77d794080cd8e0da1e14acf4cb059b80b08
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460278"
---
# <a name="timeout-duration"></a>Tempo limite (duração)

O elemento **Timeout** especifica o período de tempo antes de o tempo limite de uma assinatura pull ter expirado pelo servidor. 
  
```XML
<Timeout></Timeout>
```

 **SubscriptionTimeoutType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[PullSubscriptionRequest](pullsubscriptionrequest.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do elemento **Timeout** é o período de tempo, em minutos, antes que uma assinatura pull seja esgotada pelo servidor. O valor mínimo é 1; o valor máximo é 1440. 
  
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
   

