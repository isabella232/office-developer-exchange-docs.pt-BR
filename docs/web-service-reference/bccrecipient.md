---
title: BccRecipient
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BccRecipient
api_type:
- schema
ms.assetid: 4ef0cff5-8a5a-4d76-9d2b-938774d8fc1b
description: O elemento BccRecipient representa um destinatário para receber uma cópia carbono oculta (Cco) de uma mensagem de email.
ms.openlocfilehash: bed58536263196a61651493e92a4dcd1df3f5ec9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751260"
---
# <a name="bccrecipient"></a><span data-ttu-id="cd96f-103">BccRecipient</span><span class="sxs-lookup"><span data-stu-id="cd96f-103">BccRecipient</span></span>

<span data-ttu-id="cd96f-104">O elemento **BccRecipient** representa um destinatário para receber uma cópia carbono oculta (Cco) de uma mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="cd96f-104">The **BccRecipient** element represents a recipient to receive a blind carbon copy (Bcc) of an e-mail message.</span></span> 
  
```XML
<BccRecipient>true | false</BccRecipient>
```

 <span data-ttu-id="cd96f-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="cd96f-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cd96f-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="cd96f-106">Attributes and elements</span></span>

<span data-ttu-id="cd96f-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="cd96f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cd96f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="cd96f-108">Attributes</span></span>

<span data-ttu-id="cd96f-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cd96f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cd96f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="cd96f-110">Child elements</span></span>

<span data-ttu-id="cd96f-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cd96f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cd96f-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="cd96f-112">Parent elements</span></span>

|<span data-ttu-id="cd96f-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cd96f-113">**Element**</span></span>|<span data-ttu-id="cd96f-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cd96f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cd96f-115">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="cd96f-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="cd96f-116">Contém informações para um único evento de um destinatário.</span><span class="sxs-lookup"><span data-stu-id="cd96f-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cd96f-117">Text value</span><span class="sxs-lookup"><span data-stu-id="cd96f-117">Text value</span></span>

<span data-ttu-id="cd96f-118">Esse elemento pode ser **true** ou **false**.</span><span class="sxs-lookup"><span data-stu-id="cd96f-118">This element can be either **true** or **false**.</span></span> <span data-ttu-id="cd96f-119">Um valor **true** indica que o destinatário está cego carbono copiado; um valor **false** indica que o destinatário não é copiado de carbono deficientes Visual.</span><span class="sxs-lookup"><span data-stu-id="cd96f-119">A value of **true** indicates that the recipient is blind carbon copied; a value of **false** indicates that the recipient is not blind carbon copied.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="cd96f-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="cd96f-120">Remarks</span></span>

<span data-ttu-id="cd96f-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="cd96f-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cd96f-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="cd96f-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cd96f-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="cd96f-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cd96f-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="cd96f-124">Schema Name</span></span>  <br/> |<span data-ttu-id="cd96f-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="cd96f-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="cd96f-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="cd96f-126">Validation File</span></span>  <br/> |<span data-ttu-id="cd96f-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cd96f-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cd96f-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="cd96f-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="cd96f-129">False</span><span class="sxs-lookup"><span data-stu-id="cd96f-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cd96f-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="cd96f-130">See also</span></span>



- [<span data-ttu-id="cd96f-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="cd96f-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

