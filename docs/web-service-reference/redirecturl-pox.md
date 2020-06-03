---
title: RedirectUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: c54f310f-8c99-4c37-8e73-ac87722b6229
description: O elemento RedirectUrl contém a URL do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada que deve ser usada para obter as configurações de descoberta automática.
ms.openlocfilehash: 5400b1e7a4bb7ebebc58b6a0f1fc9bf37f5a2e22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468086"
---
# <a name="redirecturl-pox"></a>RedirectUrl (POX)

O elemento **RedirectUrl** contém a URL do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada que deve ser usada para obter as configurações de descoberta automática. 
  
[Descoberta automática (POX)](autodiscover-pox.md)
  
[Resposta (POX)](response-pox.md)
  
[Conta (POX)](account-pox.md)
  
[RedirectUrl (POX)](redirecturl-pox.md)
  
```xml
<RedirectUrl/>
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
|[Conta (POX)](account-pox.md) <br/> |Especifica as configurações de conta do usuário.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa a URL do servidor de acesso para cliente que deve ser usado para obter as configurações de descoberta automática.
  
## <a name="remarks"></a>Comentários

O aplicativo cliente deve parar de redirecionamento após 10 redirecionamentos.
  
## <a name="see-also"></a>Confira também



[Elementos XML de descoberta automática de POX para o Exchange](pox-autodiscover-xml-elements-for-exchange.md)

