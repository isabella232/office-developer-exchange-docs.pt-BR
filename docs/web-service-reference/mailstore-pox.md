---
title: Armazenamento_de_email (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: af338f99-9e62-4124-9bff-8d7cc2008161
description: O elemento Armazenamento_de_email contém as especificações para conectar um cliente de caixa de correio do usuário por meio do protocolo MAPI/HTTP.
ms.openlocfilehash: 4c82c7b61752cf7d91287a3968f6c642f4943855
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824301"
---
# <a name="mailstore-pox"></a>Armazenamento_de_email (POX)

O elemento **Armazenamento_de_email** contém as especificações para conectar um cliente de caixa de correio do usuário por meio do protocolo MAPI/HTTP. 
  
[Descoberta automática (POX)](autodiscover-pox.md)
  
[Resposta POX)](response-pox.md)
  
[Conta (POX)](account-pox.md)
  
[Protocolo (POX)](protocol-pox.md)
  
[Armazenamento_de_email (POX)](mailstore-pox.md)
  
```XML
<MailStore>
   <ExternalUrl/>
   <InternalUrl/>
</MailStore>
```

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ExternalUrl POX)](externalurl-pox.md) <br/> |Contém a URL que deve ser usada para acessar a caixa de correio do usuário de fora da rede da organização por meio do protocolo MAPI/HTTP.  <br/> |
|[InternalUrl (POX)](internalurl-pox.md) <br/> |Contém a URL que deve ser usada para acessar a caixa de correio do usuário do dentro da rede da organização por meio do protocolo MAPI/HTTP.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Protocolo (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente para o servidor de acesso para cliente.  <br/> |
   
## <a name="remarks"></a>Coment�rios

O elemento **Armazenamento_de_email** está presente em uma resposta que tem um elemento de [Protocolo POX ()](protocol-pox.md) com um valor do atributo de **tipo** de "mapiHttp". 
  
O elemento **Armazenamento_de_email** está disponível para os clientes que implementam o protocolo MAPI/HTTP e destino Exchange Online, Exchange Online como parte do Office 365, e versões locais do Exchange, começando com o build 15.00.0847.032 (Exchange Server 2013 SP1). 
  
## <a name="see-also"></a>Confira também



[Elementos de Autodiscover XML POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

