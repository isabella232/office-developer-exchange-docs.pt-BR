---
title: AddressBook POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: b2d62fd0-741c-4a41-9762-cc7d0ff01c9c
description: O elemento de AddressBook contém as especificações para conectar-se um cliente para o servidor de catálogo de endereços usando o protocolo MAPI/HTTP.
ms.openlocfilehash: c30f0ee7c36de7e63157d07d003a11187d661fd7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751063"
---
# <a name="addressbook-pox"></a>AddressBook POX)

O elemento de **AddressBook** contém as especificações para conectar-se um cliente para o servidor de catálogo de endereços usando o protocolo MAPI/HTTP. 
  
[Descoberta automática (POX)](autodiscover-pox.md)
  
[Resposta POX)](response-pox.md)
  
[Conta (POX)](account-pox.md)
  
[Protocolo (POX)](protocol-pox.md)
  
[AddressBook POX)](addressbook-pox.md)
  
```XML
<AddressBook>
   <ExternalUrl/>
   <InternalUrl/>
</AddressBook>
```

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ExternalUrl POX)](externalurl-pox.md) <br/> |Contém a URL que deve ser usada para acessar o catálogo de endereços de fora da rede da organização por meio do protocolo MAPI/HTTP.  <br/> |
|[InternalUrl (POX)](internalurl-pox.md) <br/> |Contém a URL que deve ser usada para acessar o catálogo de endereços de dentro da rede da organização por meio do protocolo MAPI/HTTP.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Protocolo (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente para o servidor de acesso para cliente.  <br/> |
   
## <a name="remarks"></a>Comentários

O elemento **AddressBook** está presente em uma resposta que tem um elemento de [Protocolo POX ()](protocol-pox.md) com um valor do atributo de **tipo** de "mapiHttp". 
  
O elemento **AddressBook** está disponível para clientes que implementam o protocolo MAPI/HTTP e destino Exchange Online, Exchange Online como parte do Office 365, e versões de local do Exchange, começando com o build 15.00.0847.032 (Exchange Server 2013 SP1) . 
  
## <a name="see-also"></a>Confira também

- [Elementos de Autodiscover XML POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

