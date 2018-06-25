---
title: PublicFolderInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6
description: O elemento PublicFolderInformation contém informações que os clientes podem usar para enviar uma solicitação de descoberta automática para descobrir informações de pasta pública para o usuário.
ms.openlocfilehash: bb4432a664024c3d1ccb17826948cfe7a1b58cdf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824927"
---
# <a name="publicfolderinformation-pox"></a><span data-ttu-id="d204e-103">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="d204e-103">PublicFolderInformation (POX)</span></span>

<span data-ttu-id="d204e-104">O elemento **PublicFolderInformation** contém informações que os clientes podem usar para enviar uma solicitação de descoberta automática para descobrir informações de pasta pública para o usuário.</span><span class="sxs-lookup"><span data-stu-id="d204e-104">The **PublicFolderInformation** element contains information that clients can use to send an Autodiscover request to discover public folder information for the user.</span></span> 
  
[<span data-ttu-id="d204e-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="d204e-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="d204e-106">Resposta POX)</span><span class="sxs-lookup"><span data-stu-id="d204e-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="d204e-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="d204e-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="d204e-108">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="d204e-108">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md)
  
```XML
<PublicFolderInformation>
   <SmtpAddress/>
</PublicFolderInformation>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="d204e-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d204e-109">Attributes and elements</span></span>

<span data-ttu-id="d204e-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d204e-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d204e-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="d204e-111">Attributes</span></span>

<span data-ttu-id="d204e-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d204e-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d204e-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d204e-113">Child elements</span></span>

|<span data-ttu-id="d204e-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d204e-114">**Element**</span></span>|<span data-ttu-id="d204e-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d204e-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d204e-116">SmtpAddress POX)</span><span class="sxs-lookup"><span data-stu-id="d204e-116">SmtpAddress (POX)</span></span>](smtpaddress-pox.md) <br/> |<span data-ttu-id="d204e-117">Contém o endereço de SMTP atribuído para o armazenamento de pasta pública de mensagens configurado para o usuário.</span><span class="sxs-lookup"><span data-stu-id="d204e-117">Contains the SMTP address assigned to the public folder message store configured for the user.</span></span> <span data-ttu-id="d204e-118">Esse endereço SMTP pode ser usado no elemento [EMailAddress POX ()](emailaddress-pox.md) de uma solicitação de descoberta automática para descobrir as configurações de pasta pública.</span><span class="sxs-lookup"><span data-stu-id="d204e-118">This SMTP address can be used in the [EMailAddress (POX)](emailaddress-pox.md) element of an Autodiscover request to discover public folder settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d204e-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d204e-119">Parent elements</span></span>

|<span data-ttu-id="d204e-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d204e-120">**Element**</span></span>|<span data-ttu-id="d204e-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d204e-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d204e-122">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="d204e-122">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="d204e-123">Especifica as configurações da conta do usuário.</span><span class="sxs-lookup"><span data-stu-id="d204e-123">Specifies account settings for the user.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d204e-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="d204e-124">Remarks</span></span>

<span data-ttu-id="d204e-125">O **PublicFolderInformation** é um elemento filho opcionais do elemento de **conta** .</span><span class="sxs-lookup"><span data-stu-id="d204e-125">The **PublicFolderInformation** element is an optional child element of the **Account** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="d204e-126">Confira também</span><span class="sxs-lookup"><span data-stu-id="d204e-126">See also</span></span>



[<span data-ttu-id="d204e-127">Elementos de Autodiscover XML POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="d204e-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

