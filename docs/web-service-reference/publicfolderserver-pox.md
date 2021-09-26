---
title: PublicFolderServer (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 37ad46ab-7817-4fdd-ad2d-26cb525cd96b
description: O elemento PublicFolderServer contém o FQDN (nome de domínio totalmente qualificado) do servidor de pastas públicas do usuário.
ms.openlocfilehash: d81d7cdc10cdf0c5f06e9c4bf9e1c8a089de293d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542950"
---
# <a name="publicfolderserver-pox"></a>PublicFolderServer (POX)

O **elemento PublicFolderServer** contém o FQDN (nome de domínio totalmente qualificado) do servidor de pastas públicas do usuário. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[PublicFolderServer (POX)](publicfolderserver-pox.md)
  
```XML
<PublicFolderServer/>
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

O valor de texto representa o FQDN do servidor de pasta pública do usuário.
  
## <a name="remarks"></a>Comentários

O **elemento PublicFolderServer** é um elemento filho opcional do **elemento Protocol.** 
  
## <a name="see-also"></a>Confira também



[Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

