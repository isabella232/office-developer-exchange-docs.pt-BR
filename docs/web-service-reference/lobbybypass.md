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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458093"
---
# <a name="lobbybypass"></a><span data-ttu-id="0c4e3-103">LobbyBypass</span><span class="sxs-lookup"><span data-stu-id="0c4e3-103">LobbyBypass</span></span>

<span data-ttu-id="0c4e3-104">O elemento **LobbyBypass** especifica a configuração de reunião online para ignorar o lobby virtual.</span><span class="sxs-lookup"><span data-stu-id="0c4e3-104">The **LobbyBypass** element specifies the online meeting setting to bypass the virtual lobby.</span></span> 
  
```XML
<LobbyBypass> Disabled | EnabledForGatewayParticipants </LobbyBypass>
```

 <span data-ttu-id="0c4e3-105">**LobbyBypassType**</span><span class="sxs-lookup"><span data-stu-id="0c4e3-105">**LobbyBypassType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0c4e3-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="0c4e3-106">Attributes and elements</span></span>

<span data-ttu-id="0c4e3-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0c4e3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0c4e3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0c4e3-108">Attributes</span></span>

<span data-ttu-id="0c4e3-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0c4e3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0c4e3-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0c4e3-110">Child elements</span></span>

<span data-ttu-id="0c4e3-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0c4e3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0c4e3-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0c4e3-112">Parent elements</span></span>

[<span data-ttu-id="0c4e3-113">OnlineMeetingSettings</span><span class="sxs-lookup"><span data-stu-id="0c4e3-113">OnlineMeetingSettings</span></span>](onlinemeetingsettings.md)
  
## <a name="text-value"></a><span data-ttu-id="0c4e3-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="0c4e3-114">Text value</span></span>

<span data-ttu-id="0c4e3-115">O valor de texto do elemento **LobbyBypass** pode ser **desabilitado** ou **EnabledForGatewayParticipants**.</span><span class="sxs-lookup"><span data-stu-id="0c4e3-115">The text value of the **LobbyBypass** element can be either **Disabled** or **EnabledForGatewayParticipants**.</span></span> <span data-ttu-id="0c4e3-116">O valor **Disabled** indica que o bypass de lobby está desabilitado para que todos os participantes da reunião tenham acesso por meio do lobby virtual.</span><span class="sxs-lookup"><span data-stu-id="0c4e3-116">The **Disabled** value indicates that the lobby bypass is disabled so all meeting attendees must access through the virtual lobby.</span></span> <span data-ttu-id="0c4e3-117">O valor **EnabledForGatewayParticipants** indica que o bypass de lobby está habilitado para participantes do telefone.</span><span class="sxs-lookup"><span data-stu-id="0c4e3-117">The **EnabledForGatewayParticipants** value indicates that the lobby bypass is enabled for telephone participants.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="0c4e3-118">Comentários</span><span class="sxs-lookup"><span data-stu-id="0c4e3-118">Remarks</span></span>

<span data-ttu-id="0c4e3-119">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0c4e3-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0c4e3-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0c4e3-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  

