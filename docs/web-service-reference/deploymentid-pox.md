---
title: DeploymentId (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: b879c134-307e-4645-bb53-55d8ba4fad9c
description: O elemento DeploymentId identifica exclusivamente a floresta do Microsoft Exchange Server 2007.
ms.openlocfilehash: 4f2548709753d8407d02218acecd9233f0ba764f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751779"
---
# <a name="deploymentid-pox"></a>DeploymentId (POX)

O elemento **DeploymentId** identifica exclusivamente a floresta do Microsoft Exchange Server 2007. 
  
- [Descoberta automática (POX)](autodiscover-pox.md)  
- [Resposta POX)](response-pox.md) 
- [Usuário (POX)](user-pox.md)  
- [DeploymentId (POX)](deploymentid-pox.md)
  
```xml
<DeploymentId/>
```

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Usuário (POX)](user-pox.md) <br/> |Fornece informações específicas do usuário.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto identifica exclusivamente a floresta do Exchange 2007 no formato GUID.
  
## <a name="remarks"></a>Comentários

Se você desinstalar e reinstalar o Exchange 2007 e usar o mesmo nome de servidor, o valor de **DeploymentId** é alterado. 
  
## <a name="see-also"></a>Confira também

- [Elementos de Autodiscover XML POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

