---
title: UsePOPAuth (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 28f552d8-6bb8-49b4-a45c-b2053670f1cc
description: O elemento UsePOPAuth indica se as informações de autenticação fornecidas para um tipo pop3 de conta também são usadas para o SMTP (Simple Mail Transfer Protocol).
ms.openlocfilehash: 354c027bf40ddf30cda472eb4ca0d018dca64f9c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542621"
---
# <a name="usepopauth-pox"></a>UsePOPAuth (POX)

O **elemento UsePOPAuth** indica se as informações de autenticação fornecidas para um tipo pop3 de conta também são usadas para o SMTP (Simple Mail Transfer Protocol). 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[UsePOPAuth (POX)](usepopauth-pox.md)
  
```xml
<UsePOPAuth>on or off</UsePOPAuth>
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente ao computador que está executando Microsoft Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto indica se as informações de autenticação fornecidas para um tipo POP3 de conta também são usadas para SMTP. Os valores possíveis **estão on** e **off**.
  
## <a name="remarks"></a>Comentários

O **elemento UsePOPAuth** só é usado quando [Type (POX)](type-pox.md) é SMTP. 
  
## <a name="see-also"></a>Confira também



[Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

