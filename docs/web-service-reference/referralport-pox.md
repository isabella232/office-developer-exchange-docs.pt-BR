---
title: ReferralPort (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: cd693f1e-fed4-4eb9-8297-178906f47050
description: O elemento ReferralPort Especifica a porta usada para obter uma referência para um diretório.
ms.openlocfilehash: 5045c0c5a9f15d5a31ac2e884b942e00dfb1f520
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825037"
---
# <a name="referralport-pox"></a>ReferralPort (POX)

O elemento **ReferralPort** Especifica a porta usada para obter uma referência para um diretório. 
  
[Descoberta automática (POX)](autodiscover-pox.md)
  
[Resposta POX)](response-pox.md)
  
[Conta (POX)](account-pox.md)
  
[Protocolo (POX)](protocol-pox.md)
  
[ReferralPort (POX)](referralport-pox.md)
  
```xml
<ReferralPort/>
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
|[Protocolo (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente para o computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto representa a porta usada para acessar o servidor do Exchange.
  
## <a name="remarks"></a>Comentários

O elemento **ReferralPort** é usado apenas quando o elemento de [Tipo POX ()](type-pox.md) é igual a EXCH ou EXPR. 
  
## <a name="see-also"></a>Confira também



[Elementos de Autodiscover XML POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

