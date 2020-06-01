---
title: PublicFolderServer (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 37ad46ab-7817-4fdd-ad2d-26cb525cd96b
description: O elemento PublicFolderServer contém o FQDN (nome de domínio totalmente qualificado) do servidor de pasta pública para o usuário.
ms.openlocfilehash: 868eab83d05387f570bc033522121f25f09817c4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44433683"
---
# <a name="publicfolderserver-pox"></a>PublicFolderServer (POX)

O elemento **PublicFolderServer** contém o FQDN (nome de domínio totalmente qualificado) do servidor de pasta pública para o usuário. 
  
[Descoberta automática (POX)](autodiscover-pox.md)
  
[Resposta (POX)](response-pox.md)
  
[Conta (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[PublicFolderServer (POX)](publicfolderserver-pox.md)
  
```XML
<PublicFolderServer/>
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

O valor de texto representa o FQDN do servidor de pasta pública para o usuário.
  
## <a name="remarks"></a>Comentários

O elemento **PublicFolderServer** é um elemento filho opcional do elemento **Protocol** . 
  
## <a name="see-also"></a>Também consulte



[Elementos XML de descoberta automática de POX para o Exchange](pox-autodiscover-xml-elements-for-exchange.md)

