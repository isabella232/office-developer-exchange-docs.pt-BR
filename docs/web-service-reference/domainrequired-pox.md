---
title: DomainRequired (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 1f26b691-7331-4c7f-a92b-dfcc66c26963
description: O elemento DomainRequired indica se o domínio é necessário para autenticação.
ms.openlocfilehash: f314b9d27d1b4ee472d249ec49af1a785ff9ac25
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751914"
---
# <a name="domainrequired-pox"></a>DomainRequired (POX)

O elemento **DomainRequired** indica se o domínio é necessário para autenticação. 
  
- [Descoberta automática (POX)](autodiscover-pox.md)  
- [Resposta POX)](response-pox.md) 
- [Conta (POX)](account-pox.md)  
- [Protocolo (POX)](protocol-pox.md)  
- [DomainRequired (POX)](domainrequired-pox.md)
  
```xml
<DomainRequired>on or off</DomainRequired>
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

O valor de texto indica se o domínio é necessário para autenticação. Os valores possíveis são **Ativar** e **Desativar**. Se o valor estiver **ligado**, a solicitação subsequente deve conter o domínio da conta do usuário.
  
## <a name="remarks"></a>Comentários

Se o domínio não for especificado no elemento [LoginName POX ()](loginname-pox.md) ou o elemento **LoginName** não foi especificado, o usuário deve digitar o domínio antes de autenticação terá êxito. 
  
## <a name="see-also"></a>Confira também

- [Elementos de Autodiscover XML POX para Exchange](pox-autodiscover-xml-elements-for-exchange.md)

