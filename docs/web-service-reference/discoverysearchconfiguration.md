---
title: DiscoverySearchConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 085384f9-dca4-4534-82e2-dd782471d0da
description: O elemento DiscoverySearchConfiguration especifica a configuração da pesquisa de descoberta eletrônica.
ms.openlocfilehash: 8819d951f35ccc215bdf0128d2a16b60bbf20f2a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529053"
---
# <a name="discoverysearchconfiguration"></a><span data-ttu-id="cad4f-103">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="cad4f-103">DiscoverySearchConfiguration</span></span>

<span data-ttu-id="cad4f-104">O elemento **DiscoverySearchConfiguration** especifica a configuração da pesquisa de descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="cad4f-104">The **DiscoverySearchConfiguration** element specifies the configuration for eDiscovery search.</span></span> 
  
```XML
<DiscoverySearchConfiguration>
    <SearchId></SearchId>
    <SearchQuery></SearchQuery>
    <SearchableMailboxes></SearchableMailboxes>
</DiscoverySearchConfiguration>
```

 <span data-ttu-id="cad4f-105">**DiscoverySearchConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="cad4f-105">**DiscoverySearchConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cad4f-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="cad4f-106">Attributes and elements</span></span>

<span data-ttu-id="cad4f-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="cad4f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cad4f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="cad4f-108">Attributes</span></span>

<span data-ttu-id="cad4f-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cad4f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cad4f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="cad4f-110">Child elements</span></span>

|<span data-ttu-id="cad4f-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cad4f-111">**Element**</span></span>|<span data-ttu-id="cad4f-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cad4f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cad4f-113">SearchId</span><span class="sxs-lookup"><span data-stu-id="cad4f-113">SearchId</span></span>](searchid.md) <br/> |<span data-ttu-id="cad4f-114">Especifica o identificador da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="cad4f-114">Specifies the identifier of the search.</span></span>  <br/> |
|[<span data-ttu-id="cad4f-115">SearchQuery</span><span class="sxs-lookup"><span data-stu-id="cad4f-115">SearchQuery</span></span>](searchquery.md) <br/> |<span data-ttu-id="cad4f-116">Especifica o nome de uma consulta de pesquisa de descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="cad4f-116">Specifies the name of an eDiscovery search query.</span></span>  <br/> |
|[<span data-ttu-id="cad4f-117">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="cad4f-117">SearchableMailboxes</span></span>](searchablemailboxes.md) <br/> |<span data-ttu-id="cad4f-118">Contém uma lista das caixas de correio retornadas de uma solicitação **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="cad4f-118">Contains a list of the mailboxes returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cad4f-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="cad4f-119">Parent elements</span></span>

|<span data-ttu-id="cad4f-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cad4f-120">**Element**</span></span>|<span data-ttu-id="cad4f-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cad4f-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cad4f-122">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="cad4f-122">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md) <br/> |<span data-ttu-id="cad4f-123">Especifica uma matriz de elementos **DiscoverySearchConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="cad4f-123">Specifies an array of **DiscoverySearchConfiguration** elements.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cad4f-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="cad4f-124">Remarks</span></span>

<span data-ttu-id="cad4f-125">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="cad4f-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="cad4f-126">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="cad4f-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cad4f-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="cad4f-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cad4f-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="cad4f-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cad4f-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="cad4f-129">Schema Name</span></span>  <br/> |<span data-ttu-id="cad4f-130">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="cad4f-130">Message schema</span></span>  <br/> |
|<span data-ttu-id="cad4f-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="cad4f-131">Validation File</span></span>  <br/> |<span data-ttu-id="cad4f-132">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="cad4f-132">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cad4f-133">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="cad4f-133">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="cad4f-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="cad4f-134">See also</span></span>

- [<span data-ttu-id="cad4f-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="cad4f-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

