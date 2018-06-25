---
title: ExternalUrl POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 3b647d88-6feb-40d7-9299-b2ca47b707db
description: O elemento ExternalUrl contém a URL para conectar um cliente para o servidor de catálogo de endereços ou caixa de correio do usuário de fora da organização do usuário por meio do protocolo MAPI/HTTP.
ms.openlocfilehash: 603e2109e7b3c98acdd4cbc13df81ed9717630ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752222"
---
# <a name="externalurl-pox"></a>ExternalUrl POX)

O elemento **ExternalUrl** contém a URL para conectar um cliente para o servidor de catálogo de endereços ou caixa de correio do usuário de fora da organização do usuário por meio do protocolo MAPI/HTTP. 
  
```XML
<ExternalUrl/>
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

O valor de texto representa uma URL que pode ser usada para acessar um servidor de catálogo de endereços ou caixa de correio do usuário de fora da organização do usuário.
  
## <a name="remarks"></a>Comentários

O elemento **ExternalUrl** pode estar presente em uma resposta que tem um elemento de [Protocolo POX ()](protocol-pox.md) com um valor do atributo de **tipo** de "mapiHttp". 
  
O elemento **ExternalUrl** está disponível para clientes que implementam o protocolo MAPI/HTTP e destino Exchange Online, Exchange Online como parte do Office 365, e versões de local do Exchange, começando com o build 15.00.0847.032 (Exchange Server 2013 SP1) . 
  
## <a name="see-also"></a>Confira também



[Elementos de Autodiscover XML POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

