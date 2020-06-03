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
description: O elemento user fornece informações específicas do usuário.
ms.openlocfilehash: 8f53319bcf34595305748adafc9aa1e25283611e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530215"
---
# <a name="user-pox"></a><span data-ttu-id="2910f-103">Usuário (POX)</span><span class="sxs-lookup"><span data-stu-id="2910f-103">User (POX)</span></span>

<span data-ttu-id="2910f-104">O elemento **User** fornece informações específicas do usuário.</span><span class="sxs-lookup"><span data-stu-id="2910f-104">The **User** element provides user-specific information.</span></span> 
  
[<span data-ttu-id="2910f-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="2910f-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="2910f-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="2910f-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="2910f-107">Usuário (POX)</span><span class="sxs-lookup"><span data-stu-id="2910f-107">User (POX)</span></span>](user-pox.md)
  
```xml
<User>
   <DisplayName/>
   <LegacyDN/>
   <DeploymentId/>
   <AutoDiscoverSMTPAddress/>
</User>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="2910f-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="2910f-108">Attributes and elements</span></span>

<span data-ttu-id="2910f-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2910f-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2910f-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="2910f-110">Attributes</span></span>

<span data-ttu-id="2910f-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2910f-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2910f-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2910f-112">Child elements</span></span>

|<span data-ttu-id="2910f-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2910f-113">**Element**</span></span>|<span data-ttu-id="2910f-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2910f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2910f-115">DisplayName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="2910f-115">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="2910f-116">Representa o nome para exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="2910f-116">Represents the user's display name.</span></span>  <br/> |
|[<span data-ttu-id="2910f-117">LegacyDN (POX)</span><span class="sxs-lookup"><span data-stu-id="2910f-117">LegacyDN (POX)</span></span>](legacydn-pox.md) <br/> |<span data-ttu-id="2910f-118">Identifica a caixa de correio de um usuário com o nome diferenciado herdado.</span><span class="sxs-lookup"><span data-stu-id="2910f-118">Identifies a user's mailbox by legacy distinguished name.</span></span>  <br/> |
|[<span data-ttu-id="2910f-119">DeploymentId (POX)</span><span class="sxs-lookup"><span data-stu-id="2910f-119">DeploymentId (POX)</span></span>](deploymentid-pox.md) <br/> |<span data-ttu-id="2910f-120">Identifica exclusivamente a floresta do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2910f-120">Uniquely identifies the Exchange forest.</span></span>  <br/> |
|[<span data-ttu-id="2910f-121">AutoDiscoverSMTPAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="2910f-121">AutoDiscoverSMTPAddress (POX)</span></span>](autodiscoversmtpaddress-pox.md) <br/> |<span data-ttu-id="2910f-122">Contém o endereço SMTP do usuário que é usado para o processo de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="2910f-122">Contains the user's SMTP address that is used for the Autodiscover process.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2910f-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2910f-123">Parent elements</span></span>

|<span data-ttu-id="2910f-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2910f-124">**Element**</span></span>|<span data-ttu-id="2910f-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2910f-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2910f-126">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="2910f-126">Response (POX)</span></span>](response-pox.md) <br/> |<span data-ttu-id="2910f-127">Contém a resposta do serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="2910f-127">Contains the response from the Autodiscover service.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2910f-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="2910f-128">Remarks</span></span>

<span data-ttu-id="2910f-129">As solicitações e respostas de descoberta automática devem ser codificadas em UTF-8.</span><span class="sxs-lookup"><span data-stu-id="2910f-129">Autodiscover requests and responses must be UTF-8 encoded.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="2910f-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="2910f-130">See also</span></span>



[<span data-ttu-id="2910f-131">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="2910f-131">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

