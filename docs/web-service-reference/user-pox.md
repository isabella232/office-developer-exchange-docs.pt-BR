---
title: Usuário (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 7c42b516-77f6-4aee-99d8-b866d82d793a
description: O elemento do usuário fornece informações específicas do usuário.
ms.openlocfilehash: 3f90ff0cc00170170c7304f2a19fe1d7abd9d1bc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837968"
---
# <a name="user-pox"></a><span data-ttu-id="f92f9-103">Usuário (POX)</span><span class="sxs-lookup"><span data-stu-id="f92f9-103">User (POX)</span></span>

<span data-ttu-id="f92f9-104">O elemento do **usuário** fornece informações específicas do usuário.</span><span class="sxs-lookup"><span data-stu-id="f92f9-104">The **User** element provides user-specific information.</span></span> 
  
[<span data-ttu-id="f92f9-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="f92f9-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="f92f9-106">Resposta POX)</span><span class="sxs-lookup"><span data-stu-id="f92f9-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="f92f9-107">Usuário (POX)</span><span class="sxs-lookup"><span data-stu-id="f92f9-107">User (POX)</span></span>](user-pox.md)
  
```xml
<User>
   <DisplayName/>
   <LegacyDN/>
   <DeploymentId/>
   <AutoDiscoverSMTPAddress/>
</User>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="f92f9-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f92f9-108">Attributes and elements</span></span>

<span data-ttu-id="f92f9-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f92f9-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f92f9-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="f92f9-110">Attributes</span></span>

<span data-ttu-id="f92f9-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f92f9-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f92f9-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f92f9-112">Child elements</span></span>

|<span data-ttu-id="f92f9-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f92f9-113">**Element**</span></span>|<span data-ttu-id="f92f9-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f92f9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f92f9-115">DisplayName (string)</span><span class="sxs-lookup"><span data-stu-id="f92f9-115">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="f92f9-116">Representa o nome para exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="f92f9-116">Represents the user's display name.</span></span>  <br/> |
|[<span data-ttu-id="f92f9-117">LegacyDN (POX)</span><span class="sxs-lookup"><span data-stu-id="f92f9-117">LegacyDN (POX)</span></span>](legacydn-pox.md) <br/> |<span data-ttu-id="f92f9-118">Identifica a caixa de correio de um usuário por nome distinto herdado.</span><span class="sxs-lookup"><span data-stu-id="f92f9-118">Identifies a user's mailbox by legacy distinguished name.</span></span>  <br/> |
|[<span data-ttu-id="f92f9-119">DeploymentId (POX)</span><span class="sxs-lookup"><span data-stu-id="f92f9-119">DeploymentId (POX)</span></span>](deploymentid-pox.md) <br/> |<span data-ttu-id="f92f9-120">Identifica exclusivamente a floresta do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f92f9-120">Uniquely identifies the Exchange forest.</span></span>  <br/> |
|[<span data-ttu-id="f92f9-121">AutoDiscoverSMTPAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="f92f9-121">AutoDiscoverSMTPAddress (POX)</span></span>](autodiscoversmtpaddress-pox.md) <br/> |<span data-ttu-id="f92f9-122">Contém o endereço SMTP do usuário que é usado para o processo de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="f92f9-122">Contains the user's SMTP address that is used for the Autodiscover process.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f92f9-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f92f9-123">Parent elements</span></span>

|<span data-ttu-id="f92f9-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f92f9-124">**Element**</span></span>|<span data-ttu-id="f92f9-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f92f9-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f92f9-126">Resposta POX)</span><span class="sxs-lookup"><span data-stu-id="f92f9-126">Response (POX)</span></span>](response-pox.md) <br/> |<span data-ttu-id="f92f9-127">Contém a resposta do serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="f92f9-127">Contains the response from the Autodiscover service.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f92f9-128">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="f92f9-128">Remarks</span></span>

<span data-ttu-id="f92f9-129">Respostas e solicitações de descoberta automática devem ser codificados UTF-8.</span><span class="sxs-lookup"><span data-stu-id="f92f9-129">Autodiscover requests and responses must be UTF-8 encoded.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="f92f9-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="f92f9-130">See also</span></span>



[<span data-ttu-id="f92f9-131">Elementos de Autodiscover XML POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="f92f9-131">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

