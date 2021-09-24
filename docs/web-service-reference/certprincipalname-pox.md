---
title: CertPrincipalName (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: a24092c9-58be-4008-92c4-68ec5c6c0fa6
description: O elemento CertPrincipalName especifica o nome principal do certificado SSL (Secure Sockets Layer) necessário para se conectar à organização Microsoft Exchange Server 2007 usando sSL.
ms.openlocfilehash: 69ee49cdad09032c269ffbbcc918044daf61cb9b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523248"
---
# <a name="certprincipalname-pox"></a>CertPrincipalName (POX)

O **elemento CertPrincipalName** especifica o nome principal do certificado SSL (Secure Sockets Layer) necessário para se conectar à organização Microsoft Exchange Server 2007 usando SSL. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[CertPrincipalName (POX)](certprincipalname-pox.md)
  
```xml
<CertPrincipalName>none or servername</CertPrinicpalName>
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente ao computador que está executando Exchange 2007 que tem a função de servidor de Acesso para Cliente instalada.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto especifica o nome principal do certificado SSL que é necessário para se conectar à organização do microsoft Exchange usando SSL.
  
## <a name="remarks"></a>Comentários

Se o **elemento CertPrincipalName** não for especificado, o padrão será definido como msstd:SERVER, onde SERVER é o valor especificado no elemento [Server (POX).](server-pox.md) Por exemplo, se SERVER for especificado como example.com **e CertPrincipalName** for deixado em branco com [SSL (POX)](ssl-pox.md) ligado, o valor padrão de **CertPrincipalName** seria msstd:example.com. 
  
Se **nenhum** for especificado, Windows validará o nome principal do certificado de acordo com as informações encontradas no tópico [Nomes Principais](https://go.microsoft.com/fwlink/?LinkId=93417) no MSDN. 
  
## <a name="see-also"></a>Confira também



[Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

