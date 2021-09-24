---
title: EwsPartnerUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 2ebae21c-3efa-4239-9b49-4a3a8871449b
description: O elemento EwsPartnerUrl especifica a URL da melhor instância de ponto de extremidade para Exchange Web Services (EWS) para um usuário habilitado para email.
ms.openlocfilehash: 88ee0abdc5b8db09a938fc5fdba717a166b42399
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524319"
---
# <a name="ewspartnerurl-pox"></a>EwsPartnerUrl (POX)

O **elemento EwsPartnerUrl** especifica a URL da melhor instância de ponto de extremidade para Exchange Web Services (EWS) para um usuário habilitado para email. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[EwsPartnerUrl (POX)](ewspartnerurl-pox.md)
  
```XML
<EwsPartnerUrl/>
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

O valor de texto representa a URL do ponto de extremidade EWS para o usuário.
  
## <a name="remarks"></a>Comentários

O **elemento EwsPartnerUrl** é um elemento filho opcional do **elemento Protocol.** É equivalente ao elemento [EwsUrl (POX).](ewsurl-pox.md) 
  
## <a name="see-also"></a>Confira também



[Elementos XML de Descoberta Automática POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

