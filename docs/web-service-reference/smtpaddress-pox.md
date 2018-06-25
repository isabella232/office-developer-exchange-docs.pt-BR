---
title: SmtpAddress POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 984ccd97-c337-47b6-ba42-3405a8b55a71
description: O elemento de SmtpAddress contém o endereço de SMTP atribuído para o armazenamento de pasta pública de mensagens configurado para o usuário.
ms.openlocfilehash: 43ebb328e31cdec11412e80b743d4d4393b7960a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825507"
---
# <a name="smtpaddress-pox"></a><span data-ttu-id="391a8-103">SmtpAddress POX)</span><span class="sxs-lookup"><span data-stu-id="391a8-103">SmtpAddress (POX)</span></span>

<span data-ttu-id="391a8-104">O elemento de **SmtpAddress** contém o endereço de SMTP atribuído para o armazenamento de pasta pública de mensagens configurado para o usuário.</span><span class="sxs-lookup"><span data-stu-id="391a8-104">The **SmtpAddress** element contains the SMTP address assigned to the public folder message store configured for the user.</span></span> 
  
- [<span data-ttu-id="391a8-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="391a8-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="391a8-106">Resposta POX)</span><span class="sxs-lookup"><span data-stu-id="391a8-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="391a8-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="391a8-107">Account (POX)</span></span>](account-pox.md)
  
- [<span data-ttu-id="391a8-108">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="391a8-108">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md)
  
- [<span data-ttu-id="391a8-109">SmtpAddress POX)</span><span class="sxs-lookup"><span data-stu-id="391a8-109">SmtpAddress (POX)</span></span>](smtpaddress-pox.md)
  
```XML
<SmtpAddress/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="391a8-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="391a8-110">Attributes and elements</span></span>

<span data-ttu-id="391a8-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="391a8-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="391a8-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="391a8-112">Attributes</span></span>

<span data-ttu-id="391a8-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="391a8-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="391a8-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="391a8-114">Child elements</span></span>

<span data-ttu-id="391a8-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="391a8-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="391a8-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="391a8-116">Parent elements</span></span>

|<span data-ttu-id="391a8-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="391a8-117">**Element**</span></span>|<span data-ttu-id="391a8-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="391a8-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="391a8-119">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="391a8-119">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md) <br/> |<span data-ttu-id="391a8-120">Contém informações que os clientes podem usar para enviar uma solicitação de descoberta automática para descobrir informações de pasta pública para o usuário.</span><span class="sxs-lookup"><span data-stu-id="391a8-120">Contains information that clients can use to send an Autodiscover request to discover public folder information for the user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="391a8-121">Text value</span><span class="sxs-lookup"><span data-stu-id="391a8-121">Text value</span></span>

<span data-ttu-id="391a8-122">O valor de texto representa o endereço SMTP atribuído ao repositório de pasta pública configurado para o usuário.</span><span class="sxs-lookup"><span data-stu-id="391a8-122">The text value represents the SMTP address assigned to the public folder store configured for the user.</span></span> <span data-ttu-id="391a8-123">Esse endereço SMTP pode ser usado no elemento [EMailAddress POX ()](emailaddress-pox.md) de uma solicitação de descoberta automática para descobrir as configurações de pasta pública.</span><span class="sxs-lookup"><span data-stu-id="391a8-123">This SMTP address can be used in the [EMailAddress (POX)](emailaddress-pox.md) element of an Autodiscover request to discover public folder settings.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="391a8-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="391a8-124">Remarks</span></span>

<span data-ttu-id="391a8-125">O **SmtpAddress** é um elemento necessário filho do elemento **PublicFolderInformation** .</span><span class="sxs-lookup"><span data-stu-id="391a8-125">The **SmtpAddress** element is a required child element of the **PublicFolderInformation** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="391a8-126">Confira também</span><span class="sxs-lookup"><span data-stu-id="391a8-126">See also</span></span>

- [<span data-ttu-id="391a8-127">Elementos de Autodiscover XML POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="391a8-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

