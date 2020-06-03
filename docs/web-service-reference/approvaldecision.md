---
title: ApprovalDecision
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5e7c5687-cb9e-4f0b-ac8f-b82591914a39
description: O elemento ApprovalDecision especifica a decisão feita em uma mensagem de solicitação de aprovação.
ms.openlocfilehash: a8dc168edec882ba97cdea764f8d20c71ed85f8a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463444"
---
# <a name="approvaldecision"></a><span data-ttu-id="ecd9d-103">ApprovalDecision</span><span class="sxs-lookup"><span data-stu-id="ecd9d-103">ApprovalDecision</span></span>

<span data-ttu-id="ecd9d-104">O elemento **ApprovalDecision** especifica a decisão feita em uma mensagem de solicitação de aprovação.</span><span class="sxs-lookup"><span data-stu-id="ecd9d-104">The **ApprovalDecision** element specifies the decision made on an approval request message.</span></span> 
  
```XML
<ApprovalDecision> 1 | 2 </ApprovalDecision>
```

 <span data-ttu-id="ecd9d-105">**int**</span><span class="sxs-lookup"><span data-stu-id="ecd9d-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ecd9d-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ecd9d-106">Attributes and elements</span></span>

<span data-ttu-id="ecd9d-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ecd9d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ecd9d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ecd9d-108">Attributes</span></span>

<span data-ttu-id="ecd9d-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ecd9d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ecd9d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ecd9d-110">Child elements</span></span>

<span data-ttu-id="ecd9d-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ecd9d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ecd9d-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ecd9d-112">Parent elements</span></span>

[<span data-ttu-id="ecd9d-113">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="ecd9d-113">ApprovalRequestData</span></span>](approvalrequestdata.md)
  
## <a name="text-value"></a><span data-ttu-id="ecd9d-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="ecd9d-114">Text value</span></span>

<span data-ttu-id="ecd9d-115">O valor de texto do elemento **ApprovalDecision** será 1 se for aprovado e 2 se rejeitado.</span><span class="sxs-lookup"><span data-stu-id="ecd9d-115">The text value of the **ApprovalDecision** element is 1 if approved and 2 if rejected.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ecd9d-116">Comentários</span><span class="sxs-lookup"><span data-stu-id="ecd9d-116">Remarks</span></span>

<span data-ttu-id="ecd9d-117">Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ecd9d-117">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="ecd9d-118">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ecd9d-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ecd9d-119">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ecd9d-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ecd9d-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="ecd9d-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ecd9d-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ecd9d-121">Schema Name</span></span>  <br/> |<span data-ttu-id="ecd9d-122">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ecd9d-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="ecd9d-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ecd9d-123">Validation File</span></span>  <br/> |<span data-ttu-id="ecd9d-124">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ecd9d-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ecd9d-125">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ecd9d-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="ecd9d-126">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="ecd9d-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ecd9d-127">Confira também</span><span class="sxs-lookup"><span data-stu-id="ecd9d-127">See also</span></span>

- [<span data-ttu-id="ecd9d-128">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="ecd9d-128">ApprovalRequestData</span></span>](approvalrequestdata.md)
- [<span data-ttu-id="ecd9d-129">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ecd9d-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

