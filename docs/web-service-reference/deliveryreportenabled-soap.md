---
title: DeliveryReportEnabled (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2ab522bc-40ea-4e43-aa57-6d2562db35e9
description: O elemento DeliveryReportEnabled representa o sinalizador DeliveryReportEnabled(). O elemento DeliveryReportEnabled é apenas para uso interno. Este elemento não é usado pelos clientes.
ms.openlocfilehash: 089256a5f75ad92a4f11c5aaf3d175382eeee456
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751775"
---
# <a name="deliveryreportenabled-soap"></a>DeliveryReportEnabled (SOAP)

O elemento **DeliveryReportEnabled** representa o sinalizador **DeliveryReportEnabled()** . O elemento **DeliveryReportEnabled** é apenas para uso interno. Este elemento não é usado pelos clientes. 
  
```XML
<DeliveryReportEnabled>true | false</DeliveryReportEnabled>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[OrganizationRelationshipSettings (SOAP)](organizationrelationshipsettings-soap.md) <br/> |Representa uma lista de relacionamentos de organização para uma única organização.  <br/> |
   
## <a name="text-value"></a>Text value

Um valor de texto, True para o elemento DeliveryReportEnabled indica que os relatórios de entrega de usuários na organização podem ser usados. Um valor false indica que os relatórios de entrega deve ser suprimida.
  
## <a name="remarks"></a>Coment�rios

Use esse elemento para permitir ou suprimir notificações de entrega do servidor.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação de GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

