---
title: CertPrincipalName (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a24092c9-58be-4008-92c4-68ec5c6c0fa6
description: O elemento CertPrincipalName especifica o nome principal do certificado SSL (Secure Sockets Layer) necessário para se conectar à organização do Microsoft Exchange Server 2007 usando SSL.
ms.openlocfilehash: fb2a1c8577bce41945b669be56f2a94a2c4dca26
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463339"
---
# <a name="certprincipalname-pox"></a>CertPrincipalName (POX)

O elemento **CertPrincipalName** especifica o nome principal do certificado SSL (Secure Sockets Layer) necessário para se conectar à organização do Microsoft Exchange Server 2007 usando SSL. 
  
[Descoberta automática (POX)](autodiscover-pox.md)
  
[Resposta (POX)](response-pox.md)
  
[Conta (POX)](account-pox.md)
  
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente ao computador que está executando o Exchange 2007 que tem a função de servidor de acesso para Cliente instalada.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto especifica o nome principal do certificado SSL necessário para se conectar à organização do Microsoft Exchange usando SSL.
  
## <a name="remarks"></a>Comentários

Se o elemento **CertPrincipalName** não for especificado, o padrão será definido como MSSTD: Server, onde Server é o valor especificado no elemento [Server (POX)](server-pox.md) . Por exemplo, se o servidor for especificado como example.com e **CertPrincipalName** for deixado em branco com o [SSL (POX)](ssl-pox.md) ativado, o valor padrão de **CertPrincipalName** seria msstd:example. com. 
  
Se **nenhum** for especificado, o Windows validará o nome principal do certificado de acordo com as informações encontradas no tópico [nomes de entidade de segurança](https://go.microsoft.com/fwlink/?LinkId=93417) no msdn. 
  
## <a name="see-also"></a>Confira também



[Elementos XML de descoberta automática de POX para o Exchange](pox-autodiscover-xml-elements-for-exchange.md)

