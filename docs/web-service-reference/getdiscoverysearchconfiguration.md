---
title: GetDiscoverySearchConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e15dbfca-3b9d-463e-94ec-4f1b6115bee3
description: O elemento GetDiscoverySearchConfiguration Especifica uma solicitação para recuperar a configuração de pesquisa de descoberta eletrônica.
ms.openlocfilehash: 41a3cabb2822c4ee6a31aa7ff3074d62987edc92
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752460"
---
# <a name="getdiscoverysearchconfiguration"></a><span data-ttu-id="f8665-103">GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="f8665-103">GetDiscoverySearchConfiguration</span></span>

<span data-ttu-id="f8665-104">O elemento **GetDiscoverySearchConfiguration** Especifica uma solicitação para recuperar a configuração de pesquisa de descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="f8665-104">The **GetDiscoverySearchConfiguration** element specifies a request to retrieve the eDiscovery search configuration.</span></span> 
  
```XML
<GetDiscoverySearchConfiguration>
    <SearchId/>
    <ExpandGroupMembership/>
</GetDiscoverySearchConfiguration>
```

 <span data-ttu-id="f8665-105">**GetDiscoverySearchConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="f8665-105">**GetDiscoverySearchConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f8665-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f8665-106">Attributes and elements</span></span>

<span data-ttu-id="f8665-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f8665-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f8665-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f8665-108">Attributes</span></span>

<span data-ttu-id="f8665-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f8665-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f8665-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f8665-110">Child elements</span></span>

|<span data-ttu-id="f8665-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f8665-111">**Element**</span></span>|<span data-ttu-id="f8665-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f8665-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f8665-113">SearchId</span><span class="sxs-lookup"><span data-stu-id="f8665-113">SearchId</span></span>](searchid.md) <br/> |<span data-ttu-id="f8665-114">Especifica o identificador da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="f8665-114">Specifies the identifier of the search.</span></span>  <br/> |
|[<span data-ttu-id="f8665-115">ExpandGroupMembership</span><span class="sxs-lookup"><span data-stu-id="f8665-115">ExpandGroupMembership</span></span>](expandgroupmembership.md) <br/> |<span data-ttu-id="f8665-116">Contém um valor Boolean que indica se é necessário expandir a associação do grupo retornado de uma solicitação de **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="f8665-116">Contains a Boolean value that indicates whether to expand the membership of the group returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f8665-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f8665-117">Parent elements</span></span>

<span data-ttu-id="f8665-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f8665-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f8665-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="f8665-119">Remarks</span></span>

<span data-ttu-id="f8665-120">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f8665-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f8665-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f8665-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f8665-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f8665-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f8665-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="f8665-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f8665-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f8665-124">Schema Name</span></span>  <br/> |<span data-ttu-id="f8665-125">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="f8665-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="f8665-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f8665-126">Validation File</span></span>  <br/> |<span data-ttu-id="f8665-127">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f8665-127">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f8665-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="f8665-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="f8665-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="f8665-129">See also</span></span>



- [<span data-ttu-id="f8665-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f8665-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

