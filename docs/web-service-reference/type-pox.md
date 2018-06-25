---
title: Tipo (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 9a627244-554f-4223-b9d8-a601b81a4a1a
description: O elemento de tipo identifica o tipo da conta de email configurada.
ms.openlocfilehash: 6e1349769c6a5349304f576419e0c609d3edd9a0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837807"
---
# <a name="type-pox"></a>Tipo (POX)

O **tipo** de elemento identifica o tipo da conta de email configurada. 
  
[Descoberta automática (POX)](autodiscover-pox.md)
  
[Resposta POX)](response-pox.md)
  
[Conta (POX)](account-pox.md)
  
[Protocolo (POX)](protocol-pox.md)
  
[Tipo (POX)](type-pox.md)
  
```XML
<Type>WEB or EXCH or EXPR or EXHTTP</Type>
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

O valor de texto representa o tipo de conta de email. A tabela a seguir lista os valores possíveis.
  
|**Valor**|**Descrição**|
|:-----|:-----|
|EXCH  <br/> |O protocolo usado para conectar ao servidor é RPC do Exchange.  <br/> |
|EXHTTP  <br/> |O protocolo que é usado para conectar-se para as conexões de servidor RPC/HTTP.  <br/> |
|EXPR  <br/> |O protocolo que é usado para conectar ao servidor é Exchange RPC sobre HTTP, usando um servidor proxy RPC.  <br/> Isso só é aplicável quando o elemento [AccountType POX ()](accounttype-pox.md) é definido como email.  <br/> |
|WEB  <br/> |Email é acessada a partir de um navegador da Web usando a URL especificada no elemento [Server POX ()](server-pox.md) .  <br/> Isso só é aplicável quando o elemento [AccountType POX ()](accounttype-pox.md) é definido como email.  <br/> |
   
### <a name="version-differences"></a>Diferenças de versão

O Office 365, Exchange Online e versões de local do Exchange começando com compilação 15.00.0995.014 retorno um valor igual a "EXHTTP" somente se o servidor está configurado para aceitar conexões de RPC/HTTP e o cliente incluir um cabeçalho [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) que contém "ExHttpInfo". 
  
## <a name="see-also"></a>Confira também



[Elementos de Autodiscover XML POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

