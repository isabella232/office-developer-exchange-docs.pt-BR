---
title: FreeBusyAccessEnabled (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 8d2d3276-b180-424e-a707-7256d14a1776
description: O elemento FreeBusyAccessEnabled representa o sinalizador FreeBusyAccessEnabled (). O elemento FreeBusyAccessEnabled é somente para uso interno. Esse elemento não é usado por clientes.
ms.openlocfilehash: c148d8fa1301339f8579884dc02b6c9e452f3035
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461293"
---
# <a name="freebusyaccessenabled-soap"></a>FreeBusyAccessEnabled (SOAP)

O elemento **FreeBusyAccessEnabled** representa o sinalizador **FreeBusyAccessEnabled ()** . O elemento **FreeBusyAccessEnabled** é somente para uso interno. Esse elemento não é usado por clientes. 
  
```XML
<FreeBusyAccessEnabled>true | false</FreeBusyAccessEnabled>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[OrganizationRelationshipSettings (SOAP)](organizationrelationshipsettings-soap.md) <br/> |Representa uma lista de relações de organização para uma única organização.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto **true** para o elemento **FreeBusyAccessEnabled** indica que a relação de compartilhamento deve ser usada para recuperar informações de disponibilidade de usuários na organização. Um valor **false** indica que a relação de compartilhamento deve ser suprimida. 
  
## <a name="remarks"></a>Comentários

Use este elemento para permitir ou suprimir informações de disponibilidade do servidor. 
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de descoberta automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

