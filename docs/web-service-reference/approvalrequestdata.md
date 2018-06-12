---
title: ApprovalRequestData
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6c971cf7-5c3a-4e5e-9a7d-048f4ac0aadb
description: O elemento ApprovalRequestData Especifica o estado de aprovação de uma mensagem de solicitação de aprovação.
ms.openlocfilehash: ed1c1e3db4edd2cf4de032dc61abd73e863d4f1d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751193"
---
# <a name="approvalrequestdata"></a><span data-ttu-id="4dbb5-103">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="4dbb5-103">ApprovalRequestData</span></span>

<span data-ttu-id="4dbb5-104">O elemento **ApprovalRequestData** Especifica o estado de aprovação de uma mensagem de solicitação de aprovação.</span><span class="sxs-lookup"><span data-stu-id="4dbb5-104">The **ApprovalRequestData** element specifies the approval state of an approval request message.</span></span> 
  
```xml
<ApprovalRequestData>
   <IsUndecidedApprovalRequest/>
   <ApprovalDecision/>
   <ApprovalDecisionMaker/>
   <ApprovalDecisionTime/>
</ApprovalRequestData>
```

 <span data-ttu-id="4dbb5-105">**ApprovalRequestDataType**</span><span class="sxs-lookup"><span data-stu-id="4dbb5-105">**ApprovalRequestDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4dbb5-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="4dbb5-106">Attributes and elements</span></span>

<span data-ttu-id="4dbb5-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4dbb5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4dbb5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4dbb5-108">Attributes</span></span>

<span data-ttu-id="4dbb5-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4dbb5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4dbb5-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4dbb5-110">Child elements</span></span>

<span data-ttu-id="4dbb5-111">[IsUndecidedApprovalRequest](isundecidedapprovalrequest.md) | [ApprovalDecision](approvaldecision.md) | [ApprovalDecisionMaker](approvaldecisionmaker.md) | [ApprovalDecisionTime](approvaldecisiontime.md)</span><span class="sxs-lookup"><span data-stu-id="4dbb5-111">[IsUndecidedApprovalRequest](isundecidedapprovalrequest.md) | [ApprovalDecision](approvaldecision.md) | [ApprovalDecisionMaker](approvaldecisionmaker.md) | [ApprovalDecisionTime](approvaldecisiontime.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4dbb5-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4dbb5-112">Parent elements</span></span>

[<span data-ttu-id="4dbb5-113">Mensagem</span><span class="sxs-lookup"><span data-stu-id="4dbb5-113">Message</span></span>](message-ex15websvcsotherref.md)
  
## <a name="remarks"></a><span data-ttu-id="4dbb5-114">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="4dbb5-114">Remarks</span></span>

<span data-ttu-id="4dbb5-115">Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="4dbb5-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="4dbb5-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4dbb5-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4dbb5-117">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="4dbb5-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4dbb5-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="4dbb5-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4dbb5-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4dbb5-119">Schema Name</span></span>  <br/> |<span data-ttu-id="4dbb5-120">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="4dbb5-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="4dbb5-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4dbb5-121">Validation File</span></span>  <br/> |<span data-ttu-id="4dbb5-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4dbb5-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4dbb5-123">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="4dbb5-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="4dbb5-124">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="4dbb5-124">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4dbb5-125">Ver também</span><span class="sxs-lookup"><span data-stu-id="4dbb5-125">See also</span></span>

- [<span data-ttu-id="4dbb5-126">Mensagem</span><span class="sxs-lookup"><span data-stu-id="4dbb5-126">Message</span></span>](message-ex15websvcsotherref.md)
- [<span data-ttu-id="4dbb5-127">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4dbb5-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

