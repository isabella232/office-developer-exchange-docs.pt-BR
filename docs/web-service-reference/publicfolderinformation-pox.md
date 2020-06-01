---
title: PublicFolderInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6
description: O elemento PublicFolderInformation contém informações que os clientes podem usar para enviar uma solicitação de descoberta automática para descobrir informações de pasta pública para o usuário.
ms.openlocfilehash: e044a1feddfaeb4eb93c289c617dde9adc66f332
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457715"
---
# <a name="publicfolderinformation-pox"></a><span data-ttu-id="79101-103">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="79101-103">PublicFolderInformation (POX)</span></span>

<span data-ttu-id="79101-104">O elemento **PublicFolderInformation** contém informações que os clientes podem usar para enviar uma solicitação de descoberta automática para descobrir informações de pasta pública para o usuário.</span><span class="sxs-lookup"><span data-stu-id="79101-104">The **PublicFolderInformation** element contains information that clients can use to send an Autodiscover request to discover public folder information for the user.</span></span> 
  
[<span data-ttu-id="79101-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="79101-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="79101-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="79101-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="79101-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="79101-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="79101-108">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="79101-108">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md)
  
```XML
<PublicFolderInformation>
   <SmtpAddress/>
</PublicFolderInformation>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="79101-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="79101-109">Attributes and elements</span></span>

<span data-ttu-id="79101-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="79101-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="79101-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="79101-111">Attributes</span></span>

<span data-ttu-id="79101-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="79101-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="79101-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="79101-113">Child elements</span></span>

|<span data-ttu-id="79101-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="79101-114">**Element**</span></span>|<span data-ttu-id="79101-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="79101-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="79101-116">SmtpAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="79101-116">SmtpAddress (POX)</span></span>](smtpaddress-pox.md) <br/> |<span data-ttu-id="79101-117">Contém o endereço SMTP atribuído ao repositório de mensagens de pasta pública configurado para o usuário.</span><span class="sxs-lookup"><span data-stu-id="79101-117">Contains the SMTP address assigned to the public folder message store configured for the user.</span></span> <span data-ttu-id="79101-118">Esse endereço SMTP pode ser usado no elemento de [EMailAddress (POX)](emailaddress-pox.md) de uma solicitação de descoberta automática para descobrir as configurações de pasta pública.</span><span class="sxs-lookup"><span data-stu-id="79101-118">This SMTP address can be used in the [EMailAddress (POX)](emailaddress-pox.md) element of an Autodiscover request to discover public folder settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="79101-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="79101-119">Parent elements</span></span>

|<span data-ttu-id="79101-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="79101-120">**Element**</span></span>|<span data-ttu-id="79101-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="79101-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="79101-122">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="79101-122">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="79101-123">Especifica as configurações de conta do usuário.</span><span class="sxs-lookup"><span data-stu-id="79101-123">Specifies account settings for the user.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="79101-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="79101-124">Remarks</span></span>

<span data-ttu-id="79101-125">O elemento **PublicFolderInformation** é um elemento filho opcional do elemento **Account** .</span><span class="sxs-lookup"><span data-stu-id="79101-125">The **PublicFolderInformation** element is an optional child element of the **Account** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="79101-126">Também consulte</span><span class="sxs-lookup"><span data-stu-id="79101-126">See also</span></span>



[<span data-ttu-id="79101-127">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="79101-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

