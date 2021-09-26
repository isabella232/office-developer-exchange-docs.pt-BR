---
title: Timeout (duration)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: bb15f9a7-8ea5-4765-9877-762c3f98bf50
description: O elemento Timeout especifica o período de tempo antes que uma assinatura pull seja temporada pelo servidor.
ms.openlocfilehash: a5a9e094c25f609c0bcfa207ab96ae7f0877f43f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545766"
---
# <a name="timeout-duration"></a>Timeout (duration)

O **elemento Timeout** especifica o período de tempo antes que uma assinatura pull seja temporada pelo servidor. 
  
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

O valor de texto do **elemento Timeout** é o período de tempo, em minutos, antes que uma assinatura pull seja o tempo de tempo de tempo do servidor. O valor mínimo é 1; o valor máximo é 1440. 
  
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
   

