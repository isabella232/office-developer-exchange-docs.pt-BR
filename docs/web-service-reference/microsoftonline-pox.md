---
title: MicrosoftOnline (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 0b88f02a-9c50-44b3-841b-560b24e37af5
description: O elemento MicrosoftOnline contém um valor que indica se a caixa de correio do usuário está hospedada no Exchange Online ou Exchange Online como parte do Office 365.
ms.openlocfilehash: fbf230df18ca488babb1523cc7f689923eaeb55b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510942"
---
# <a name="microsoftonline-pox"></a>MicrosoftOnline (POX)

O **elemento MicrosoftOnline** contém um valor que indica se a caixa de correio do usuário está hospedada no Exchange Online ou Exchange Online como parte do Office 365. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
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
|[Account (POX)](account-pox.md) <br/> |Especifica as configurações da conta para o usuário ou contém respostas de erro.  <br/> |
   
## <a name="remarks"></a>Comentários

O valor de texto indica se a caixa de correio do usuário está hospedada em Exchange Online. O valor será **true** se a caixa de correio do usuário estiver hospedada em Exchange Online; caso contrário, **false**.
  
## <a name="see-also"></a>Confira também



[Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

