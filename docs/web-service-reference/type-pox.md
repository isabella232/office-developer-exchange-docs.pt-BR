---
title: Type (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 9a627244-554f-4223-b9d8-a601b81a4a1a
description: O elemento Type identifica o tipo da conta de email configurada.
ms.openlocfilehash: bb92913071509fec46736341bce56b1a00730f6b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517522"
---
# <a name="type-pox"></a>Type (POX)

O **elemento Type** identifica o tipo da conta de email configurada. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[Type (POX)](type-pox.md)
  
```XML
<Type>WEB or EXCH or EXPR or EXHTTP</Type>
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente ao Exchange servidor.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa o tipo de conta de email. A tabela a seguir lista os valores possíveis.
  
|**Valor**|**Descrição**|
|:-----|:-----|
|EXCH  <br/> |O protocolo usado para se conectar ao servidor é Exchange RPC.  <br/> |
|EXHTTP  <br/> |O protocolo usado para se conectar às conexões RPC/HTTP do servidor.  <br/> |
|EXPR  <br/> |O protocolo usado para se conectar ao servidor é Exchange RPC sobre HTTP, usando um servidor proxy RPC.  <br/> Isso só é aplicável quando o [elemento AccountType (POX)](accounttype-pox.md) é definido como email.  <br/> |
|WEB  <br/> |O email é acessado de um navegador da Web usando a URL especificada no [elemento Server (POX).](server-pox.md)  <br/> Isso só é aplicável quando o [elemento AccountType (POX)](accounttype-pox.md) é definido como email.  <br/> |
   
### <a name="version-differences"></a>Diferenças de versão

Office 365, Exchange Online e versões locais do Exchange a partir da com build 15.00.0995.014 retornarão um valor "EXHTTP" somente se o servidor estiver configurado para aceitar conexões RPC/HTTP e o cliente incluir um cabeçalho [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) que contenha "ExHttpInfo". 
  
## <a name="see-also"></a>Confira também



[Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

