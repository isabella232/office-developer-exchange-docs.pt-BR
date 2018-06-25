---
title: IsExternalMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5cc83174-e684-42c8-b72a-f82d3de3bb2f
description: O elemento IsExternalMailbox indica se a caixa de correio é parte da organização.
ms.openlocfilehash: cf9f71e9b955cffd1bebefd5f23acba66ba1b894
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824010"
---
# <a name="isexternalmailbox"></a><span data-ttu-id="dd689-103">IsExternalMailbox</span><span class="sxs-lookup"><span data-stu-id="dd689-103">IsExternalMailbox</span></span>

<span data-ttu-id="dd689-104">O elemento **IsExternalMailbox** indica se a caixa de correio é parte da organização.</span><span class="sxs-lookup"><span data-stu-id="dd689-104">The **IsExternalMailbox** element indicates whether the mailbox is external to the organization.</span></span> 
  
```XML
<IsExternalMailbox>true | false</IsExternalMailbox>
```

 <span data-ttu-id="dd689-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="dd689-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dd689-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="dd689-106">Attributes and elements</span></span>

<span data-ttu-id="dd689-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="dd689-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dd689-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="dd689-108">Attributes</span></span>

<span data-ttu-id="dd689-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="dd689-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dd689-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="dd689-110">Child elements</span></span>

<span data-ttu-id="dd689-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="dd689-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dd689-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="dd689-112">Parent elements</span></span>

[<span data-ttu-id="dd689-113">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="dd689-113">SearchableMailbox</span></span>](searchablemailbox.md)
  
## <a name="text-value"></a><span data-ttu-id="dd689-114">Text value</span><span class="sxs-lookup"><span data-stu-id="dd689-114">Text value</span></span>

<span data-ttu-id="dd689-115">Um valor de texto de **true** para o elemento **IsExternalMailbox** indica que a caixa de correio está em uma organização externa.</span><span class="sxs-lookup"><span data-stu-id="dd689-115">A text value of **true** for the **IsExternalMailbox** element indicates that the mailbox is in an external organization.</span></span> <span data-ttu-id="dd689-116">Um valor **false** indica que a caixa de correio está na organização.</span><span class="sxs-lookup"><span data-stu-id="dd689-116">A value of **false** indicates that the mailbox is in the organization.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="dd689-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="dd689-117">Remarks</span></span>

<span data-ttu-id="dd689-118">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="dd689-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="dd689-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="dd689-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dd689-120">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="dd689-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dd689-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="dd689-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dd689-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="dd689-122">Schema name</span></span>  <br/> |<span data-ttu-id="dd689-123">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="dd689-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="dd689-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="dd689-124">Validation file</span></span>  <br/> |<span data-ttu-id="dd689-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="dd689-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dd689-126">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="dd689-126">Can be empty</span></span>  <br/> |<span data-ttu-id="dd689-127">False</span><span class="sxs-lookup"><span data-stu-id="dd689-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dd689-128">Ver também</span><span class="sxs-lookup"><span data-stu-id="dd689-128">See also</span></span>



- [<span data-ttu-id="dd689-129">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="dd689-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

