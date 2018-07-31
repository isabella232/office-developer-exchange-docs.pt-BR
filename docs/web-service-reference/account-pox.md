---
title: Account (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 488fdbdc-e9d9-4301-91ab-e22eb42e549e
description: O elemento de conta Especifica as configurações da conta do usuário ou contém respostas de erro.
ms.openlocfilehash: 6cd87e678b3a524a69f6dca4d6999a3cff22fa57
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353340"
---
# <a name="account-pox"></a><span data-ttu-id="90671-103">Account (POX)</span><span class="sxs-lookup"><span data-stu-id="90671-103">Account (POX)</span></span>

<span data-ttu-id="90671-104">O elemento de **conta** Especifica as configurações da conta do usuário ou contém respostas de erro.</span><span class="sxs-lookup"><span data-stu-id="90671-104">The **Account** element specifies account settings for the user or contains error responses.</span></span> 
  
- [<span data-ttu-id="90671-105">AutoDiscover (POX)</span><span class="sxs-lookup"><span data-stu-id="90671-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
- [<span data-ttu-id="90671-106">Response (POX)</span><span class="sxs-lookup"><span data-stu-id="90671-106">Response (POX)</span></span>](response-pox.md)
- [<span data-ttu-id="90671-107">Account (POX)</span><span class="sxs-lookup"><span data-stu-id="90671-107">Account (POX)</span></span>](account-pox.md)
  
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

## <a name="attributes-and-elements"></a><span data-ttu-id="90671-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="90671-108">Attributes and elements</span></span>

<span data-ttu-id="90671-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="90671-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="90671-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="90671-110">Attributes</span></span>

<span data-ttu-id="90671-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="90671-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="90671-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="90671-112">Child elements</span></span>

|<span data-ttu-id="90671-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="90671-113">**Element**</span></span>|<span data-ttu-id="90671-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="90671-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="90671-115">AccountType (POX)</span><span class="sxs-lookup"><span data-stu-id="90671-115">AccountType (POX)</span></span>](accounttype-pox.md) <br/> |<span data-ttu-id="90671-116">Representa o tipo de conta.</span><span class="sxs-lookup"><span data-stu-id="90671-116">Represents the account type.</span></span>  <br/> |
|[<span data-ttu-id="90671-117">Action (POX)</span><span class="sxs-lookup"><span data-stu-id="90671-117">Action (POX)</span></span>](action-pox.md) <br/> |<span data-ttu-id="90671-118">Fornece informações que são usadas para determinar se outra solicitação de descoberta automática é necessária para retornar as informações de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="90671-118">Provides information that is used to determine whether another Autodiscover request is required to return the user configuration information.</span></span>  <br/> |
|[<span data-ttu-id="90671-119">MicrosoftOnline (POX)</span><span class="sxs-lookup"><span data-stu-id="90671-119">MicrosoftOnline (POX)</span></span>](microsoftonline-pox.md) <br/> |<span data-ttu-id="90671-120">Contém um valor que indica se caixas de correio do usuário está hospedada no Exchange Online ou Exchange Online como parte do Office 365.</span><span class="sxs-lookup"><span data-stu-id="90671-120">Contains a value that indicates whether the user's mailbox is hosted in Exchange Online or Exchange Online as part of Office 365.</span></span>  <br/> |
|[<span data-ttu-id="90671-121">RedirectUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="90671-121">RedirectUrl (POX)</span></span>](redirecturl-pox.md) <br/> |<span data-ttu-id="90671-122">Contém a URL do computador que está executando o Exchange Server que possui a função de servidor do acesso para cliente instalada deve ser usada para obter as configurações de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="90671-122">Contains the URL of the computer that is running Exchange Server that has the Client Access server role installed that should be used to obtain Autodiscover settings.</span></span>  <br/> |
|[<span data-ttu-id="90671-123">RedirectAddr (POX)</span><span class="sxs-lookup"><span data-stu-id="90671-123">RedirectAddr (POX)</span></span>](redirectaddr-pox.md) <br/> |<span data-ttu-id="90671-124">Especifica o endereço de email que deve ser usado para uma solicitação de descoberta automática subsequente.</span><span class="sxs-lookup"><span data-stu-id="90671-124">Specifies the email address that should be used for a subsequent Autodiscover request.</span></span>  <br/> |
|[<span data-ttu-id="90671-125">Image (POX)</span><span class="sxs-lookup"><span data-stu-id="90671-125">Image (POX)</span></span>](image-pox.md) <br/> |<span data-ttu-id="90671-126">Contém o caminho de uma imagem que é usado para marcar a experiência de configuração.</span><span class="sxs-lookup"><span data-stu-id="90671-126">Contains the path of an image that is used to brand the configuration experience.</span></span>  <br/> |
|[<span data-ttu-id="90671-127">ServiceHome (POX)</span><span class="sxs-lookup"><span data-stu-id="90671-127">ServiceHome (POX)</span></span>](servicehome-pox.md) <br/> |<span data-ttu-id="90671-128">Contém a URL da home page do provedor de serviços de Internet (ISP).</span><span class="sxs-lookup"><span data-stu-id="90671-128">Contains the URL of the home page of the Internet service provider (ISP).</span></span>  <br/> |
|[<span data-ttu-id="90671-129">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="90671-129">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="90671-130">Contém as especificações para conectar um cliente para o servidor de acesso para cliente.</span><span class="sxs-lookup"><span data-stu-id="90671-130">Contains the specifications for connecting a client to the Client Access server.</span></span>  <br/> |
|[<span data-ttu-id="90671-131">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="90671-131">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md) <br/> |<span data-ttu-id="90671-132">Contém informações que os clientes podem usar para enviar uma solicitação de descoberta automática para descobrir informações de pasta pública para o usuário.</span><span class="sxs-lookup"><span data-stu-id="90671-132">Contains information that clients can use to send an Autodiscover request to discover public folder information for the user.</span></span>  <br/> |
|[<span data-ttu-id="90671-133">Error (POX)</span><span class="sxs-lookup"><span data-stu-id="90671-133">Error (POX)</span></span>](error-pox.md) <br/> |<span data-ttu-id="90671-134">Contém uma resposta de erro de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="90671-134">Contains an Autodiscover error response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="90671-135">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="90671-135">Parent elements</span></span>

|<span data-ttu-id="90671-136">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="90671-136">**Element**</span></span>|<span data-ttu-id="90671-137">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="90671-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="90671-138">Response (POX)</span><span class="sxs-lookup"><span data-stu-id="90671-138">Response (POX)</span></span>](response-pox.md) <br/> |<span data-ttu-id="90671-139">Contém a resposta do serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="90671-139">Contains the response from the Autodiscover service.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="90671-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="90671-140">See also</span></span>

- [<span data-ttu-id="90671-141">Elementos de Autodiscover XML POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="90671-141">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

