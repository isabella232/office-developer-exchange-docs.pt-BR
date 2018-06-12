---
title: GroupingInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2d8a007f-d79c-43c8-90e3-2c6d883f3a7c
description: O elemento GroupingInformation contém um valor que é usado para a caixa de correio do usuário para manter a afinidade quando a assinatura de notificações em várias caixas de correio de grupo.
ms.openlocfilehash: bcde002c794ac79d9515befc0755c1f954ee8706
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823781"
---
# <a name="groupinginformation-pox"></a>GroupingInformation (POX)

O elemento **GroupingInformation** contém um valor que é usado para agrupar a caixa de correio do usuário para [manter a afinidade](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx) quando a assinatura de notificações em várias caixas de correio. 
  
[Descoberta automática (POX)](autodiscover-pox.md)
  
[Resposta POX)](response-pox.md)
  
[Conta (POX)](account-pox.md)
  
[Protocolo (POX)](protocol-pox.md)
  
[GroupingInformation (POX)](groupinginformation-pox.md)
  
```XML
<GroupingInformation/>
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
|[Protocolo (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente para o Exchange server.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto é comparado com o valor do elemento **GroupingInformation** para outras caixas de correio. Caixas de correio que têm o mesmo valor e usar o mesmo ponto de extremidade de serviços Web do Exchange (EWS) podem ser agrupadas para manter a afinidade. Para obter mais detalhes, consulte [Manter afinidade entre um grupo de assinaturas e o servidor de caixa de correio no Exchange](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx).
  
## <a name="remarks"></a>Coment�rios

O elemento **GroupingInformation** só é aplicável aos elementos de **protocolo** que têm um elemento filho de [Tipo POX ()](type-pox.md) com um valor de "EXPR". 
  
## <a name="see-also"></a>Confira também

- [Elementos de Autodiscover XML POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)
- [Manter a afinidade entre um grupo de assinaturas e o servidor de caixa de correio no Exchange](http://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)

