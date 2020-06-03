---
title: GetDiscoverySearchConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e15dbfca-3b9d-463e-94ec-4f1b6115bee3
description: O elemento GetDiscoverySearchConfiguration especifica uma solicitação para recuperar a configuração de pesquisa de descoberta eletrônica.
ms.openlocfilehash: 821c5e1429c160e326f6d99df3ff4fcc831b83d1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460999"
---
# <a name="getdiscoverysearchconfiguration"></a><span data-ttu-id="24de2-103">GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="24de2-103">GetDiscoverySearchConfiguration</span></span>

<span data-ttu-id="24de2-104">O elemento **GetDiscoverySearchConfiguration** especifica uma solicitação para recuperar a configuração de pesquisa de descoberta eletrônica.</span><span class="sxs-lookup"><span data-stu-id="24de2-104">The **GetDiscoverySearchConfiguration** element specifies a request to retrieve the eDiscovery search configuration.</span></span> 
  
```XML
<GetDiscoverySearchConfiguration>
    <SearchId/>
    <ExpandGroupMembership/>
</GetDiscoverySearchConfiguration>
```

 <span data-ttu-id="24de2-105">**GetDiscoverySearchConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="24de2-105">**GetDiscoverySearchConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="24de2-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="24de2-106">Attributes and elements</span></span>

<span data-ttu-id="24de2-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="24de2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="24de2-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="24de2-108">Attributes</span></span>

<span data-ttu-id="24de2-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="24de2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="24de2-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="24de2-110">Child elements</span></span>

|<span data-ttu-id="24de2-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="24de2-111">**Element**</span></span>|<span data-ttu-id="24de2-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="24de2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="24de2-113">SearchId</span><span class="sxs-lookup"><span data-stu-id="24de2-113">SearchId</span></span>](searchid.md) <br/> |<span data-ttu-id="24de2-114">Especifica o identificador da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="24de2-114">Specifies the identifier of the search.</span></span>  <br/> |
|[<span data-ttu-id="24de2-115">ExpandGroupMembership</span><span class="sxs-lookup"><span data-stu-id="24de2-115">ExpandGroupMembership</span></span>](expandgroupmembership.md) <br/> |<span data-ttu-id="24de2-116">Contém um valor Boolean que indica se a associação do grupo retornado de uma solicitação **GetSearchableMailboxes** deve ser expandida.</span><span class="sxs-lookup"><span data-stu-id="24de2-116">Contains a Boolean value that indicates whether to expand the membership of the group returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="24de2-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="24de2-117">Parent elements</span></span>

<span data-ttu-id="24de2-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="24de2-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="24de2-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="24de2-119">Remarks</span></span>

<span data-ttu-id="24de2-120">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="24de2-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="24de2-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="24de2-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="24de2-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="24de2-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="24de2-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="24de2-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="24de2-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="24de2-124">Schema Name</span></span>  <br/> |<span data-ttu-id="24de2-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="24de2-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="24de2-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="24de2-126">Validation File</span></span>  <br/> |<span data-ttu-id="24de2-127">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="24de2-127">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="24de2-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="24de2-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="24de2-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="24de2-129">See also</span></span>



- [<span data-ttu-id="24de2-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="24de2-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

