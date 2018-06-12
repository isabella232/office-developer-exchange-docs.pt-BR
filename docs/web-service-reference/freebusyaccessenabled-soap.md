---
title: FreeBusyAccessEnabled (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 8d2d3276-b180-424e-a707-7256d14a1776
description: O elemento FreeBusyAccessEnabled representa o sinalizador FreeBusyAccessEnabled(). O elemento FreeBusyAccessEnabled é apenas para uso interno. Este elemento não é usado pelos clientes.
ms.openlocfilehash: 4727e7054c02a4b5d454cb880691ecc01a075327
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752367"
---
# <a name="freebusyaccessenabled-soap"></a>FreeBusyAccessEnabled (SOAP)

O elemento **FreeBusyAccessEnabled** representa o sinalizador **FreeBusyAccessEnabled()** . O elemento **FreeBusyAccessEnabled** é apenas para uso interno. Este elemento não é usado pelos clientes. 
  
```XML
<FreeBusyAccessEnabled>true | false</FreeBusyAccessEnabled>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[OrganizationRelationshipSettings (SOAP)](organizationrelationshipsettings-soap.md) <br/> |Representa uma lista de relacionamentos de organização para uma única organização.  <br/> |
   
## <a name="text-value"></a>Text value

Um valor de texto de **true** para o elemento **FreeBusyAccessEnabled** indica que a relação de compartilhamento deve ser usada para recuperar informações de disponibilidade dos usuários na organização. Um valor **false** indica que a relação de compartilhamento deve ser suprimida. 
  
## <a name="remarks"></a>Coment�rios

Use esse elemento para permitir ou impedir que informações de disponibilidade do servidor. 
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação de GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

