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
description: O elemento CertPrincipalName Especifica o nome principal do certificado Secure Sockets Layer (SSL) que é necessária para conectar-se para a organização do Microsoft Exchange Server 2007 usando SSL.
ms.openlocfilehash: d2766b16a3e8a1bcd013de332d9c07f709fcf949
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751386"
---
# <a name="certprincipalname-pox"></a>CertPrincipalName (POX)

O elemento **CertPrincipalName** Especifica o nome principal do certificado Secure Sockets Layer (SSL) que é necessária para conectar-se para a organização do Microsoft Exchange Server 2007 usando SSL. 
  
[Descoberta automática (POX)](autodiscover-pox.md)
  
[Resposta POX)](response-pox.md)
  
[Conta (POX)](account-pox.md)
  
[Protocolo (POX)](protocol-pox.md)
  
[CertPrincipalName (POX)](certprincipalname-pox.md)
  
```xml
<CertPrincipalName>none or servername</CertPrinicpalName>
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
|[Protocolo (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente para o computador que está executando o Exchange 2007 que possui a função de servidor acesso para cliente instalada.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto Especifica o nome principal do certificado SSL que é necessária para conectar-se à organização do Microsoft Exchange usando SSL.
  
## <a name="remarks"></a>Comentários

Se o elemento **CertPrincipalName** não for especificado, o padrão é definido como msstd:SERVER, em que servidor é o valor especificado no elemento [Server POX ()](server-pox.md) . Por exemplo, se o servidor é especificado como example.com e **CertPrincipalName** for deixado em branco com [SSL (POX)](ssl-pox.md) ativado, o valor padrão de **CertPrincipalName** seria msstd:example.com. 
  
Se **Nenhum** for especificado, o Windows validará o nome principal do certificado de acordo com a informação encontrada no tópico [Nomes de entidade](http://go.microsoft.com/fwlink/?LinkId=93417) no MSDN. 
  
## <a name="see-also"></a>Confira também



[Elementos de Autodiscover XML POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

