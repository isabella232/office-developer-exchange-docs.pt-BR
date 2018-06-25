---
title: MicrosoftOnline (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 0b88f02a-9c50-44b3-841b-560b24e37af5
description: O elemento MicrosoftOnline contém um valor que indica se caixas de correio do usuário está hospedada no Exchange Online ou Exchange Online como parte do Office 365.
ms.openlocfilehash: b952bfda17b30dcf29812697d225db32718d9781
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824458"
---
# <a name="microsoftonline-pox"></a>MicrosoftOnline (POX)

O elemento **MicrosoftOnline** contém um valor que indica se caixas de correio do usuário está hospedada no Exchange Online ou Exchange Online como parte do Office 365. 
  
[Descoberta automática (POX)](autodiscover-pox.md)
  
[Resposta POX)](response-pox.md)
  
[Conta (POX)](account-pox.md)
  
[MicrosoftOnline (POX)](microsoftonline-pox.md)
  
```XML
<MicrosoftOnline/>
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
|[Conta (POX)](account-pox.md) <br/> |Especifica as configurações da conta do usuário ou contém respostas de erro.  <br/> |
   
## <a name="remarks"></a>Comentários

O valor de texto indica se a caixa de correio do usuário está hospedada no Exchange Online. O valor será **true** se a caixa de correio do usuário está hospedadas no Exchange Online; Caso contrário, **false**.
  
## <a name="see-also"></a>Confira também



[Elementos de Autodiscover XML POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

