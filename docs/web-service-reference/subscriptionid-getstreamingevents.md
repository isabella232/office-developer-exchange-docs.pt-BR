---
title: SubscriptionId (GetStreamingEvents)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3f86c178-2311-4844-82db-c2a0e469d116
description: O elemento SubscriptionId representa o identificador de uma assinatura de streaming.
ms.openlocfilehash: babf02c514e7fe8711f51ac52e425a18f3ab47f7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457995"
---
# <a name="subscriptionid-getstreamingevents"></a>SubscriptionId (GetStreamingEvents)

O elemento **SubscriptionId** representa o identificador de uma assinatura de streaming. 
  
```XML
<SubscriptionId/>
```

 **SubscriptionIdType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetStreamingEvents](getstreamingevents.md) <br/> |Representa a operação usada por clientes para solicitar notificações de streaming do servidor.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é obrigatório. O valor de texto é um GUID.
  
## <a name="remarks"></a>Comentários

O GUID que representa o identificador de assinatura é gerado pelo servidor de acesso para cliente quando a assinatura é criada.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetStreamingEvents](getstreamingevents-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

