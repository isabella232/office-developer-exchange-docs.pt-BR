---
title: Guid
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 49dcf69f-bf8d-4be6-a24c-03bbd13f4fe5
description: O elemento de Guid Especifica o identificador exclusivo da caixa de correio.
ms.openlocfilehash: 35307a706523fc5c2916767c7508dec07deb8d09
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823799"
---
# <a name="guid"></a><span data-ttu-id="da26c-103">Guid</span><span class="sxs-lookup"><span data-stu-id="da26c-103">Guid</span></span>

<span data-ttu-id="da26c-104">O elemento de **Guid** Especifica o identificador exclusivo da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="da26c-104">The **Guid** element specifies the globally unique identifier of the mailbox.</span></span> 
  
```XML
<Guid></Guid>
```

 <span data-ttu-id="da26c-105">**GuidType**</span><span class="sxs-lookup"><span data-stu-id="da26c-105">**GuidType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="da26c-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="da26c-106">Attributes and elements</span></span>

<span data-ttu-id="da26c-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="da26c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="da26c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="da26c-108">Attributes</span></span>

<span data-ttu-id="da26c-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="da26c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="da26c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="da26c-110">Child elements</span></span>

<span data-ttu-id="da26c-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="da26c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="da26c-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="da26c-112">Parent elements</span></span>

|<span data-ttu-id="da26c-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="da26c-113">**Element**</span></span>|<span data-ttu-id="da26c-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="da26c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="da26c-115">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="da26c-115">SearchableMailbox</span></span>](searchablemailbox.md) <br/> |<span data-ttu-id="da26c-116">Especifica uma caixa de correio retornados de uma solicitação de **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="da26c-116">Specifies a mailbox returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="da26c-117">Text value</span><span class="sxs-lookup"><span data-stu-id="da26c-117">Text value</span></span>

<span data-ttu-id="da26c-118">O valor de texto do elemento **Guid** é um valor GUID que identifica exclusivamente uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="da26c-118">The text value of the **Guid** element is a GUID value that uniquely identifies a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="da26c-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="da26c-119">Remarks</span></span>

<span data-ttu-id="da26c-120">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="da26c-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="da26c-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="da26c-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="da26c-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="da26c-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="da26c-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="da26c-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="da26c-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="da26c-124">Schema Name</span></span>  <br/> |<span data-ttu-id="da26c-125">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="da26c-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="da26c-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="da26c-126">Validation File</span></span>  <br/> |<span data-ttu-id="da26c-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="da26c-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="da26c-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="da26c-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="da26c-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="da26c-129">See also</span></span>



- [<span data-ttu-id="da26c-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="da26c-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

