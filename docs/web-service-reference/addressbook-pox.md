---
title: AddressBook (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: b2d62fd0-741c-4a41-9762-cc7d0ff01c9c
description: O elemento AddressBook contém as especificações para conectar um cliente ao servidor de catálogo de endereços usando o protocolo MAPI/HTTP.
ms.openlocfilehash: 28de1d41146b082c8b7f82c868fbbed1ce2c483e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546795"
---
# <a name="addressbook-pox"></a>AddressBook (POX)

O **elemento AddressBook** contém as especificações para conectar um cliente ao servidor de catálogo de endereços usando o protocolo MAPI/HTTP. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[AddressBook (POX)](addressbook-pox.md)
  
```XML
<AddressBook>
   <ExternalUrl/>
   <InternalUrl/>
</AddressBook>
```

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ExternalUrl (POX)](externalurl-pox.md) <br/> |Contém a URL que deve ser usada para acessar o livro de endereços de fora da rede da organização usando o protocolo MAPI/HTTP.  <br/> |
|[InternalUrl (POX)](internalurl-pox.md) <br/> |Contém a URL que deve ser usada para acessar o livro de endereços de dentro da rede da organização usando o protocolo MAPI/HTTP.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Protocol (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente ao servidor de Acesso para Cliente.  <br/> |
   
## <a name="remarks"></a>Comentários

O **elemento AddressBook** está presente em uma resposta que tem um elemento [Protocol (POX)](protocol-pox.md) com um **valor de** atributo Type de "mapiHttp". 
  
O elemento **AddressBook** está disponível para clientes que implementam o protocolo MAPI/HTTP e o Exchange Online, Exchange Online como parte do Office 365 e versões locais do Exchange a partir da com build 15.00.0847.032 (Exchange Server 2013 SP1). 
  
## <a name="see-also"></a>Confira também

- [Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

