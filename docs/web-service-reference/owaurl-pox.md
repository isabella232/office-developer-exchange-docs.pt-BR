---
title: OWAUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 450b86a1-1722-49f5-b541-16c1edc3db7a
description: O elemento OWAUrl descreve a URL e o esquema de autenticação usados para acessar um determinado computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada que hospeda o Outlook Web Access.
ms.openlocfilehash: c0728af063cfbf1353eb7d3b81f5fcfe8b398f7d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457260"
---
# <a name="owaurl-pox"></a><span data-ttu-id="e5313-103">OWAUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="e5313-103">OWAUrl (POX)</span></span>

<span data-ttu-id="e5313-104">O elemento **OWAUrl** descreve a URL e o esquema de autenticação usados para acessar um determinado computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada que hospeda o Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="e5313-104">The **OWAUrl** element describes the URL and authentication schema that is used to access a particular computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed that hosts Outlook Web Access.</span></span> 
  
[<span data-ttu-id="e5313-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="e5313-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="e5313-106">Resposta (POX)</span><span class="sxs-lookup"><span data-stu-id="e5313-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="e5313-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="e5313-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="e5313-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="e5313-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="e5313-109">Interno (POX)</span><span class="sxs-lookup"><span data-stu-id="e5313-109">Internal (POX)</span></span>](internal-pox.md)
  
[<span data-ttu-id="e5313-110">OWAUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="e5313-110">OWAUrl (POX)</span></span>](owaurl-pox.md)
  
```xml
<OWAUrl AuthenticationMethod=""/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="e5313-111">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e5313-111">Attributes and elements</span></span>

<span data-ttu-id="e5313-112">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e5313-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e5313-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="e5313-113">Attributes</span></span>

|<span data-ttu-id="e5313-114">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="e5313-114">**Attribute**</span></span>|<span data-ttu-id="e5313-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e5313-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e5313-116">**AuthenticationMethod**</span><span class="sxs-lookup"><span data-stu-id="e5313-116">**AuthenticationMethod**</span></span> <br/> |<span data-ttu-id="e5313-117">Descreve os métodos de autenticação para acessar o Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="e5313-117">Describes the authentication methods for accessing Outlook Web Access.</span></span>  <br/> |
   
#### <a name="authenticationmethod-attribute"></a><span data-ttu-id="e5313-118">Atributo AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e5313-118">AuthenticationMethod Attribute</span></span>

|<span data-ttu-id="e5313-119">**Valor**</span><span class="sxs-lookup"><span data-stu-id="e5313-119">**Value**</span></span>|<span data-ttu-id="e5313-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e5313-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e5313-121">WindowsIntegrated</span><span class="sxs-lookup"><span data-stu-id="e5313-121">WindowsIntegrated</span></span>  <br/> |<span data-ttu-id="e5313-122">Autenticação integrada do Windows.</span><span class="sxs-lookup"><span data-stu-id="e5313-122">Integrated Windows authentication.</span></span>  <br/> |
|<span data-ttu-id="e5313-123">FBA</span><span class="sxs-lookup"><span data-stu-id="e5313-123">FBA</span></span>  <br/> |<span data-ttu-id="e5313-124">Autenticação baseada em formulários.</span><span class="sxs-lookup"><span data-stu-id="e5313-124">Forms-based authentication.</span></span>  <br/> |
|<span data-ttu-id="e5313-125">NTLM</span><span class="sxs-lookup"><span data-stu-id="e5313-125">NTLM</span></span>  <br/> |<span data-ttu-id="e5313-126">Autenticação NTLM.</span><span class="sxs-lookup"><span data-stu-id="e5313-126">NTLM authentication.</span></span>  <br/> |
|<span data-ttu-id="e5313-127">Digest</span><span class="sxs-lookup"><span data-stu-id="e5313-127">Digest</span></span>  <br/> |<span data-ttu-id="e5313-128">Autenticação Digest.</span><span class="sxs-lookup"><span data-stu-id="e5313-128">Digest authentication.</span></span>  <br/> |
|<span data-ttu-id="e5313-129">Básica</span><span class="sxs-lookup"><span data-stu-id="e5313-129">Basic</span></span>  <br/> |<span data-ttu-id="e5313-130">Autenticação básica.</span><span class="sxs-lookup"><span data-stu-id="e5313-130">Basic authentication.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e5313-131">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e5313-131">Child elements</span></span>

<span data-ttu-id="e5313-132">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e5313-132">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e5313-133">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e5313-133">Parent elements</span></span>

|<span data-ttu-id="e5313-134">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e5313-134">**Element**</span></span>|<span data-ttu-id="e5313-135">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e5313-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e5313-136">Interno (POX)</span><span class="sxs-lookup"><span data-stu-id="e5313-136">Internal (POX)</span></span>](internal-pox.md) <br/> |<span data-ttu-id="e5313-137">Contém a coleção de URLs do Outlook Web Access às quais um cliente pode se conectar quando está dentro do firewall.</span><span class="sxs-lookup"><span data-stu-id="e5313-137">Contains the collection of Outlook Web Access URLs that a client can connect to when it is inside the firewall.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e5313-138">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="e5313-138">Text value</span></span>

<span data-ttu-id="e5313-139">O valor de texto representa a URL do serviço do Outlook Web Access em um servidor de acesso para cliente.</span><span class="sxs-lookup"><span data-stu-id="e5313-139">The text value represents the URL for the Outlook Web Access service on a Client Access server.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="e5313-140">Também consulte</span><span class="sxs-lookup"><span data-stu-id="e5313-140">See also</span></span>



[<span data-ttu-id="e5313-141">Elementos XML de descoberta automática de POX para o Exchange</span><span class="sxs-lookup"><span data-stu-id="e5313-141">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

