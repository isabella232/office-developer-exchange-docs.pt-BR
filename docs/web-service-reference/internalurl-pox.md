---
title: InternalUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 4649baa9-eec9-426d-952b-361818c25fe0
description: O elemento InternalUrl contém a URL para conectar um cliente ao servidor do livro de endereços ou à caixa de correio de um usuário de dentro da organização do usuário usando o protocolo MAPI/HTTP.
ms.openlocfilehash: 4ce04743c7d0f260439849a02f8f6d389f6c83fa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542193"
---
# <a name="internalurl-pox"></a>InternalUrl (POX)

O **elemento InternalUrl** contém a URL para conectar um cliente ao servidor do livro de endereços ou à caixa de correio de um usuário de dentro da organização do usuário usando o protocolo MAPI/HTTP. 
  
```XML
<InternalUrl/>
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
|[AddressBook (POX)](addressbook-pox.md) <br/> |Contém as especificações para conectar um cliente ao servidor de catálogo de endereços usando o protocolo MAPI/HTTP.  <br/> |
|[MailStore (POX)](mailstore-pox.md) <br/> |Contém as especificações para conectar um cliente à caixa de correio do usuário usando o protocolo MAPI/HTTP.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor do texto representa uma URL que pode ser usada para acessar um servidor de livro de endereços ou a caixa de correio do usuário de dentro da organização do usuário.
  
## <a name="remarks"></a>Comentários

O **elemento InternalUrl** pode estar presente em uma resposta que tem um elemento [Protocol (POX)](protocol-pox.md) com um valor de atributo **Type** de "mapiHttp". 
  
O **elemento InternalUrl** está disponível para clientes que implementam o protocolo MAPI/HTTP e destino Exchange Online, Exchange Online como parte do Office 365 e versões locais do Exchange a partir da com build 15.00.0847.032 (Exchange Server 2013 SP1). 
  
## <a name="see-also"></a>Confira também



[Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

