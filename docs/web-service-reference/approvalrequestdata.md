---
title: ApprovalRequestData
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6c971cf7-5c3a-4e5e-9a7d-048f4ac0aadb
description: O elemento ApprovalRequestData especifica o estado de aprovação de uma mensagem de solicitação de aprovação.
ms.openlocfilehash: decbd4d646a56b9810387adcdb6a9049da89bc38
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462301"
---
# <a name="approvalrequestdata"></a><span data-ttu-id="de9a2-103">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="de9a2-103">ApprovalRequestData</span></span>

<span data-ttu-id="de9a2-104">O elemento **ApprovalRequestData** especifica o estado de aprovação de uma mensagem de solicitação de aprovação.</span><span class="sxs-lookup"><span data-stu-id="de9a2-104">The **ApprovalRequestData** element specifies the approval state of an approval request message.</span></span> 
  
```xml
<ApprovalRequestData>
   <IsUndecidedApprovalRequest/>
   <ApprovalDecision/>
   <ApprovalDecisionMaker/>
   <ApprovalDecisionTime/>
</ApprovalRequestData>
```

 <span data-ttu-id="de9a2-105">**ApprovalRequestDataType**</span><span class="sxs-lookup"><span data-stu-id="de9a2-105">**ApprovalRequestDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="de9a2-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="de9a2-106">Attributes and elements</span></span>

<span data-ttu-id="de9a2-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="de9a2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="de9a2-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="de9a2-108">Attributes</span></span>

<span data-ttu-id="de9a2-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="de9a2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="de9a2-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="de9a2-110">Child elements</span></span>

<span data-ttu-id="de9a2-111">[IsUndecidedApprovalRequest](isundecidedapprovalrequest.md)  |  [ApprovalDecision](approvaldecision.md)  |  [ApprovalDecisionMaker](approvaldecisionmaker.md)  |  [ApprovalDecisionTime](approvaldecisiontime.md)</span><span class="sxs-lookup"><span data-stu-id="de9a2-111">[IsUndecidedApprovalRequest](isundecidedapprovalrequest.md) | [ApprovalDecision](approvaldecision.md) | [ApprovalDecisionMaker](approvaldecisionmaker.md) | [ApprovalDecisionTime](approvaldecisiontime.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="de9a2-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="de9a2-112">Parent elements</span></span>

[<span data-ttu-id="de9a2-113">Mensagem</span><span class="sxs-lookup"><span data-stu-id="de9a2-113">Message</span></span>](message-ex15websvcsotherref.md)
  
## <a name="remarks"></a><span data-ttu-id="de9a2-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="de9a2-114">Remarks</span></span>

<span data-ttu-id="de9a2-115">Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="de9a2-115">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="de9a2-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="de9a2-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="de9a2-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="de9a2-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="de9a2-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="de9a2-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="de9a2-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="de9a2-119">Schema Name</span></span>  <br/> |<span data-ttu-id="de9a2-120">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="de9a2-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="de9a2-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="de9a2-121">Validation File</span></span>  <br/> |<span data-ttu-id="de9a2-122">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="de9a2-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="de9a2-123">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="de9a2-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="de9a2-124">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="de9a2-124">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="de9a2-125">Confira também</span><span class="sxs-lookup"><span data-stu-id="de9a2-125">See also</span></span>

- [<span data-ttu-id="de9a2-126">Mensagem</span><span class="sxs-lookup"><span data-stu-id="de9a2-126">Message</span></span>](message-ex15websvcsotherref.md)
- [<span data-ttu-id="de9a2-127">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="de9a2-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

