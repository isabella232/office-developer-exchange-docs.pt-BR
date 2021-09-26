---
title: EcpUrl-tmCreating (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: c942758e-5ff3-4acb-9080-b8672e56f696
description: O elemento EcpUrl-tmCreating especifica uma URL parcial que pode ser combinada com o valor do elemento EcpUrl (POX) para gerar uma URL que pode ser usada para criar uma nova caixa de correio de site.
ms.openlocfilehash: 17fcd3174b70f751b07a4d6526c5b0c73d885561
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545262"
---
# <a name="ecpurl-tmcreating-pox"></a>EcpUrl-tmCreating (POX)

O **elemento EcpUrl-tmCreating** especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que pode ser usada para criar uma nova caixa de correio de site. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[EcpUrl-tmCreating (POX)](ecpurl-tmcreating-pox.md)
  
```XML
<EcpUrl-tmCreating/>
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente ao computador que está executando Microsoft Exchange Server que tem a função de servidor de Acesso para Cliente instalada.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor do texto representa uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que pode ser usada para criar uma nova caixa de correio de site. 
  
## <a name="remarks"></a>Comentários

O **elemento EcpUrl-tmCreating** é um elemento filho opcional do **elemento Protocol.** 
  
## <a name="see-also"></a>Confira também



[Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

