---
title: DeploymentId (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: b879c134-307e-4645-bb53-55d8ba4fad9c
description: O elemento DeploymentId identifica exclusivamente a floresta do Microsoft Exchange Server 2007.
ms.openlocfilehash: 4986a3404763e88fb3e84d52a5d30d54c810f93a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467918"
---
# <a name="deploymentid-pox"></a><span data-ttu-id="eeb84-103">DeploymentId (POX)</span><span class="sxs-lookup"><span data-stu-id="eeb84-103">DeploymentId (POX)</span></span>

<span data-ttu-id="eeb84-104">O elemento **DeploymentId** identifica exclusivamente a floresta do Microsoft Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="eeb84-104">The **DeploymentId** element uniquely identifies the Microsoft Exchange Server 2007 forest.</span></span> 
  
- [<span data-ttu-id="eeb84-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="eeb84-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)  
- [<span data-ttu-id="eeb84-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="eeb84-106">Response (POX)</span></span>](response-pox.md) 
- [<span data-ttu-id="eeb84-107">Usuário (POX)</span><span class="sxs-lookup"><span data-stu-id="eeb84-107">User (POX)</span></span>](user-pox.md)  
- [<span data-ttu-id="eeb84-108">DeploymentId (POX)</span><span class="sxs-lookup"><span data-stu-id="eeb84-108">DeploymentId (POX)</span></span>](deploymentid-pox.md)
  
```xml
<DeploymentId/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="eeb84-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="eeb84-109">Attributes and elements</span></span>

<span data-ttu-id="eeb84-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="eeb84-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eeb84-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="eeb84-111">Attributes</span></span>

<span data-ttu-id="eeb84-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eeb84-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eeb84-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="eeb84-113">Child elements</span></span>

<span data-ttu-id="eeb84-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="eeb84-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="eeb84-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="eeb84-115">Parent elements</span></span>

|<span data-ttu-id="eeb84-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="eeb84-116">**Element**</span></span>|<span data-ttu-id="eeb84-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="eeb84-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eeb84-118">Usuário (POX)</span><span class="sxs-lookup"><span data-stu-id="eeb84-118">User (POX)</span></span>](user-pox.md) <br/> |<span data-ttu-id="eeb84-119">Fornece informações específicas do usuário.</span><span class="sxs-lookup"><span data-stu-id="eeb84-119">Provides user-specific information.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="eeb84-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="eeb84-120">Text value</span></span>

<span data-ttu-id="eeb84-121">O valor de texto identifica exclusivamente a floresta do Exchange 2007 no formato GUID.</span><span class="sxs-lookup"><span data-stu-id="eeb84-121">The text value uniquely identifies the Exchange 2007 forest in GUID format.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="eeb84-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="eeb84-122">Remarks</span></span>

<span data-ttu-id="eeb84-123">Se você desinstalar e depois reinstalar o Exchange 2007 e usar o mesmo nome de servidor, o valor **DeploymentId** será alterado.</span><span class="sxs-lookup"><span data-stu-id="eeb84-123">If you uninstall and then reinstall Exchange 2007 and you use the same server name, the **DeploymentId** value changes.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="eeb84-124">Confira também</span><span class="sxs-lookup"><span data-stu-id="eeb84-124">See also</span></span>

- [<span data-ttu-id="eeb84-125">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="eeb84-125">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

