---
title: RequestType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RequestType
api_type:
- schema
ms.assetid: 4e657e57-528f-4250-a99c-f9850bbbcec5
description: O elemento RequestType identifica se uma solicitação de proxy é uma solicitação entre sites ou entre florestas.
ms.openlocfilehash: 3390381b903c7a39a1d2ea6cae80b3fbc07eba43
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541851"
---
# <a name="requesttype"></a>RequestType

O **elemento RequestType** identifica se uma solicitação de proxy é uma solicitação entre sites ou entre florestas. 
  
```xml
<RequestType>CrossSite or CrossForest</RequestType>
```

 **AvailabilityProxyRequestType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

Esse elemento não tem um pai no esquema. Esse elemento é usado no header SOAP. Para obter mais informações sobre como esse elemento é usado, consulte o arquivo WSDL.
  
## <a name="text-value"></a>Valor de texto

Um valor de texto é necessário para esse elemento. Veja a seguir os valores possíveis:
  
- CrossSite
    
- CrossForest
    
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

