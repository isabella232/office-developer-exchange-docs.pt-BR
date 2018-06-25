---
title: ApprovalDecision
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5e7c5687-cb9e-4f0b-ac8f-b82591914a39
description: O elemento ApprovalDecision Especifica a decisão feita em uma mensagem de solicitação de aprovação.
ms.openlocfilehash: 4ca73813440200e5d2fb9f920d81459d8cd5e4ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751189"
---
# <a name="approvaldecision"></a><span data-ttu-id="7dc65-103">ApprovalDecision</span><span class="sxs-lookup"><span data-stu-id="7dc65-103">ApprovalDecision</span></span>

<span data-ttu-id="7dc65-104">O elemento **ApprovalDecision** Especifica a decisão feita em uma mensagem de solicitação de aprovação.</span><span class="sxs-lookup"><span data-stu-id="7dc65-104">The **ApprovalDecision** element specifies the decision made on an approval request message.</span></span> 
  
```XML
<ApprovalDecision> 1 | 2 </ApprovalDecision>
```

 <span data-ttu-id="7dc65-105">**int**</span><span class="sxs-lookup"><span data-stu-id="7dc65-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7dc65-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="7dc65-106">Attributes and elements</span></span>

<span data-ttu-id="7dc65-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7dc65-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7dc65-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="7dc65-108">Attributes</span></span>

<span data-ttu-id="7dc65-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7dc65-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7dc65-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7dc65-110">Child elements</span></span>

<span data-ttu-id="7dc65-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7dc65-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7dc65-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7dc65-112">Parent elements</span></span>

[<span data-ttu-id="7dc65-113">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="7dc65-113">ApprovalRequestData</span></span>](approvalrequestdata.md)
  
## <a name="text-value"></a><span data-ttu-id="7dc65-114">Text value</span><span class="sxs-lookup"><span data-stu-id="7dc65-114">Text value</span></span>

<span data-ttu-id="7dc65-115">O valor de texto do elemento **ApprovalDecision** é 1 se aprovada e 2 rejeição.</span><span class="sxs-lookup"><span data-stu-id="7dc65-115">The text value of the **ApprovalDecision** element is 1 if approved and 2 if rejected.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="7dc65-116">Comentários</span><span class="sxs-lookup"><span data-stu-id="7dc65-116">Remarks</span></span>

<span data-ttu-id="7dc65-117">Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="7dc65-117">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="7dc65-118">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7dc65-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7dc65-119">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="7dc65-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7dc65-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="7dc65-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7dc65-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7dc65-121">Schema Name</span></span>  <br/> |<span data-ttu-id="7dc65-122">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="7dc65-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="7dc65-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7dc65-123">Validation File</span></span>  <br/> |<span data-ttu-id="7dc65-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7dc65-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7dc65-125">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="7dc65-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="7dc65-126">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="7dc65-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7dc65-127">Ver também</span><span class="sxs-lookup"><span data-stu-id="7dc65-127">See also</span></span>

- [<span data-ttu-id="7dc65-128">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="7dc65-128">ApprovalRequestData</span></span>](approvalrequestdata.md)
- [<span data-ttu-id="7dc65-129">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7dc65-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

