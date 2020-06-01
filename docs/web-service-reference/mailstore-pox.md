---
title: MailStore (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: af338f99-9e62-4124-9bff-8d7cc2008161
description: O elemento MailStore contém as especificações para conectar um cliente à caixa de correio do usuário usando o protocolo MAPI/HTTP.
ms.openlocfilehash: 635228fcfeb3ad791c845050b82666a6e060b229
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459788"
---
# <a name="mailstore-pox"></a>MailStore (POX)

O elemento **MailStore** contém as especificações para conectar um cliente à caixa de correio do usuário usando o protocolo MAPI/http. 
  
[Descoberta automática (POX)](autodiscover-pox.md)
  
[Resposta (POX)](response-pox.md)
  
[Conta (POX)](account-pox.md)
  
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente ao servidor de acesso para cliente.  <br/> |
   
## <a name="remarks"></a>Comentários

O elemento **MailStore** está presente em uma resposta que tem um elemento [Protocol (POX)](protocol-pox.md) com um valor de atributo **Type** de "mapiHttp". 
  
O elemento **MailStore** está disponível para clientes que implementam o protocolo MAPI/http e direcionam o Exchange Online, o Exchange Online como parte do Office 365 e as versões locais do Exchange a partir do Build 15.00.0847.032 (exchange server 2013 SP1). 
  
## <a name="see-also"></a>Também consulte



[Elementos XML de descoberta automática de POX para o Exchange](pox-autodiscover-xml-elements-for-exchange.md)

