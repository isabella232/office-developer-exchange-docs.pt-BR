---
title: LobbyBypass
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e05ed6eb-00ae-49c8-8341-43f6e0d728ff
description: O elemento LobbyBypass especifica a configuração de reunião online para ignorar o lobby virtual.
ms.openlocfilehash: 6940428c944b9d4d64acc6dbbf3993576e1932eb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458093"
---
# <a name="lobbybypass"></a>LobbyBypass

O elemento **LobbyBypass** especifica a configuração de reunião online para ignorar o lobby virtual. 
  
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

O valor de texto do elemento **LobbyBypass** pode ser **desabilitado** ou **EnabledForGatewayParticipants**. O valor **Disabled** indica que o bypass de lobby está desabilitado para que todos os participantes da reunião tenham acesso por meio do lobby virtual. O valor **EnabledForGatewayParticipants** indica que o bypass de lobby está habilitado para participantes do telefone. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  

