---
title: SubscriptionId (GetStreamingEvents)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 3f86c178-2311-4844-82db-c2a0e469d116
description: O elemento SubscriptionId representa o identificador de uma assinatura de streaming.
ms.openlocfilehash: 8931fda5087fa985c646da328a0cb27fa2c2a708
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540374"
---
# <a name="subscriptionid-getstreamingevents"></a>SubscriptionId (GetStreamingEvents)

O **elemento SubscriptionId** representa o identificador de uma assinatura de streaming. 
  
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
|[GetStreamingEvents](getstreamingevents.md) <br/> |Representa a operação usada pelos clientes para solicitar notificações de streaming do servidor.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é necessário. O valor do texto é um GUID.
  
## <a name="remarks"></a>Comentários

O GUID que representa o identificador de assinatura é gerado pelo servidor de Acesso para Cliente quando a assinatura é criada.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetStreamingEvents](getstreamingevents-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

