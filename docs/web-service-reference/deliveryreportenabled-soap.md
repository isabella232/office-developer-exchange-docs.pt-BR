---
title: DeliveryReportEnabled (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2ab522bc-40ea-4e43-aa57-6d2562db35e9
description: O elemento DeliveryReportEnabled representa o sinalizador DeliveryReportEnabled (). O elemento DeliveryReportEnabled é somente para uso interno. Esse elemento não é usado por clientes.
ms.openlocfilehash: 2a163b3e6ceaa169cc8f76f395b7d501419a31ed
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458471"
---
# <a name="deliveryreportenabled-soap"></a>DeliveryReportEnabled (SOAP)

O elemento **DeliveryReportEnabled** representa o sinalizador **DeliveryReportEnabled ()** . O elemento **DeliveryReportEnabled** é somente para uso interno. Esse elemento não é usado por clientes. 
  
```XML
<DeliveryReportEnabled>true | false</DeliveryReportEnabled>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[OrganizationRelationshipSettings (SOAP)](organizationrelationshipsettings-soap.md) <br/> |Representa uma lista de relações de organização para uma única organização.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto true para o elemento DeliveryReportEnabled indica que os relatórios de entrega de usuários na organização podem ser usados. Um valor false indica que os relatórios de entrega devem suprimir.
  
## <a name="remarks"></a>Comentários

Use este elemento para permitir ou suprimir os relatórios de entrega do servidor.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Também consulte

- [Operação GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

