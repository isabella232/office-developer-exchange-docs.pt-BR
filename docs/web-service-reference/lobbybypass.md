---
title: LobbyBypass
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: e05ed6eb-00ae-49c8-8341-43f6e0d728ff
description: O elemento LobbyBypass especifica a configuração de reunião online para ignorar o lobby virtual.
ms.openlocfilehash: 41ab9c3f846112d2b679bbb477a0de355a477ffa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540780"
---
# <a name="lobbybypass"></a>LobbyBypass

O **elemento LobbyBypass** especifica a configuração de reunião online para ignorar o lobby virtual. 
  
```XML
<LobbyBypass> Disabled | EnabledForGatewayParticipants </LobbyBypass>
```

 **LobbyBypassType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[OnlineMeetingSettings](onlinemeetingsettings.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do **elemento LobbyBypass** pode ser **Desabilitado** ou **EnabledForGatewayParticipants**. O **valor Disabled** indica que o bypass de lobby está desabilitado, portanto, todos os participantes da reunião devem acessar por meio do lobby virtual. O **valor EnabledForGatewayParticipants** indica que o bypass de lobby está habilitado para participantes do telefone. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  

