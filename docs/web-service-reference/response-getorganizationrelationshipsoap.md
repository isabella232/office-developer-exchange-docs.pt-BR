---
title: Resposta (GetOrganizationRelationship) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: e6bbe800-3cbc-48b2-87b3-2043f575e88b
description: O elemento de resposta contém as informações de resposta GetOrganizationRelationshipSettings operação (SOAP). O elemento de resposta é apenas para uso interno. Este elemento não é usado pelos clientes.
ms.openlocfilehash: 97bef9ab9f0b860e62646703c35d539b7922a65a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825174"
---
# <a name="response-getorganizationrelationship-soap"></a>Resposta (GetOrganizationRelationship) (SOAP)

O elemento de **resposta** contém as informações de resposta [GetOrganizationRelationshipSettings operação (SOAP)](getorganizationrelationshipsettings-operation-soap.md) . O elemento de **resposta** é apenas para uso interno. Este elemento não é usado pelos clientes. 
  
```XML
<GetOrganizationRelationshipSettingsResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <OrganizationRelationshipSettingsCollection/>
</GetOrganizationRelationshipSettingResponse>
```

 **GetOrganizationRelationshipSettingsResponse**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Representa um código de erro retornado pelo serviço de descoberta automática.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Representa uma mensagem que está associada um código de erro retornado pelo serviço de descoberta automática.  <br/> |
|[OrganizationRelationshipSettingsCollection (SOAP)](organizationrelationshipsettingscollection-soap.md) <br/> |Representa uma lista de relacionamentos da organização que correspondem à consulta.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação de GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

