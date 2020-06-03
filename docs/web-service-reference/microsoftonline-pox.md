---
title: MicrosoftOnline (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 0b88f02a-9c50-44b3-841b-560b24e37af5
description: O elemento MicrosoftOnline contém um valor que indica se a caixa de correio do usuário está hospedada no Exchange Online ou no Exchange Online como parte do Office 365.
ms.openlocfilehash: f3144a673a4c98aad821e21c562141b0ae00f426
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467981"
---
# <a name="microsoftonline-pox"></a>MicrosoftOnline (POX)

O elemento **microsoftonline** contém um valor que indica se a caixa de correio do usuário está hospedada no Exchange Online ou no Exchange Online como parte do Office 365. 
  
[Descoberta automática (POX)](autodiscover-pox.md)
  
[Resposta (POX)](response-pox.md)
  
[Conta (POX)](account-pox.md)
  
[MicrosoftOnline (POX)](microsoftonline-pox.md)
  
```XML
<MicrosoftOnline/>
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
|[Conta (POX)](account-pox.md) <br/> |Especifica as configurações de conta do usuário ou contém respostas de erro.  <br/> |
   
## <a name="remarks"></a>Comentários

O valor de texto indica se a caixa de correio do usuário está hospedada no Exchange Online. O valor será **true** se a caixa de correio do usuário estiver hospedada no Exchange Online; caso contrário, **false**.
  
## <a name="see-also"></a>Confira também



[Elementos XML de descoberta automática de POX para o Exchange](pox-autodiscover-xml-elements-for-exchange.md)

