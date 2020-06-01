---
title: EcpUrl-aggr (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 0e7879e3-9b8f-4f23-8291-bacec0e479c0
description: O elemento EcpUrl-aggr especifica uma URL parcial que pode ser combinada com o valor do elemento EcpUrl (POX) para gerar uma URL que possa ser usada para acessar as configurações de agregação de email para um usuário habilitado para email.
ms.openlocfilehash: 26e855900154fb965eae9ba90a373b88e85c2ad3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457281"
---
# <a name="ecpurl-aggr-pox"></a>EcpUrl-aggr (POX)

O elemento **EcpUrl-aggr** especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que possa ser usada para acessar as configurações de agregação de email para um usuário habilitado para email. 
  
[Descoberta automática (POX)](autodiscover-pox.md)
  
[Resposta (POX)](response-pox.md)
  
[Conta (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[EcpUrl-aggr (POX)](ecpurl-aggr-pox.md)
  
```XML
<EcpUrl-aggr/>
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente ao computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que possa ser usada para acessar as configurações de agregação de email para o usuário. 
  
## <a name="remarks"></a>Comentários

O elemento **EcpUrl-aggr** é um elemento filho opcional do elemento **Protocol** . 
  
## <a name="see-also"></a>Também consulte



[Elementos XML de descoberta automática de POX para o Exchange](pox-autodiscover-xml-elements-for-exchange.md)

