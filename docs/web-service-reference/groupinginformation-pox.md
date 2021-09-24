---
title: GroupingInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 2d8a007f-d79c-43c8-90e3-2c6d883f3a7c
description: O elemento GroupingInformation contém um valor usado para agrupar a caixa de correio do usuário para manter a afinidade ao assinar notificações em várias caixas de correio.
ms.openlocfilehash: 14e751adcd0b966907ce495a2753b2b26d812a86
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525881"
---
# <a name="groupinginformation-pox"></a>GroupingInformation (POX)

O **elemento GroupingInformation** contém um valor usado para agrupar a caixa de correio do usuário para manter [a](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx) afinidade ao assinar notificações em várias caixas de correio. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[GroupingInformation (POX)](groupinginformation-pox.md)
  
```XML
<GroupingInformation/>
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente ao Exchange servidor.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor do texto é comparado ao valor do **elemento GroupingInformation** para outras caixas de correio. Caixas de correio que têm o mesmo valor e usam o mesmo ponto de extremidade Exchange Web Services (EWS) podem ser agrupadas para manter a afinidade. Para obter mais detalhes, consulte Manter afinidade entre um grupo de [assinaturas](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)e o servidor de Caixa de Correio em Exchange .
  
## <a name="remarks"></a>Comentários

O **elemento GroupingInformation** só é aplicável aos elementos **Protocol** que têm um elemento filho [Type (POX)](type-pox.md) com um valor "EXPR". 
  
## <a name="see-also"></a>Confira também

- [Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)
- [Manter afinidade entre um grupo de assinaturas e o servidor de caixa de correio no Exchange](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)

