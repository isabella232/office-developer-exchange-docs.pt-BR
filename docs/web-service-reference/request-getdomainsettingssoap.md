---
title: Request (GetDomainSettings) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 3ea026fc-74f1-4118-86ae-908ed4f82a4b
description: O elemento Request contém uma solicitação para retornar configurações de domínio.
ms.openlocfilehash: fbee6479b844ac9026b0cfc0218cdc542ea0f2fd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540542"
---
# <a name="request-getdomainsettings-soap"></a>Request (GetDomainSettings) (SOAP)

O **elemento Request** contém uma solicitação para retornar configurações de domínio. 
  
```xml
<Request>
   <Domains/>
   <RequestedSettings/>
</Request>
```

 **GetDomainSettingsRequest**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Domains (SOAP)](domains-soap.md) <br/> |Representa os domínios para os quais as configurações são retornadas em uma operação [GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) ou os domínios que a organização federou em uma operação [GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md).  <br/> |
|[RequestedSettings (SOAP)](requestedsettings-soap.md) <br/> |Contém os nomes das configurações solicitadas.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetDomainSettingsRequestMessage (SOAP)](getdomainsettingsrequestmessage-soap.md) <br/> |Representa uma [solicitação de operação GetDomainSettings (SOAP).](getdomainsettings-operation-soap.md)  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de Descoberta Automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

