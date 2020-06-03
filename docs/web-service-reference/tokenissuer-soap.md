---
title: TokenIssuer (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2d7be675-626c-4173-89e9-e32beef81ad5
description: O elemento TokenIssuer especifica o URI (SOAP) e o ponto de extremidade (SOAP) para o serviço de token de segurança.
ms.openlocfilehash: e9c0b4140de26c7ff05daf4e863b3e8a17fedc62
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526323"
---
# <a name="tokenissuer-soap"></a>TokenIssuer (SOAP)

O elemento **TokenIssuer** especifica o [URI (SOAP)](uri-soap.md) e o [ponto de extremidade (SOAP)](endpoint-soap.md) para o serviço de token de segurança. 
  
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
|[URI (SOAP)](uri-soap.md) <br/> |O URI do serviço de token de segurança que emitiu o token de segurança.  <br/> |
|[Ponto de extremidade (SOAP)](endpoint-soap.md) <br/> |O URI do ponto de extremidade do serviço Web.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[TokenIssuers (SOAP)](tokenissuers-soap.md) <br/> |Representa uma coleção de URI de serviço de token de segurança [(SOAP)](uri-soap.md) e [ponto de extremidade (SOAP)](endpoint-soap.md).  <br/> |
   
## <a name="remarks"></a>Comentários

Use o elemento **TokenIssuer** para especificar o serviço de token de segurança ao usar tokens de segurança. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também



[Referência do serviço Web de descoberta automática do Exchange](autodiscover-web-service-reference-for-exchange.md)
  
[Elementos XML de descoberta automática SOAP para o Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

