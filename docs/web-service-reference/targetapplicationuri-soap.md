---
title: TargetApplicationUri (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: e13c0edd-2ab1-49bb-a993-54a8db2dfbb9
description: O elemento TargetApplicationUri define o URI do aplicativo de destino. O elemento TargetApplicationUri é apenas para uso interno. Esse elemento não é usado pelos clientes.
ms.openlocfilehash: 3bed26b697fc3638782de5abd53a68fd04f031e6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522568"
---
# <a name="targetapplicationuri-soap"></a>TargetApplicationUri (SOAP)

O **elemento TargetApplicationUri** define o URI do aplicativo de destino. O **elemento TargetApplicationUri** é apenas para uso interno. Esse elemento não é usado pelos clientes. 
  
```XML
<TargetApplicationUri/>
```

 **anyURI**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[OrganizationRelationshipSettings (SOAP)](organizationrelationshipsettings-soap.md) <br/> |Representa uma lista de relações de organização para uma única organização  <br/> |
   
## <a name="remarks"></a>Comentários

Esse elemento define o URI de destino da organização externa.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nome do esquema  <br/> |Esquema de Descoberta Automática  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

