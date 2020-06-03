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
description: O elemento Type identifica o tipo da conta de email configurada.
ms.openlocfilehash: ad3570094ebe28498dfdc375cf7fc255434ba20d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465097"
---
# <a name="type-pox"></a>Tipo (POX)

O elemento **Type** identifica o tipo da conta de email configurada. 
  
[Descoberta automática (POX)](autodiscover-pox.md)
  
[Resposta (POX)](response-pox.md)
  
[Conta (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[Tipo (POX)](type-pox.md)
  
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente ao servidor Exchange.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa o tipo de conta de email. A tabela a seguir lista os valores possíveis.
  
|**Valor**|**Descrição**|
|:-----|:-----|
|Exchange  <br/> |O protocolo usado para se conectar ao servidor é o RPC do Exchange.  <br/> |
|Exhttp  <br/> |O protocolo usado para estabelecer conexão com as conexões RPC/HTTP do servidor.  <br/> |
|EXPR  <br/> |O protocolo usado para se conectar ao servidor é Exchange RPC sobre HTTP, usando um servidor proxy RPC.  <br/> Isso só é aplicável quando o elemento [AccountType (POX)](accounttype-pox.md) é definido como email.  <br/> |
|WEB  <br/> |O email é acessado a partir de um navegador da Web usando a URL especificada no elemento [servidor (POX)](server-pox.md) .  <br/> Isso só é aplicável quando o elemento [AccountType (POX)](accounttype-pox.md) é definido como email.  <br/> |
   
### <a name="version-differences"></a>Diferenças de versão

O Office 365, o Exchange Online e as versões locais do Exchange começando com o Build 15.00.0995.014 retornam um valor de "exhttp" somente se o servidor estiver configurado para aceitar conexões RPC/HTTP e o cliente incluir um cabeçalho [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) que contenha "ExHttpInfo". 
  
## <a name="see-also"></a>Confira também



[Elementos XML de descoberta automática de POX para o Exchange](pox-autodiscover-xml-elements-for-exchange.md)

