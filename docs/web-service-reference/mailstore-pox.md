---
title: MailStore (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: af338f99-9e62-4124-9bff-8d7cc2008161
description: O elemento MailStore contém as especificações para conectar um cliente à caixa de correio do usuário usando o protocolo MAPI/HTTP.
ms.openlocfilehash: 635228fcfeb3ad791c845050b82666a6e060b229
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459788"
---
# <a name="mailstore-pox"></a><span data-ttu-id="caa15-103">MailStore (POX)</span><span class="sxs-lookup"><span data-stu-id="caa15-103">MailStore (POX)</span></span>

<span data-ttu-id="caa15-104">O elemento **MailStore** contém as especificações para conectar um cliente à caixa de correio do usuário usando o protocolo MAPI/http.</span><span class="sxs-lookup"><span data-stu-id="caa15-104">The **MailStore** element contains the specifications for connecting a client to the user's mailbox by using the MAPI/HTTP protocol.</span></span> 
  
[<span data-ttu-id="caa15-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="caa15-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="caa15-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="caa15-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="caa15-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="caa15-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="caa15-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="caa15-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="caa15-109">MailStore (POX)</span><span class="sxs-lookup"><span data-stu-id="caa15-109">MailStore (POX)</span></span>](mailstore-pox.md)
  
```XML
<MailStore>
   <ExternalUrl/>
   <InternalUrl/>
</MailStore>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="caa15-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="caa15-110">Attributes and elements</span></span>

<span data-ttu-id="caa15-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="caa15-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="caa15-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="caa15-112">Attributes</span></span>

<span data-ttu-id="caa15-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="caa15-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="caa15-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="caa15-114">Child elements</span></span>

|<span data-ttu-id="caa15-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="caa15-115">**Element**</span></span>|<span data-ttu-id="caa15-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="caa15-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="caa15-117">ExternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="caa15-117">ExternalUrl (POX)</span></span>](externalurl-pox.md) <br/> |<span data-ttu-id="caa15-118">Contém a URL que deve ser usada para acessar a caixa de correio do usuário de fora da rede da organização por meio do protocolo MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="caa15-118">Contains the URL that should be used to access the user's mailbox from outside the organization's network by means of the MAPI/HTTP protocol.</span></span>  <br/> |
|[<span data-ttu-id="caa15-119">InternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="caa15-119">InternalUrl (POX)</span></span>](internalurl-pox.md) <br/> |<span data-ttu-id="caa15-120">Contém a URL que deve ser usada para acessar a caixa de correio do usuário de dentro da rede da organização por meio do protocolo MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="caa15-120">Contains the URL that should be used to access the user's mailbox from inside the organization's network by means of the MAPI/HTTP protocol.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="caa15-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="caa15-121">Parent elements</span></span>

|<span data-ttu-id="caa15-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="caa15-122">**Element**</span></span>|<span data-ttu-id="caa15-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="caa15-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="caa15-124">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="caa15-124">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="caa15-125">Contém as especificações para conectar um cliente ao servidor de acesso para cliente.</span><span class="sxs-lookup"><span data-stu-id="caa15-125">Contains the specifications for connecting a client to the Client Access server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="caa15-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="caa15-126">Remarks</span></span>

<span data-ttu-id="caa15-127">O elemento **MailStore** está presente em uma resposta que tem um elemento [Protocol (POX)](protocol-pox.md) com um valor de atributo **Type** de "mapiHttp".</span><span class="sxs-lookup"><span data-stu-id="caa15-127">The **MailStore** element is present in a response that has a [Protocol (POX)](protocol-pox.md) element with a **Type** attribute value of "mapiHttp".</span></span> 
  
<span data-ttu-id="caa15-128">O elemento **MailStore** está disponível para clientes que implementam o protocolo MAPI/http e direcionam o Exchange Online, o Exchange Online como parte do Office 365 e as versões locais do Exchange a partir do Build 15.00.0847.032 (exchange server 2013 SP1).</span><span class="sxs-lookup"><span data-stu-id="caa15-128">The **MailStore** element is available to clients that implement the MAPI/HTTP protocol and target Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="caa15-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="caa15-129">See also</span></span>



[<span data-ttu-id="caa15-130">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="caa15-130">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

