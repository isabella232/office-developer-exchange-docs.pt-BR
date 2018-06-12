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
description: O elemento OWAUrl descreve a URL e o esquema de autenticação que é usada para acessar um determinado computador que executa o Microsoft Exchange Server 2007 que possui a função acesso para cliente instalada que hospeda o Outlook Web Access.
ms.openlocfilehash: 93d03506e2a74aa1b4ef6d2a49ccbda01cfc1f9a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824673"
---
# <a name="owaurl-pox"></a><span data-ttu-id="9cf13-103">OWAUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="9cf13-103">OWAUrl (POX)</span></span>

<span data-ttu-id="9cf13-104">O elemento **OWAUrl** descreve a URL e o esquema de autenticação que é usada para acessar um determinado computador que executa o Microsoft Exchange Server 2007 que possui a função acesso para cliente instalada que hospeda o Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="9cf13-104">The **OWAUrl** element describes the URL and authentication schema that is used to access a particular computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed that hosts Outlook Web Access.</span></span> 
  
[<span data-ttu-id="9cf13-105">Descoberta automática (POX)</span><span class="sxs-lookup"><span data-stu-id="9cf13-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="9cf13-106">Resposta POX)</span><span class="sxs-lookup"><span data-stu-id="9cf13-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="9cf13-107">Conta (POX)</span><span class="sxs-lookup"><span data-stu-id="9cf13-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="9cf13-108">Protocolo (POX)</span><span class="sxs-lookup"><span data-stu-id="9cf13-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="9cf13-109">Interno (POX)</span><span class="sxs-lookup"><span data-stu-id="9cf13-109">Internal (POX)</span></span>](internal-pox.md)
  
[<span data-ttu-id="9cf13-110">OWAUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="9cf13-110">OWAUrl (POX)</span></span>](owaurl-pox.md)
  
```xml
<OWAUrl AuthenticationMethod=""/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="9cf13-111">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="9cf13-111">Attributes and elements</span></span>

<span data-ttu-id="9cf13-112">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9cf13-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9cf13-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="9cf13-113">Attributes</span></span>

|<span data-ttu-id="9cf13-114">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="9cf13-114">**Attribute**</span></span>|<span data-ttu-id="9cf13-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9cf13-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9cf13-116">**AuthenticationMethod**</span><span class="sxs-lookup"><span data-stu-id="9cf13-116">**AuthenticationMethod**</span></span> <br/> |<span data-ttu-id="9cf13-117">Descreve os métodos de autenticação para acessar o Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="9cf13-117">Describes the authentication methods for accessing Outlook Web Access.</span></span>  <br/> |
   
#### <a name="authenticationmethod-attribute"></a><span data-ttu-id="9cf13-118">Atributo AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="9cf13-118">AuthenticationMethod Attribute</span></span>

|<span data-ttu-id="9cf13-119">**Valor**</span><span class="sxs-lookup"><span data-stu-id="9cf13-119">**Value**</span></span>|<span data-ttu-id="9cf13-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9cf13-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9cf13-121">WindowsIntegrated</span><span class="sxs-lookup"><span data-stu-id="9cf13-121">WindowsIntegrated</span></span>  <br/> |<span data-ttu-id="9cf13-122">Autenticação integrada do Windows.</span><span class="sxs-lookup"><span data-stu-id="9cf13-122">Integrated Windows authentication.</span></span>  <br/> |
|<span data-ttu-id="9cf13-123">FBA</span><span class="sxs-lookup"><span data-stu-id="9cf13-123">FBA</span></span>  <br/> |<span data-ttu-id="9cf13-124">Autenticação baseada em formulários.</span><span class="sxs-lookup"><span data-stu-id="9cf13-124">Forms-based authentication.</span></span>  <br/> |
|<span data-ttu-id="9cf13-125">NTLM</span><span class="sxs-lookup"><span data-stu-id="9cf13-125">NTLM</span></span>  <br/> |<span data-ttu-id="9cf13-126">Autenticação NTLM.</span><span class="sxs-lookup"><span data-stu-id="9cf13-126">NTLM authentication.</span></span>  <br/> |
|<span data-ttu-id="9cf13-127">Digest</span><span class="sxs-lookup"><span data-stu-id="9cf13-127">Digest</span></span>  <br/> |<span data-ttu-id="9cf13-128">Autenticação Digest.</span><span class="sxs-lookup"><span data-stu-id="9cf13-128">Digest authentication.</span></span>  <br/> |
|<span data-ttu-id="9cf13-129">Básico</span><span class="sxs-lookup"><span data-stu-id="9cf13-129">Basic</span></span>  <br/> |<span data-ttu-id="9cf13-130">Autenticação básica.</span><span class="sxs-lookup"><span data-stu-id="9cf13-130">Basic authentication.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9cf13-131">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9cf13-131">Child elements</span></span>

<span data-ttu-id="9cf13-132">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9cf13-132">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9cf13-133">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9cf13-133">Parent elements</span></span>

|<span data-ttu-id="9cf13-134">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9cf13-134">**Element**</span></span>|<span data-ttu-id="9cf13-135">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9cf13-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9cf13-136">Interno (POX)</span><span class="sxs-lookup"><span data-stu-id="9cf13-136">Internal (POX)</span></span>](internal-pox.md) <br/> |<span data-ttu-id="9cf13-137">Contém a coleção de URLs do Outlook Web Access que um cliente pode se conectar ao quando ele estiver dentro do firewall.</span><span class="sxs-lookup"><span data-stu-id="9cf13-137">Contains the collection of Outlook Web Access URLs that a client can connect to when it is inside the firewall.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9cf13-138">Text value</span><span class="sxs-lookup"><span data-stu-id="9cf13-138">Text value</span></span>

<span data-ttu-id="9cf13-139">O valor de texto representa a URL do serviço do Outlook Web Access em um servidor de acesso para cliente.</span><span class="sxs-lookup"><span data-stu-id="9cf13-139">The text value represents the URL for the Outlook Web Access service on a Client Access server.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="9cf13-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="9cf13-140">See also</span></span>



[<span data-ttu-id="9cf13-141">Elementos de Autodiscover XML POX para Exchange</span><span class="sxs-lookup"><span data-stu-id="9cf13-141">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

