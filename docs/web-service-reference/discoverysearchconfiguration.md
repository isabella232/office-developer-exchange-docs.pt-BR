---
title: DiscoverySearchConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 085384f9-dca4-4534-82e2-dd782471d0da
description: O elemento DiscoverySearchConfiguration Especifica a configuração de pesquisa de descoberta eletrônica.
ms.openlocfilehash: 11bf90d8fe73bb0b308deb7ae51f1443488f87e2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751855"
---
# <a name="discoverysearchconfiguration"></a><span data-ttu-id="af916-103">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="af916-103">DiscoverySearchConfiguration</span></span>

<span data-ttu-id="af916-104">O elemento **DiscoverySearchConfiguration** Especifica a configuração de pesquisa de descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="af916-104">The **DiscoverySearchConfiguration** element specifies the configuration for eDiscovery search.</span></span> 
  
```XML
<DiscoverySearchConfiguration>
    <SearchId></SearchId>
    <SearchQuery></SearchQuery>
    <SearchableMailboxes></SearchableMailboxes>
</DiscoverySearchConfiguration>
```

 <span data-ttu-id="af916-105">**DiscoverySearchConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="af916-105">**DiscoverySearchConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="af916-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="af916-106">Attributes and elements</span></span>

<span data-ttu-id="af916-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="af916-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="af916-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="af916-108">Attributes</span></span>

<span data-ttu-id="af916-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="af916-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="af916-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="af916-110">Child elements</span></span>

|<span data-ttu-id="af916-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="af916-111">**Element**</span></span>|<span data-ttu-id="af916-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="af916-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="af916-113">SearchId</span><span class="sxs-lookup"><span data-stu-id="af916-113">SearchId</span></span>](searchid.md) <br/> |<span data-ttu-id="af916-114">Especifica o identificador da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="af916-114">Specifies the identifier of the search.</span></span>  <br/> |
|[<span data-ttu-id="af916-115">SearchQuery</span><span class="sxs-lookup"><span data-stu-id="af916-115">SearchQuery</span></span>](searchquery.md) <br/> |<span data-ttu-id="af916-116">Especifica o nome de uma consulta de pesquisa de descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="af916-116">Specifies the name of an eDiscovery search query.</span></span>  <br/> |
|[<span data-ttu-id="af916-117">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="af916-117">SearchableMailboxes</span></span>](searchablemailboxes.md) <br/> |<span data-ttu-id="af916-118">Contém uma lista das caixas de correio retornados de uma solicitação de **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="af916-118">Contains a list of the mailboxes returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="af916-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="af916-119">Parent elements</span></span>

|<span data-ttu-id="af916-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="af916-120">**Element**</span></span>|<span data-ttu-id="af916-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="af916-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="af916-122">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="af916-122">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md) <br/> |<span data-ttu-id="af916-123">Especifica uma matriz de elementos de **DiscoverySearchConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="af916-123">Specifies an array of **DiscoverySearchConfiguration** elements.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="af916-124">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="af916-124">Remarks</span></span>

<span data-ttu-id="af916-125">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="af916-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="af916-126">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="af916-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="af916-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="af916-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="af916-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="af916-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="af916-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="af916-129">Schema Name</span></span>  <br/> |<span data-ttu-id="af916-130">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="af916-130">Message schema</span></span>  <br/> |
|<span data-ttu-id="af916-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="af916-131">Validation File</span></span>  <br/> |<span data-ttu-id="af916-132">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="af916-132">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="af916-133">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="af916-133">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="af916-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="af916-134">See also</span></span>

- [<span data-ttu-id="af916-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="af916-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

