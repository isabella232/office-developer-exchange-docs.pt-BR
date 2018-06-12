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
description: O elemento de solicitação representa uma solicitação de GetFederationInformationRequest (SOAP).
ms.openlocfilehash: 0fb9301c2f318aa2c27155675dd3c43b41aabecd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825119"
---
# <a name="request-getfederationinformation-soap"></a>Solicitação (GetFederationInformation) (SOAP)

O elemento de **solicitação** representa uma solicitação de [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md) . 
  
```XML
<Request>
   <Domain/>
</Request>
```

 **GetFederationInformationRequest**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Domínio (GetFederationInformation) (SOAP)](domain-getfederationinformationsoap.md) <br/> |Identifica o domínio que tenha uma relação de confiança de Federação.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetFederationInformationRequestMessage (SOAP)](getfederationinformationrequestmessage-soap.md) <br/> |Prepara uma chamada para o servidor para dados de configuração de solicitação para o serviço de token de segurança (STS).  <br/> |
   
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Ver também



[Trabalhando com a descoberta automática](http://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx)

