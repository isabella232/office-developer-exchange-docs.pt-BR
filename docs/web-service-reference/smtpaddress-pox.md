---
title: SmtpAddress (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 984ccd97-c337-47b6-ba42-3405a8b55a71
description: O elemento SmtpAddress contém o endereço SMTP atribuído ao armazenamento de mensagens de pasta pública configurado para o usuário.
ms.openlocfilehash: 48703a11fb056967c6c76073c2e928d5f6efa264
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468639"
---
# <a name="smtpaddress-pox"></a><span data-ttu-id="31ed5-103">SmtpAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="31ed5-103">SmtpAddress (POX)</span></span>

<span data-ttu-id="31ed5-104">O elemento **smtpAddress** contém o endereço SMTP atribuído ao armazenamento de mensagens de pasta pública configurado para o usuário.</span><span class="sxs-lookup"><span data-stu-id="31ed5-104">The **SmtpAddress** element contains the SMTP address assigned to the public folder message store configured for the user.</span></span> 
  
- [<span data-ttu-id="31ed5-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="31ed5-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="31ed5-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="31ed5-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="31ed5-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="31ed5-107">Account (POX)</span></span>](account-pox.md)
  
- [<span data-ttu-id="31ed5-108">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="31ed5-108">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md)
  
- [<span data-ttu-id="31ed5-109">SmtpAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="31ed5-109">SmtpAddress (POX)</span></span>](smtpaddress-pox.md)
  
```XML
<SmtpAddress/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="31ed5-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="31ed5-110">Attributes and elements</span></span>

<span data-ttu-id="31ed5-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="31ed5-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="31ed5-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="31ed5-112">Attributes</span></span>

<span data-ttu-id="31ed5-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="31ed5-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="31ed5-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="31ed5-114">Child elements</span></span>

<span data-ttu-id="31ed5-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="31ed5-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="31ed5-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="31ed5-116">Parent elements</span></span>

|<span data-ttu-id="31ed5-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="31ed5-117">**Element**</span></span>|<span data-ttu-id="31ed5-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="31ed5-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="31ed5-119">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="31ed5-119">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md) <br/> |<span data-ttu-id="31ed5-120">Contém informações que os clientes podem usar para enviar uma solicitação de descoberta automática para descobrir informações de pasta pública para o usuário.</span><span class="sxs-lookup"><span data-stu-id="31ed5-120">Contains information that clients can use to send an Autodiscover request to discover public folder information for the user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="31ed5-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="31ed5-121">Text value</span></span>

<span data-ttu-id="31ed5-122">O valor de texto representa o endereço SMTP atribuído ao armazenamento de pasta pública configurado para o usuário.</span><span class="sxs-lookup"><span data-stu-id="31ed5-122">The text value represents the SMTP address assigned to the public folder store configured for the user.</span></span> <span data-ttu-id="31ed5-123">Esse endereço SMTP pode ser usado no elemento de [EMailAddress (POX)](emailaddress-pox.md) de uma solicitação de descoberta automática para descobrir as configurações de pasta pública.</span><span class="sxs-lookup"><span data-stu-id="31ed5-123">This SMTP address can be used in the [EMailAddress (POX)](emailaddress-pox.md) element of an Autodiscover request to discover public folder settings.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="31ed5-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="31ed5-124">Remarks</span></span>

<span data-ttu-id="31ed5-125">O elemento **smtpAddress** é um elemento filho obrigatório do elemento **PublicFolderInformation** .</span><span class="sxs-lookup"><span data-stu-id="31ed5-125">The **SmtpAddress** element is a required child element of the **PublicFolderInformation** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="31ed5-126">Confira também</span><span class="sxs-lookup"><span data-stu-id="31ed5-126">See also</span></span>

- [<span data-ttu-id="31ed5-127">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="31ed5-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

