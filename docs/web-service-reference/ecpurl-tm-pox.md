---
title: EcpUrl-tm (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 3f35d5ac-55be-4d3a-ad03-7d6e9349d923
description: O elemento EcpUrl-tm especifica uma URL parcial que pode ser combinada com o valor do elemento EcpUrl (POX) para gerar uma URL que pode ser usada para acessar uma lista de todas as caixas de correio de site das quais um usuário habilitado para email é membro no momento.
ms.openlocfilehash: 5d24a198a3466bb84e14f925e4b6fa15fa229b24
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526302"
---
# <a name="ecpurl-tm-pox"></a>EcpUrl-tm (POX)

O elemento **EcpUrl-tm** especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que pode ser usada para acessar uma lista de todas as caixas de correio de site das quais um usuário habilitado para email é membro no momento. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[EcpUrl-tm (POX)](ecpurl-tm-pox.md)
  
```XML
<EcpUrl-tm/>
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

O valor do texto representa uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que pode ser usada para acessar uma lista de caixas de correio de site para o usuário. 
  
## <a name="remarks"></a>Comentários

O **elemento EcpUrl-tm** é um elemento filho opcional do **elemento Protocol.** 
  
## <a name="see-also"></a>Confira também



[Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

