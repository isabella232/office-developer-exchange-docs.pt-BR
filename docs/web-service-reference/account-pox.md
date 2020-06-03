---
title: Conta (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 488fdbdc-e9d9-4301-91ab-e22eb42e549e
description: O elemento Account especifica as configurações de conta do usuário ou contém respostas de erro.
ms.openlocfilehash: ffd8ebe4b7bd9d4b3f6a9b42fc557ac6189a068d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462315"
---
# <a name="account-pox"></a><span data-ttu-id="4ab2a-103">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="4ab2a-103">Account (POX)</span></span>

<span data-ttu-id="4ab2a-104">O elemento **Account** especifica as configurações de conta do usuário ou contém respostas de erro.</span><span class="sxs-lookup"><span data-stu-id="4ab2a-104">The **Account** element specifies account settings for the user or contains error responses.</span></span> 
  
- [<span data-ttu-id="4ab2a-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="4ab2a-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
- [<span data-ttu-id="4ab2a-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="4ab2a-106">Response (POX)</span></span>](response-pox.md)
- [<span data-ttu-id="4ab2a-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="4ab2a-107">Account (POX)</span></span>](account-pox.md)
  
```XML
<Account>
   <AccountType/>
   <Action/>
   <MicrosoftOnline/>
   <RedirectURL/>
   <RedirectAddr/>
   <Image/>
   <ServiceHome/>
   <Protocol/>
   <PublicFolderInformation/>
</Account>
```

<br/>

```XML
<Account> 
    <Error/> 
</Account>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="4ab2a-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="4ab2a-108">Attributes and elements</span></span>

<span data-ttu-id="4ab2a-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4ab2a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4ab2a-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="4ab2a-110">Attributes</span></span>

<span data-ttu-id="4ab2a-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4ab2a-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4ab2a-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4ab2a-112">Child elements</span></span>

|<span data-ttu-id="4ab2a-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4ab2a-113">**Element**</span></span>|<span data-ttu-id="4ab2a-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4ab2a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ab2a-115">AccountType (POX)</span><span class="sxs-lookup"><span data-stu-id="4ab2a-115">AccountType (POX)</span></span>](accounttype-pox.md) <br/> |<span data-ttu-id="4ab2a-116">Representa o tipo de conta.</span><span class="sxs-lookup"><span data-stu-id="4ab2a-116">Represents the account type.</span></span>  <br/> |
|[<span data-ttu-id="4ab2a-117">Ação (POX)</span><span class="sxs-lookup"><span data-stu-id="4ab2a-117">Action (POX)</span></span>](action-pox.md) <br/> |<span data-ttu-id="4ab2a-118">Fornece informações que são usadas para determinar se outra solicitação de descoberta automática é necessária para retornar as informações de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="4ab2a-118">Provides information that is used to determine whether another Autodiscover request is required to return the user configuration information.</span></span>  <br/> |
|[<span data-ttu-id="4ab2a-119">MicrosoftOnline (POX)</span><span class="sxs-lookup"><span data-stu-id="4ab2a-119">MicrosoftOnline (POX)</span></span>](microsoftonline-pox.md) <br/> |<span data-ttu-id="4ab2a-120">Contém um valor que indica se a caixa de correio do usuário está hospedada no Exchange Online ou no Exchange Online como parte do Office 365.</span><span class="sxs-lookup"><span data-stu-id="4ab2a-120">Contains a value that indicates whether the user's mailbox is hosted in Exchange Online or Exchange Online as part of Office 365.</span></span>  <br/> |
|[<span data-ttu-id="4ab2a-121">RedirectUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="4ab2a-121">RedirectUrl (POX)</span></span>](redirecturl-pox.md) <br/> |<span data-ttu-id="4ab2a-122">Contém a URL do computador que está executando o Exchange Server que tem a função de servidor de acesso para Cliente instalada que deve ser usada para obter as configurações de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="4ab2a-122">Contains the URL of the computer that is running Exchange Server that has the Client Access server role installed that should be used to obtain Autodiscover settings.</span></span>  <br/> |
|[<span data-ttu-id="4ab2a-123">RedirectAddr (POX)</span><span class="sxs-lookup"><span data-stu-id="4ab2a-123">RedirectAddr (POX)</span></span>](redirectaddr-pox.md) <br/> |<span data-ttu-id="4ab2a-124">Especifica o endereço de email que deve ser usado para uma solicitação de descoberta automática subsequente.</span><span class="sxs-lookup"><span data-stu-id="4ab2a-124">Specifies the email address that should be used for a subsequent Autodiscover request.</span></span>  <br/> |
|[<span data-ttu-id="4ab2a-125">Imagem (POX)</span><span class="sxs-lookup"><span data-stu-id="4ab2a-125">Image (POX)</span></span>](image-pox.md) <br/> |<span data-ttu-id="4ab2a-126">Contém o caminho de uma imagem usada para marcar a experiência de configuração.</span><span class="sxs-lookup"><span data-stu-id="4ab2a-126">Contains the path of an image that is used to brand the configuration experience.</span></span>  <br/> |
|[<span data-ttu-id="4ab2a-127">Onhome (POX)</span><span class="sxs-lookup"><span data-stu-id="4ab2a-127">ServiceHome (POX)</span></span>](servicehome-pox.md) <br/> |<span data-ttu-id="4ab2a-128">Contém a URL da home page do provedor de serviços de Internet (ISP).</span><span class="sxs-lookup"><span data-stu-id="4ab2a-128">Contains the URL of the home page of the Internet service provider (ISP).</span></span>  <br/> |
|[<span data-ttu-id="4ab2a-129">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="4ab2a-129">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="4ab2a-130">Contém as especificações para conectar um cliente ao servidor de acesso para cliente.</span><span class="sxs-lookup"><span data-stu-id="4ab2a-130">Contains the specifications for connecting a client to the Client Access server.</span></span>  <br/> |
|[<span data-ttu-id="4ab2a-131">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="4ab2a-131">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md) <br/> |<span data-ttu-id="4ab2a-132">Contém informações que os clientes podem usar para enviar uma solicitação de descoberta automática para descobrir informações de pasta pública para o usuário.</span><span class="sxs-lookup"><span data-stu-id="4ab2a-132">Contains information that clients can use to send an Autodiscover request to discover public folder information for the user.</span></span>  <br/> |
|[<span data-ttu-id="4ab2a-133">Erro (POX)</span><span class="sxs-lookup"><span data-stu-id="4ab2a-133">Error (POX)</span></span>](error-pox.md) <br/> |<span data-ttu-id="4ab2a-134">Contém uma resposta de erro de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="4ab2a-134">Contains an Autodiscover error response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4ab2a-135">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4ab2a-135">Parent elements</span></span>

|<span data-ttu-id="4ab2a-136">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4ab2a-136">**Element**</span></span>|<span data-ttu-id="4ab2a-137">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4ab2a-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ab2a-138">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="4ab2a-138">Response (POX)</span></span>](response-pox.md) <br/> |<span data-ttu-id="4ab2a-139">Contém a resposta do serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="4ab2a-139">Contains the response from the Autodiscover service.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4ab2a-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="4ab2a-140">See also</span></span>

- [<span data-ttu-id="4ab2a-141">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="4ab2a-141">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

