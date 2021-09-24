---
title: RedirectAddr (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 0e9fa6b6-7991-4dc1-a59a-48e5f8e041e4
description: O elemento RedirectAddr especifica o endereço de email que deve ser usado para uma solicitação de Descoberta Automática subsequente.
ms.openlocfilehash: 75db62a84ccce743e73c812082ab9dbbc4fdb1cd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540591"
---
# <a name="redirectaddr-pox"></a>RedirectAddr (POX)

O **elemento RedirectAddr** especifica o endereço de email que deve ser usado para uma solicitação de Descoberta Automática subsequente. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[RedirectAddr (POX)](redirectaddr-pox.md)
  
```xml
<RedirectAddr/>
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

O valor de texto representa o endereço de email que deve ser usado para uma solicitação de Descoberta Automática subsequente.
  
## <a name="remarks"></a>Comentários

Se esse elemento estiver presente na resposta Descoberta Automática, faça outra solicitação usando o valor de texto do **elemento RedirectAddr.** 
  
## <a name="see-also"></a>Confira também



[Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

