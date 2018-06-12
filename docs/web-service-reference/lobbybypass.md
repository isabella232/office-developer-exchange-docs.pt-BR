---
title: LobbyBypass
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e05ed6eb-00ae-49c8-8341-43f6e0d728ff
description: O elemento LobbyBypass Especifica a definição como ignoram o lobby virtual de reunião online.
ms.openlocfilehash: 9ecc920acd9e1aea3476ad1194d6c7d0529b21c7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824246"
---
# <a name="lobbybypass"></a><span data-ttu-id="0d1dc-103">LobbyBypass</span><span class="sxs-lookup"><span data-stu-id="0d1dc-103">LobbyBypass</span></span>

<span data-ttu-id="0d1dc-104">O elemento **LobbyBypass** Especifica a definição como ignoram o lobby virtual de reunião online.</span><span class="sxs-lookup"><span data-stu-id="0d1dc-104">The **LobbyBypass** element specifies the online meeting setting to bypass the virtual lobby.</span></span> 
  
```XML
<LobbyBypass> Disabled | EnabledForGatewayParticipants </LobbyBypass>
```

 <span data-ttu-id="0d1dc-105">**LobbyBypassType**</span><span class="sxs-lookup"><span data-stu-id="0d1dc-105">**LobbyBypassType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0d1dc-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="0d1dc-106">Attributes and elements</span></span>

<span data-ttu-id="0d1dc-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0d1dc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0d1dc-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0d1dc-108">Attributes</span></span>

<span data-ttu-id="0d1dc-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0d1dc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0d1dc-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0d1dc-110">Child elements</span></span>

<span data-ttu-id="0d1dc-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0d1dc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0d1dc-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0d1dc-112">Parent elements</span></span>

[<span data-ttu-id="0d1dc-113">OnlineMeetingSettings</span><span class="sxs-lookup"><span data-stu-id="0d1dc-113">OnlineMeetingSettings</span></span>](onlinemeetingsettings.md)
  
## <a name="text-value"></a><span data-ttu-id="0d1dc-114">Text value</span><span class="sxs-lookup"><span data-stu-id="0d1dc-114">Text value</span></span>

<span data-ttu-id="0d1dc-115">O valor de texto do elemento **LobbyBypass** pode ser **desativado** ou **EnabledForGatewayParticipants**.</span><span class="sxs-lookup"><span data-stu-id="0d1dc-115">The text value of the **LobbyBypass** element can be either **Disabled** or **EnabledForGatewayParticipants**.</span></span> <span data-ttu-id="0d1dc-116">O valor de **desabilitada** indica que o desvio de lobby está desativado para que todos os participantes da reunião devem acessar pelo lobby virtual.</span><span class="sxs-lookup"><span data-stu-id="0d1dc-116">The **Disabled** value indicates that the lobby bypass is disabled so all meeting attendees must access through the virtual lobby.</span></span> <span data-ttu-id="0d1dc-117">O valor de **EnabledForGatewayParticipants** indica que o desvio de lobby está habilitado para participantes de telefone.</span><span class="sxs-lookup"><span data-stu-id="0d1dc-117">The **EnabledForGatewayParticipants** value indicates that the lobby bypass is enabled for telephone participants.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="0d1dc-118">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="0d1dc-118">Remarks</span></span>

<span data-ttu-id="0d1dc-119">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0d1dc-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0d1dc-120">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0d1dc-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  

