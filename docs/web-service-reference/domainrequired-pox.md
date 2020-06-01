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
ms.openlocfilehash: 97d602c40b247f9a6650cc4440b53bf23c18482e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461321"
---
# <a name="domainrequired-pox"></a>DomainRequired (POX)

O elemento **DomainRequired** indica se o domínio é necessário para autenticação. 
  
- [Descoberta automática (POX)](autodiscover-pox.md)  
- [Resposta (POX)](response-pox.md) 
- [Conta (POX)](account-pox.md)  
- [Protocol (POX)](protocol-pox.md)  
- [DomainRequired (POX)](domainrequired-pox.md)
  
```xml
<DomainRequired>on or off</DomainRequired>
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
|[Protocol (POX)](protocol-pox.md) <br/> |Contém as especificações para conectar um cliente ao computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto indica se o domínio é necessário para autenticação. Os valores possíveis estão **ativados** e **desativados**. Se o valor estiver **ativado**, a solicitação subsequente deverá conter o domínio da conta do usuário.
  
## <a name="remarks"></a>Comentários

Se o domínio não for especificado no elemento [LoginName (POX)](loginname-pox.md) ou se o elemento **LoginName** não tiver sido especificado, o usuário deverá inserir o domínio antes que a autenticação seja bem-sucedida. 
  
## <a name="see-also"></a>Também consulte

- [Elementos XML de descoberta automática de POX para o Exchange](pox-autodiscover-xml-elements-for-exchange.md)

