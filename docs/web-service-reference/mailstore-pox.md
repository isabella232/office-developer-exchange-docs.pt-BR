---
title: MailStore (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: af338f99-9e62-4124-9bff-8d7cc2008161
description: O elemento MailStore contém as especificações para conectar um cliente à caixa de correio do usuário usando o protocolo MAPI/HTTP.
ms.openlocfilehash: 543bcb8df84904f2b70d6feeabf16d1cc021f3e5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511119"
---
# <a name="mailstore-pox"></a>MailStore (POX)

O **elemento MailStore** contém as especificações para conectar um cliente à caixa de correio do usuário usando o protocolo MAPI/HTTP. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[MailStore (POX)](mailstore-pox.md)
  
```XML
<MailStore>
   <ExternalUrl/>
   <InternalUrl/>
</MailStore>
```

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ExternalUrl (POX)](externalurl-pox.md) <br/> |Contém a URL que deve ser usada para acessar a caixa de correio do usuário de fora da rede da organização por meio do protocolo MAPI/HTTP.  <br/> |
|[InternalUrl (POX)](internalurl-pox.md) <br/> |Contém a URL que deve ser usada para acessar a caixa de correio do usuário de dentro da rede da organização por meio do protocolo MAPI/HTTP.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Protocol (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente ao servidor de Acesso para Cliente.  <br/> |
   
## <a name="remarks"></a>Comentários

O **elemento MailStore** está presente em uma resposta que tem um elemento [Protocol (POX)](protocol-pox.md) com um **valor de** atributo Type de "mapiHttp". 
  
O elemento **MailStore** está disponível para clientes que implementam o protocolo MAPI/HTTP e o Exchange Online, Exchange Online como parte do Office 365 e versões locais do Exchange a partir da com build 15.00.0847.032 (Exchange Server 2013 SP1). 
  
## <a name="see-also"></a>Confira também



[Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

