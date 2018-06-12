---
title: RedirectUrl POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: c54f310f-8c99-4c37-8e73-ac87722b6229
description: O elemento RedirectUrl contém a URL do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor do acesso para cliente instalada deve ser usada para obter as configurações de descoberta automática.
ms.openlocfilehash: 3b634f1a3a3d44b6aae1a826a005149200641dcb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825027"
---
# <a name="redirecturl-pox"></a>RedirectUrl POX)

O elemento **RedirectUrl** contém a URL do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor do acesso para cliente instalada deve ser usada para obter as configurações de descoberta automática. 
  
[Descoberta automática (POX)](autodiscover-pox.md)
  
[Resposta POX)](response-pox.md)
  
[Conta (POX)](account-pox.md)
  
[RedirectUrl POX)](redirecturl-pox.md)
  
```xml
<RedirectUrl/>
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
|[Conta (POX)](account-pox.md) <br/> |Especifica as configurações da conta do usuário.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto representa a URL do servidor acesso para cliente que deve ser usado para obter as configurações de descoberta automática.
  
## <a name="remarks"></a>Coment�rios

O aplicativo cliente deve parar redirecionando após 10 redirecionamentos.
  
## <a name="see-also"></a>Confira também



[Elementos de Autodiscover XML POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

