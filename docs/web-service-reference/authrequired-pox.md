---
title: AuthRequired (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 241a23ee-d2a2-4724-b794-d0d523d480a2
description: O elemento AuthRequired especifica se a autenticação é necessária.
ms.openlocfilehash: 25e3aff6a6db719c7f466e30fd6166e602f2d418
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461622"
---
# <a name="authrequired-pox"></a>AuthRequired (POX)

O elemento **AuthRequired** especifica se a autenticação é necessária. 
  
- [Descoberta automática (POX)](autodiscover-pox.md)
  
- [Resposta (POX)](response-pox.md)
  
- [Conta (POX)](account-pox.md)
  
- [Protocol (POX)](protocol-pox.md)
  
- [AuthRequired (POX)](authrequired-pox.md)
  
```xml
<AuthRequired>on or off</AuthRequired>
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente ao computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto especifica se a autenticação é necessária. Os valores possíveis estão **ativados** e **desativados**. Se um valor não for especificado, o valor padrão será **ativado**. 
  
## <a name="see-also"></a>Confira também

- [Elementos XML de descoberta automática de POX para o Exchange](pox-autodiscover-xml-elements-for-exchange.md)

