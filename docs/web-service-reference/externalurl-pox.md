---
title: ExternalUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 3b647d88-6feb-40d7-9299-b2ca47b707db
description: O elemento ExternalUrl contém a URL para conectar um cliente ao servidor de catálogo de endereços ou caixa de correio de um usuário de fora da organização do usuário usando o protocolo MAPI/HTTP.
ms.openlocfilehash: 94265051be68ed06d1dab8d46dd4ce29d8694c93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457953"
---
# <a name="externalurl-pox"></a>ExternalUrl (POX)

O elemento **ExternalURL** contém a URL para conectar um cliente ao servidor de catálogo de endereços ou caixa de correio de um usuário de fora da organização do usuário usando o protocolo MAPI/http. 
  
```XML
<ExternalUrl/>
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

O valor de texto representa uma URL que pode ser usada para acessar um servidor de catálogo de endereços ou caixa de correio do usuário de fora da organização do usuário.
  
## <a name="remarks"></a>Comentários

O elemento **ExternalURL** pode estar presente em uma resposta que tem um elemento [Protocol (POX)](protocol-pox.md) com um valor de atributo **Type** de "mapiHttp". 
  
O elemento **ExternalURL** está disponível para clientes que implementam o protocolo MAPI/http e direcionam o Exchange Online, o Exchange Online como parte do Office 365 e as versões locais do Exchange a partir do Build 15.00.0847.032 (exchange server 2013 SP1). 
  
## <a name="see-also"></a>Também consulte



[Elementos XML de descoberta automática de POX para o Exchange](pox-autodiscover-xml-elements-for-exchange.md)

