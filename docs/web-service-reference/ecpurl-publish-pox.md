---
title: EcpUrl-publish (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: a51189db-f6e5-428d-833d-65a209204a5b
description: O elemento EcpUrl-publish especifica uma URL parcial que pode ser combinada com o valor do elemento EcpUrl (POX) para gerar uma URL que pode ser usada para acessar as configurações de publicação de calendário para um usuário habilitado para email.
ms.openlocfilehash: e48b6fa2075c12947f5f8d97ba44e9fd38dfba8e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544125"
---
# <a name="ecpurl-publish-pox"></a>EcpUrl-publish (POX)

O elemento **EcpUrl-publish** especifica uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que pode ser usada para acessar as configurações de publicação de calendário para um usuário habilitado para email. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[EcpUrl-publish (POX)](ecpurl-publish-pox.md)
  
```XML
<EcpUrl-publish/>
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente ao computador que está executando Microsoft Exchange Server que tem a função de servidor de Acesso para Cliente instalada.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa uma URL parcial que pode ser combinada com o valor do elemento [EcpUrl (POX)](ecpurl-pox.md) para gerar uma URL que pode ser usada para acessar as configurações de publicação de calendário para o usuário. 
  
## <a name="remarks"></a>Comentários

O **elemento EcpUrl-publish** é um elemento filho opcional do **elemento Protocol.** 
  
## <a name="see-also"></a>Confira também



[Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

