---
title: SMTPLast (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: f1aa8bd9-c6ac-41ac-8d2d-56fb20006005
description: O elemento SMTPLast especifica se o servidor SMTP exige que o email seja baixado antes de enviar emails usando o servidor SMTP.
ms.openlocfilehash: 7019da28ffa196a9abc8798aa75aff2756198da3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468429"
---
# <a name="smtplast-pox"></a>SMTPLast (POX)

O elemento **SMTPLast** especifica se o servidor SMTP exige que o email seja baixado antes de enviar emails usando o servidor SMTP. 
  
- [Descoberta automática (POX)](autodiscover-pox.md)
  
- [Resposta (POX)](response-pox.md)
  
- [Conta (POX)](account-pox.md)
  
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente ao computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto especifica se o servidor SMTP exige que o email seja baixado antes de enviar emails usando o servidor SMTP. Os valores possíveis estão **ativados** e **desativados**. O valor padrão é **desativado**.
  
## <a name="see-also"></a>Confira também

- [Elementos XML de descoberta automática de POX para o Exchange](pox-autodiscover-xml-elements-for-exchange.md)

