---
title: TokenIssuers (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 26c55228-184e-4340-bd80-f86be56f3e7a
description: Os elementos TokenIssuers representam a coleção TokenIssuer (SOAP).
ms.openlocfilehash: 352487ad3fd9c1ee7de756a109fb98a49d0cdcd7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457071"
---
# <a name="tokenissuers-soap"></a>TokenIssuers (SOAP)

Os elementos **TokenIssuers** representam a coleção [TokenIssuer (SOAP)](tokenissuer-soap.md) . 
  
```XML
<TokenIssuers>
    <TokenIssuer/>
</TokenIssuers>
```

 **TokenIssuers**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhuma
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[TokenIssuer (SOAP)](tokenissuer-soap.md) <br/> |Especifica o [URI (SOAP)](uri-soap.md) e o [ponto de extremidade (SOAP)](endpoint-soap.md) para o serviço de token de segurança.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetFederationInformationResponse (SOAP)](getfederationinformationresponse-soap.md) <br/> |Contém a resposta de [operação GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .  <br/> |
   
## <a name="remarks"></a>Comentários

O **TokenIssuers** representa uma coleção de elementos [TokenIssuer (SOAP)](tokenissuer-soap.md) a serem usados na descoberta automática. 
  
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

