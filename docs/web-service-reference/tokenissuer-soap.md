---
title: TokenIssuer (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 2d7be675-626c-4173-89e9-e32beef81ad5
description: O elemento TokenIssuer especifica o Uri (SOAP) e o Ponto de Extremidade (SOAP) para o serviço de token de segurança.
ms.openlocfilehash: ea1c93493e4f47a6f2551c24586e54614f4f45e6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59527262"
---
# <a name="tokenissuer-soap"></a>TokenIssuer (SOAP)

O **elemento TokenIssuer** especifica o [Uri (SOAP)](uri-soap.md) e o Ponto de [Extremidade (SOAP)](endpoint-soap.md) para o serviço de token de segurança. 
  
```XML
<TokenIssuer>
   <Uri/>
   <Endpoint/>
</TokenIssuer>
```

 **TokenIssuer**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhuma
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Uri (SOAP)](uri-soap.md) <br/> |O URI do serviço de token de segurança que emitiu o token de segurança.  <br/> |
|[Endpoint (SOAP)](endpoint-soap.md) <br/> |O URI do ponto de extremidade do serviço Web.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[TokenIssuers (SOAP)](tokenissuers-soap.md) <br/> |Representa uma coleção de [Uri (SOAP)](uri-soap.md) e [Endpoint (SOAP)](endpoint-soap.md).  <br/> |
   
## <a name="remarks"></a>Comentários

Use o **elemento TokenIssuer** para especificar o serviço de token de segurança ao usar tokens de segurança. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de Descoberta Automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também



[Referência do serviço Web de Descoberta Automática para Exchange](autodiscover-web-service-reference-for-exchange.md)
  
[Elementos XML de Descoberta Automática SOAP para Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

