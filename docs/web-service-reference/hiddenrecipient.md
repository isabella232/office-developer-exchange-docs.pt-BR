---
title: HiddenRecipient
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- HiddenRecipient
api_type:
- schema
ms.assetid: a8209f75-0070-4424-8dcd-273cfd192728
description: O elemento HiddenRecipient indica que o destinatário foi adicionado por uma política de organização que deve ficar ocultos dos usuários sem privilégios.
ms.openlocfilehash: 73b2e3e39c675cf3e2bc56105b1e76009d4a2451
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823810"
---
# <a name="hiddenrecipient"></a><span data-ttu-id="30899-103">HiddenRecipient</span><span class="sxs-lookup"><span data-stu-id="30899-103">HiddenRecipient</span></span>

<span data-ttu-id="30899-104">O elemento **HiddenRecipient** indica que o destinatário foi adicionado por uma política de organização que deve ficar ocultos dos usuários sem privilégios.</span><span class="sxs-lookup"><span data-stu-id="30899-104">The **HiddenRecipient** element indicates that the recipient was added by an organization policy that should be hidden from unprivileged users.</span></span> 
  
```XML
<HiddenRecipient>true | false</HiddenRecipient>
```

 <span data-ttu-id="30899-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="30899-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="30899-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="30899-106">Attributes and elements</span></span>

<span data-ttu-id="30899-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="30899-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="30899-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="30899-108">Attributes</span></span>

<span data-ttu-id="30899-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="30899-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="30899-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="30899-110">Child elements</span></span>

<span data-ttu-id="30899-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="30899-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="30899-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="30899-112">Parent elements</span></span>

|<span data-ttu-id="30899-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="30899-113">**Element**</span></span>|<span data-ttu-id="30899-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="30899-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="30899-115">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="30899-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="30899-116">Contém informações para um único evento de um destinatário.</span><span class="sxs-lookup"><span data-stu-id="30899-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="30899-117">Text value</span><span class="sxs-lookup"><span data-stu-id="30899-117">Text value</span></span>

<span data-ttu-id="30899-118">Esse elemento pode ser **true** ou **false**.</span><span class="sxs-lookup"><span data-stu-id="30899-118">This element can be either **true** or **false**.</span></span> <span data-ttu-id="30899-119">Um valor **true** indica que o usuário foi adicionado por uma política de organização; um valor **false** indica que o usuário não foi adicionado por uma política de organização.</span><span class="sxs-lookup"><span data-stu-id="30899-119">A value of **true** indicates that the user was added by an organization policy; a value of **false** indicates that the user was not added by an organization policy.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="30899-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="30899-120">Remarks</span></span>

<span data-ttu-id="30899-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="30899-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="30899-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="30899-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="30899-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="30899-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="30899-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="30899-124">Schema Name</span></span>  <br/> |<span data-ttu-id="30899-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="30899-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="30899-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="30899-126">Validation File</span></span>  <br/> |<span data-ttu-id="30899-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="30899-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="30899-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="30899-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="30899-129">False</span><span class="sxs-lookup"><span data-stu-id="30899-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="30899-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="30899-130">See also</span></span>



- [<span data-ttu-id="30899-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="30899-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

