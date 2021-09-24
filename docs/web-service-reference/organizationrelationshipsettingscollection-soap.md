---
title: OrganizationRelationshipSettingsCollection (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 33456abf-a1b6-46da-a864-3ec8af2780de
description: O elemento OrganizationRelationshipSettingsCollection representa uma lista de relações de organização que corresponde à consulta. O elemento OrganizationRelationshipSettingsCollection é apenas para uso interno. Esse elemento não é usado pelos clientes.
ms.openlocfilehash: e3bb4c21e77bc22af051c63b714aaaef4d883609
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514232"
---
# <a name="organizationrelationshipsettingscollection-soap"></a>OrganizationRelationshipSettingsCollection (SOAP)

O **elemento OrganizationRelationshipSettingsCollection** representa uma lista de relações de organização que corresponde à consulta. O **elemento OrganizationRelationshipSettingsCollection** é apenas para uso interno. Esse elemento não é usado pelos clientes. 
  
```XML
<OrganizationRelationshipSettingsCollection>
   <OrganizationRelationshipSettings/>
</OrganizationRelationshipSettingsCollection>
```

 **OrganizationRelationshipSettingsCollection**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[OrganizationRelationshipSettings (SOAP)](organizationrelationshipsettings-soap.md) <br/> |Representa a lista de relações de organização para a organização selecionada e endereços SMTP.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Response (GetOrganizationRelationship) (SOAP)](response-getorganizationrelationshipsoap.md) <br/> |Contém as informações de resposta [getOrganizationRelationshipSettings (SOAP).](getorganizationrelationshipsettings-operation-soap.md)  <br/> |
   
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



[Operação GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

