---
title: ExpandGroupMembership
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8989e96b-8fa1-4858-93b2-2cbdb30b9ca9
description: O elemento ExpandGroupMembership indica se expandir a associação do grupo retornado de uma solicitação de GetSearchableMailboxes.
ms.openlocfilehash: 11bfcf6893a147c726c94df77f7d9a9dfbaa773e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752143"
---
# <a name="expandgroupmembership"></a><span data-ttu-id="a5fcb-103">ExpandGroupMembership</span><span class="sxs-lookup"><span data-stu-id="a5fcb-103">ExpandGroupMembership</span></span>

<span data-ttu-id="a5fcb-104">O elemento **ExpandGroupMembership** indica se expandir a associação do grupo retornado de uma solicitação de **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="a5fcb-104">The **ExpandGroupMembership** element indicates whether to expand the membership of the group returned from a **GetSearchableMailboxes** request.</span></span> 
  
```XML
<ExpandGroupMembership>true | false</ExpandGroupMembership>
```

 <span data-ttu-id="a5fcb-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="a5fcb-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a5fcb-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a5fcb-106">Attributes and elements</span></span>

<span data-ttu-id="a5fcb-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a5fcb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a5fcb-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a5fcb-108">Attributes</span></span>

<span data-ttu-id="a5fcb-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a5fcb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a5fcb-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a5fcb-110">Child elements</span></span>

<span data-ttu-id="a5fcb-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a5fcb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a5fcb-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a5fcb-112">Parent elements</span></span>

<span data-ttu-id="a5fcb-113">[GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration.md) | [GetSearchableMailboxes](getsearchablemailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="a5fcb-113">[GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration.md) | [GetSearchableMailboxes](getsearchablemailboxes.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="a5fcb-114">Text value</span><span class="sxs-lookup"><span data-stu-id="a5fcb-114">Text value</span></span>

<span data-ttu-id="a5fcb-115">Um valor de texto de **true** para o elemento **ExpandGroupElement** indica que a associação ao grupo for expandida.</span><span class="sxs-lookup"><span data-stu-id="a5fcb-115">A text value of **true** for the **ExpandGroupElement** element indicates that group membership is expanded.</span></span> <span data-ttu-id="a5fcb-116">Um valor **false** indica que a associação de grupo não é expandida para mostrar os membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="a5fcb-116">A value of **false** indicates that the group membership is not expanded to show the members of the group.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a5fcb-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="a5fcb-117">Remarks</span></span>

<span data-ttu-id="a5fcb-118">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a5fcb-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a5fcb-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a5fcb-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a5fcb-120">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a5fcb-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a5fcb-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="a5fcb-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a5fcb-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a5fcb-122">Schema name</span></span>  <br/> |<span data-ttu-id="a5fcb-123">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="a5fcb-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a5fcb-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a5fcb-124">Validation file</span></span>  <br/> |<span data-ttu-id="a5fcb-125">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a5fcb-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a5fcb-126">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="a5fcb-126">Can be empty</span></span>  <br/> |<span data-ttu-id="a5fcb-127">false</span><span class="sxs-lookup"><span data-stu-id="a5fcb-127">false</span></span>  <br/> |
   

