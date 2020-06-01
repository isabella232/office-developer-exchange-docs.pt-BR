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
ms.openlocfilehash: 4986a3404763e88fb3e84d52a5d30d54c810f93a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467918"
---
# <a name="deploymentid-pox"></a>DeploymentId (POX)

O elemento **DeploymentId** identifica exclusivamente a floresta do Microsoft Exchange Server 2007. 
  
- [Descoberta automática (POX)](autodiscover-pox.md)  
- [Resposta (POX)](response-pox.md) 
- [Usuário (POX)](user-pox.md)  
- [DeploymentId (POX)](deploymentid-pox.md)
  
```xml
<DeploymentId/>
```

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Usuário (POX)](user-pox.md) <br/> |Fornece informações específicas do usuário.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto identifica exclusivamente a floresta do Exchange 2007 no formato GUID.
  
## <a name="remarks"></a>Comentários

Se você desinstalar e depois reinstalar o Exchange 2007 e usar o mesmo nome de servidor, o valor **DeploymentId** será alterado. 
  
## <a name="see-also"></a>Também consulte

- [Elementos XML de descoberta automática de POX para o Exchange](pox-autodiscover-xml-elements-for-exchange.md)

