---
title: EmwsUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: cad0fa91-8d75-4dde-a484-518c837ae063
description: O elemento EmwsUrl especifica a URL da melhor instância de ponto de extremidade para os serviços Web do Exchange (EWS) para um usuário habilitado para email.
ms.openlocfilehash: 19e1078ae8d08513e85d75d87e960a910986f727
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530667"
---
# <a name="emwsurl-pox"></a>EmwsUrl (POX)

O elemento **EmwsUrl** especifica a URL da melhor instância de ponto de extremidade para os serviços Web do Exchange (EWS) para um usuário habilitado para email. 
  
- [Descoberta automática (POX)](autodiscover-pox.md) 
- [Resposta (POX)](response-pox.md) 
- [Conta (POX)](account-pox.md) 
- [Protocol (POX)](protocol-pox.md) 
- [EmwsUrl (POX)](emwsurl-pox.md)
  
```XML
<EmwsUrl/>
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

O valor de texto representa a URL do ponto de extremidade do EWS para o usuário. É equivalente ao elemento [EwsUrl (POX)](ewsurl-pox.md) . 
  
## <a name="remarks"></a>Comentários

O elemento **EmwsUrl** é um elemento filho opcional do elemento **Protocol** . 
  
## <a name="see-also"></a>Confira também

- [Elementos XML de descoberta automática de POX para o Exchange](pox-autodiscover-xml-elements-for-exchange.md)

