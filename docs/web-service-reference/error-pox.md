---
title: Erro (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 91c63b62-ab68-4c32-a2f7-5a87c188335b
description: O elemento error contém uma resposta de erro de descoberta automática.
ms.openlocfilehash: 1a1a3e83898674e605921cb75371036a8a561a95
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530646"
---
# <a name="error-pox"></a><span data-ttu-id="f0e1f-103">Erro (POX)</span><span class="sxs-lookup"><span data-stu-id="f0e1f-103">Error (POX)</span></span>

<span data-ttu-id="f0e1f-104">O elemento **Error** contém uma resposta de erro de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="f0e1f-104">The **Error** element contains an Autodiscover error response.</span></span> 
  
[<span data-ttu-id="f0e1f-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="f0e1f-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="f0e1f-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="f0e1f-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="f0e1f-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="f0e1f-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="f0e1f-108">Erro (POX)</span><span class="sxs-lookup"><span data-stu-id="f0e1f-108">Error (POX)</span></span>](error-pox.md)
  
```xml
<Error Time="" Id="">
   <ErrorCode/>
   <Message/>
   <DebugData/>
</Error>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="f0e1f-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="f0e1f-109">Attributes and elements</span></span>

<span data-ttu-id="f0e1f-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f0e1f-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f0e1f-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="f0e1f-111">Attributes</span></span>

|<span data-ttu-id="f0e1f-112">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="f0e1f-112">**Attribute**</span></span>|<span data-ttu-id="f0e1f-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f0e1f-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f0e1f-114">Hora</span><span class="sxs-lookup"><span data-stu-id="f0e1f-114">Time</span></span>  <br/> |<span data-ttu-id="f0e1f-115">Representa a hora em que a resposta de erro foi retornada.</span><span class="sxs-lookup"><span data-stu-id="f0e1f-115">Represents the time when the error response was returned.</span></span>  <br/> |
|<span data-ttu-id="f0e1f-116">Id</span><span class="sxs-lookup"><span data-stu-id="f0e1f-116">Id</span></span>  <br/> |<span data-ttu-id="f0e1f-117">Representa um hash do nome do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="f0e1f-117">Represents a hash of the name of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f0e1f-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f0e1f-118">Child elements</span></span>

|<span data-ttu-id="f0e1f-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f0e1f-119">**Element**</span></span>|<span data-ttu-id="f0e1f-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f0e1f-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f0e1f-121">ErrorCode (POX)</span><span class="sxs-lookup"><span data-stu-id="f0e1f-121">ErrorCode (POX)</span></span>](errorcode-pox.md) <br/> |<span data-ttu-id="f0e1f-122">Contém o código de erro para uma resposta de descoberta automática de erro.</span><span class="sxs-lookup"><span data-stu-id="f0e1f-122">Contains the error code for an error Autodiscover response.</span></span>  <br/> |
|[<span data-ttu-id="f0e1f-123">Mensagem (POX)</span><span class="sxs-lookup"><span data-stu-id="f0e1f-123">Message (POX)</span></span>](message-pox.md) <br/> |<span data-ttu-id="f0e1f-124">Contém a mensagem de erro para uma resposta de descoberta automática de erro.</span><span class="sxs-lookup"><span data-stu-id="f0e1f-124">Contains the error message for an error Autodiscover response.</span></span>  <br/> |
|[<span data-ttu-id="f0e1f-125">DebugData (POX)</span><span class="sxs-lookup"><span data-stu-id="f0e1f-125">DebugData (POX)</span></span>](debugdata-pox.md) <br/> |<span data-ttu-id="f0e1f-126">Contém os dados de depuração de uma resposta de descoberta automática de erro.</span><span class="sxs-lookup"><span data-stu-id="f0e1f-126">Contains the debug data for an error Autodiscover response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f0e1f-127">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f0e1f-127">Parent elements</span></span>

|<span data-ttu-id="f0e1f-128">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f0e1f-128">**Element**</span></span>|<span data-ttu-id="f0e1f-129">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f0e1f-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f0e1f-130">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="f0e1f-130">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="f0e1f-131">Contém uma resposta de erro de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="f0e1f-131">Contains an Autodiscover error response.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f0e1f-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="f0e1f-132">See also</span></span>



[<span data-ttu-id="f0e1f-133">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="f0e1f-133">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

