---
title: TokenIssuer (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2d7be675-626c-4173-89e9-e32beef81ad5
description: O elemento TokenIssuer Especifica o Uri (SOAP) e o ponto de extremidade (SOAP) para o serviço de token de segurança.
ms.openlocfilehash: 1c267fc6cbfdadd471c568473cc9aeeafb43ae2d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837756"
---
# <a name="tokenissuer-soap"></a>TokenIssuer (SOAP)

O elemento **TokenIssuer** Especifica o [Uri (SOAP)](uri-soap.md) e o [Ponto de extremidade (SOAP)](endpoint-soap.md) para o serviço de token de segurança. 
  
```XML
<TokenIssuer>
   <Uri/>
   <Endpoint/>
</TokenIssuer>
```

 **TokenIssuer**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhuma
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[URI (SOAP)](uri-soap.md) <br/> |O URI do serviço de token de segurança que emitiu o token de segurança.  <br/> |
|[Ponto de extremidade (SOAP)](endpoint-soap.md) <br/> |URI do ponto de extremidade do serviço web.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[TokenIssuers (SOAP)](tokenissuers-soap.md) <br/> |Representa uma coleção de serviço de token de segurança [Uri (SOAP)](uri-soap.md) e o [Ponto de extremidade (SOAP)](endpoint-soap.md).  <br/> |
   
## <a name="remarks"></a>Comentários

Use o elemento **TokenIssuer** para especificar o serviço de token de segurança ao usar os tokens de segurança. 
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Ver também



[Referência de web service de descoberta automática do Exchange](autodiscover-web-service-reference-for-exchange.md)
  
[Elementos de Autodiscover XML SOAP para o Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

