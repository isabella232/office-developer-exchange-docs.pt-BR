---
title: Request (GetOrganizationRelationship) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 85dc155c-fad0-4756-b9a8-dedf5040a7c6
description: O elemento Request representa uma solicitação GetOrganizationRelationshipSettingsRequest (SOAP). O elemento Request é apenas para uso interno. Esse elemento não é usado pelos clientes.
ms.openlocfilehash: 06af9ca1067407f7fac9db3ff7c5b4e0fbe8a108
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512363"
---
# <a name="request-getorganizationrelationship-soap"></a>Request (GetOrganizationRelationship) (SOAP)

O **elemento Request** representa uma [solicitação GetOrganizationRelationshipSettingsRequest (SOAP).](getorganizationrelationshipsettingsrequest-soap.md) O **elemento Request** é apenas para uso interno. Esse elemento não é usado pelos clientes. 
  
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
|[Domains (SOAP)](domains-soap.md) <br/> |Representa os domínios para os quais a Descoberta Automática deve ser executado e que devem ser usados em uma consulta.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetOrganizationRelationshipSettingsRequestMessage (SOAP)](getorganizationrelationshipsettingsrequestmessage-soap.md) <br/> |Representa uma [solicitação de operação GetOrganizationRelationshipSettings (SOAP).](getorganizationrelationshipsettings-operation-soap.md)  <br/> |
   
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



[GetOrganizationRelationshipSettingsRequest (SOAP)](getorganizationrelationshipsettingsrequest-soap.md)


[Trabalhando com Descoberta Automática](https://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx)

