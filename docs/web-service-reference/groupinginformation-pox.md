---
title: GroupingInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2d8a007f-d79c-43c8-90e3-2c6d883f3a7c
description: O elemento GroupingInformation contém um valor usado para agrupar a caixa de correio do usuário para manter a afinidade ao assinar notificações em várias caixas de correio.
ms.openlocfilehash: 7cab5d68f7dd5ec1f6caded5b9da6cfee03f3a67
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530075"
---
# <a name="groupinginformation-pox"></a>GroupingInformation (POX)

O elemento **GroupingInformation** contém um valor usado para agrupar a caixa de correio do usuário para [manter a afinidade](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx) ao assinar notificações em várias caixas de correio. 
  
[Descoberta automática (POX)](autodiscover-pox.md)
  
[Resposta (POX)](response-pox.md)
  
[Conta (POX)](account-pox.md)
  
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente ao servidor Exchange.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto é comparado com o valor do elemento **GroupingInformation** para outras caixas de correio. As caixas de correio que têm o mesmo valor e usam o mesmo ponto de extremidade do EWS (serviços Web do Exchange) podem ser agrupadas para manter a afinidade. Para obter mais detalhes, consulte [manter afinidade entre um grupo de assinaturas e o servidor de caixa de correio no Exchange](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx).
  
## <a name="remarks"></a>Comentários

O elemento **GroupingInformation** só é aplicável a elementos de **protocolo** que têm um elemento filho [tipo (POX)](type-pox.md) com um valor de "expr". 
  
## <a name="see-also"></a>Confira também

- [Elementos XML de descoberta automática de POX para o Exchange](pox-autodiscover-xml-elements-for-exchange.md)
- [Manter a afinidade entre um grupo de assinaturas e o servidor de caixa de correio no Exchange](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)

