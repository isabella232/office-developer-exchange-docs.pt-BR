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
description: O elemento SMTPLast Especifica se o servidor Simple Mail Transfer Protocol (SMTP) requer que o email seja baixada antes de enviar email usando o servidor SMTP.
ms.openlocfilehash: 5359f20b33855f4ef48566058bc46bd618e3b2ff
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825505"
---
# <a name="smtplast-pox"></a>SMTPLast (POX)

O elemento **SMTPLast** Especifica se o servidor Simple Mail Transfer Protocol (SMTP) requer que o email seja baixada antes de enviar email usando o servidor SMTP. 
  
- [Descoberta automática (POX)](autodiscover-pox.md)
  
- [Resposta POX)](response-pox.md)
  
- [Conta (POX)](account-pox.md)
  
- [Protocolo (POX)](protocol-pox.md)
  
- [SMTPLast (POX)](smtplast-pox.md)
  
```xml
<SMTPLast>on or off</SMTPLast>
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
|[Protocolo (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente para o computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto Especifica se o servidor SMTP requer que o email seja baixada antes de enviar email usando o servidor SMTP. Os valores possíveis são **Ativar** e **Desativar**. O valor padrão é **desativado**.
  
## <a name="see-also"></a>Confira também

- [Elementos de Autodiscover XML POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

