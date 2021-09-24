---
title: Response (GetFederationInformation) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: ca48a4b3-5006-4bb7-973e-d9137ce67e16
description: O elemento Response contém as informações de resposta da operação GetFederationInformation (SOAP).
ms.openlocfilehash: b5618dc1d2c862e504ea3134b28edca39c71f62c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523521"
---
# <a name="response-getfederationinformation-soap"></a>Response (GetFederationInformation) (SOAP)

O **elemento Response** contém as informações de resposta da operação [GetFederationInformation (SOAP).](getfederationinformation-operation-soap.md) 
  
```XML
<Response>
   <ErrorCode/>
   <ErrorMessage/>
   <ApplicationUri/>
   <Domains/>
</Response>
```

 **GetFederationInformationResponse**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Representa um código de erro retornado pelo serviço descoberta automática.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Representa uma mensagem associada a um código de erro retornado pelo serviço de Descoberta Automática.  <br/> |
|[ApplicationUri (SOAP)](applicationuri-soap.md) <br/> |Define o local de um aplicativo.  <br/> |
|[Domains (SOAP)](domains-soap.md) <br/> |Representa a coleção de domínios para as configurações para as quais são retornadas em uma operação [GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)ou os domínios que a organização federou em uma operação [GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md).  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetFederationInformationResponseMessage (SOAP)](getfederationinformationresponsemessage-soap.md) <br/> |Define uma resposta a uma [solicitação getFederationInformation operation (SOAP).](getfederationinformation-operation-soap.md)  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de Descoberta Automática  <br/> |
|Arquivo de validação  <br/> |messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)

