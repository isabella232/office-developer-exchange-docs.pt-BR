---
title: EcpUrl-extinstall (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: f81807e6-93de-4e47-afee-1e1ae6a85054
description: O elemento EcpUrl-extinstall especifica uma URL parcial que pode ser combinada com o valor do elemento EcpUrl (POX) para gerar uma URL que pode ser usada para exibir ou alterar os aplicativos de email atualmente instalados na caixa de correio do usuário.
ms.openlocfilehash: bf91b12cbcff3b08b3b13569eac9c957dea12757
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541417"
---
# <a name="ecpurl-extinstall-pox"></a>EcpUrl-extinstall (POX)

O elemento **EcpUrl-extinstall** especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que pode ser usada para exibir ou alterar os aplicativos de email atualmente instalados na caixa de correio do usuário. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[EcpUrl-extinstall (POX)](ecpurl-extinstall-pox.md)
  
```XML
<EcpUrl-extinstall/>
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

O valor do texto representa uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que pode ser usada para exibir ou alterar os aplicativos de email atualmente instalados na caixa de correio do usuário. 
  
## <a name="remarks"></a>Comentários

O **elemento EcpUrl-extinstall** é um elemento filho opcional do **elemento Protocol.** 
  
## <a name="see-also"></a>Confira também



[Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

