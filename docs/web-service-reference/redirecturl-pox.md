---
title: RedirectUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: c54f310f-8c99-4c37-8e73-ac87722b6229
description: O elemento RedirectUrl contém a URL do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor acesso para cliente instalada que deve ser usada para obter configurações de Descoberta Automática.
ms.openlocfilehash: d515f3f79f2370dc496614bab0a3f77300ad4e30
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513525"
---
# <a name="redirecturl-pox"></a>RedirectUrl (POX)

O **elemento RedirectUrl** contém a URL do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor acesso para cliente instalada que deve ser usada para obter configurações de Descoberta Automática. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
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
|[Account (POX)](account-pox.md) <br/> |Especifica as configurações da conta para o usuário.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa a URL do servidor de Acesso para Cliente que deve ser usada para obter configurações de Descoberta Automática.
  
## <a name="remarks"></a>Comentários

O aplicativo cliente deve parar de redirecionar após 10 redirecionamentos.
  
## <a name="see-also"></a>Confira também



[Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

