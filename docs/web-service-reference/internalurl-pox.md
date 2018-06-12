---
title: InternalUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 4649baa9-eec9-426d-952b-361818c25fe0
description: O elemento InternalUrl contém a URL para conectar um cliente para o servidor de catálogo de endereços ou caixa de correio do usuário do dentro da organização do usuário por meio do protocolo MAPI/HTTP.
ms.openlocfilehash: 3823236081961128b31bb2c0f563062897c55814
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823950"
---
# <a name="internalurl-pox"></a>InternalUrl (POX)

O elemento **InternalUrl** contém a URL para conectar um cliente para o servidor de catálogo de endereços ou caixa de correio do usuário do dentro da organização do usuário por meio do protocolo MAPI/HTTP. 
  
```XML
<InternalUrl/>
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
|[AddressBook POX)](addressbook-pox.md) <br/> |Contém as especificações para conectar-se um cliente para o servidor de catálogo de endereços usando o protocolo MAPI/HTTP.  <br/> |
|[Armazenamento_de_email (POX)](mailstore-pox.md) <br/> |Contém as especificações para conectar um cliente de caixa de correio do usuário por meio do protocolo MAPI/HTTP.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto representa uma URL que pode ser usada para acessar um servidor de catálogo de endereços ou caixa de correio do usuário do dentro da organização do usuário.
  
## <a name="remarks"></a>Coment�rios

O elemento **InternalUrl** pode estar presente em uma resposta que tem um elemento de [Protocolo POX ()](protocol-pox.md) com um valor do atributo de **tipo** de "mapiHttp". 
  
O elemento **InternalUrl** é disponível para os clientes que implementam o protocolo MAPI/HTTP e destino Exchange Online, Exchange Online como parte do Office 365, e versões de local do Exchange, começando com compilação 15.00.0847.032 (Exchange Server 2013 SP1) . 
  
## <a name="see-also"></a>Confira também



[Elementos de Autodiscover XML POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

