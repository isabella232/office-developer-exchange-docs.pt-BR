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
ms.openlocfilehash: eb451e611c4922fa3b9cff7edec54dfb8260f5f5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837666"
---
# <a name="subscriptionid-getstreamingevents"></a>SubscriptionId (GetStreamingEvents)

O elemento **SubscriptionId** representa o identificador de uma assinatura de streaming. 
  
```XML
<SubscriptionId/>
```

 **SubscriptionIdType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetStreamingEvents](getstreamingevents.md) <br/> |Representa a operação que é usada pelos clientes para solicitar notificações de streaming do servidor.  <br/> |
   
## <a name="text-value"></a>Text value

É necessário um valor de texto. O valor de texto é um GUID.
  
## <a name="remarks"></a>Coment�rios

O GUID que representa o identificador de inscrição é gerado pelo servidor de acesso para cliente quando a assinatura é criada.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação GetStreamingEvents](getstreamingevents-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

