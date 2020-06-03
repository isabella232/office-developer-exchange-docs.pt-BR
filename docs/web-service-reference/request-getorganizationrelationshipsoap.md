---
title: Solicitação (GetOrganizationRelationship) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 85dc155c-fad0-4756-b9a8-dedf5040a7c6
description: O elemento Request representa uma solicitação GetOrganizationRelationshipSettingsRequest (SOAP). O elemento request é somente para uso interno. Esse elemento não é usado por clientes.
ms.openlocfilehash: 90ccd3579c91c916ea645e6a3b466c9de4706421
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459557"
---
# <a name="request-getorganizationrelationship-soap"></a>Solicitação (GetOrganizationRelationship) (SOAP)

O elemento **Request** representa uma solicitação [GetOrganizationRelationshipSettingsRequest (SOAP)](getorganizationrelationshipsettingsrequest-soap.md) . O elemento **Request** é somente para uso interno. Esse elemento não é usado por clientes. 
  
```XML
<Request>
   <Domains/>
</Request>
```

 **GetOrganizationRelationshipSettingsRequest**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Domínios (SOAP)](domains-soap.md) <br/> |Representa os domínios para os quais a descoberta automática deve ser executada e que devem ser usados em uma consulta.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetOrganizationRelationshipSettingsRequestMessage (SOAP)](getorganizationrelationshipsettingsrequestmessage-soap.md) <br/> |Representa uma solicitação de operação de [operação de GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md) .  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também



[GetOrganizationRelationshipSettingsRequest (SOAP)](getorganizationrelationshipsettingsrequest-soap.md)


[Trabalhando com a descoberta automática](https://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx)

