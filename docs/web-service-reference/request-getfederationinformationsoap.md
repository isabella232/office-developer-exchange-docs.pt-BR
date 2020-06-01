---
title: Solicitação (GetFederationInformation) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: beeb5371-f57b-4346-9753-035dd42c6bee
description: O elemento Request representa uma solicitação GetFederationInformationRequest (SOAP).
ms.openlocfilehash: dbd88537d03f6325cf0025d08c63ae486544d705
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459578"
---
# <a name="request-getfederationinformation-soap"></a>Solicitação (GetFederationInformation) (SOAP)

O elemento **Request** representa uma solicitação [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md) . 
  
```XML
<Request>
   <Domain/>
</Request>
```

 **GetFederationInformationRequest**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Domínio (GetFederationInformation) (SOAP)](domain-getfederationinformationsoap.md) <br/> |Identifica o domínio que tem uma confiança de Federação.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetFederationInformationRequestMessage (SOAP)](getfederationinformationrequestmessage-soap.md) <br/> |Prepara uma chamada para o servidor para solicitar dados de configuração para o serviço de token de segurança (STS).  <br/> |
   
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Também consulte



[Trabalhando com a descoberta automática](https://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx)

