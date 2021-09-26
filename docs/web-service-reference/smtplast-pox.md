---
title: SMTPLast (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: f1aa8bd9-c6ac-41ac-8d2d-56fb20006005
description: O elemento SMTPLast especifica se o servidor SMTP (Simple Mail Transfer Protocol) exige que o email seja baixado antes de enviar emails usando o servidor SMTP.
ms.openlocfilehash: ff1e47fa1e3ebd0267879cd596a3a559f2702943
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544679"
---
# <a name="smtplast-pox"></a>SMTPLast (POX)

O **elemento SMTPLast** especifica se o servidor SMTP (Simple Mail Transfer Protocol) exige que o email seja baixado antes de enviar emails usando o servidor SMTP. 
  
- [AutoDiscover (POX)](autodiscover-pox.md)
  
- [Response (POX)](response-pox.md)
  
- [Account (POX)](account-pox.md)
  
- [Protocol (POX)](protocol-pox.md)
  
- [SMTPLast (POX)](smtplast-pox.md)
  
```xml
<SMTPLast>on or off</SMTPLast>
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

O valor do texto especifica se o servidor SMTP exige que o email seja baixado antes de enviar emails usando o servidor SMTP. Os valores possíveis **estão on** e **off**. O valor padrão está **desligado**.
  
## <a name="see-also"></a>Confira também

- [Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

