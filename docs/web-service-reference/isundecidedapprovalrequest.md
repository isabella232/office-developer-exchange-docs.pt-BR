---
title: IsUndecidedApprovalRequest
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 90841617-3b83-4124-8125-0293c9470f4a
description: O elemento IsUndecidedApprovalRequest especifica se uma mensagem de solicitação de aprovação foi acionada.
ms.openlocfilehash: 0949cf64b8583c4b3fa5a1700475f01cc480f69f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458170"
---
# <a name="isundecidedapprovalrequest"></a><span data-ttu-id="33b63-103">IsUndecidedApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="33b63-103">IsUndecidedApprovalRequest</span></span>

<span data-ttu-id="33b63-104">O elemento **IsUndecidedApprovalRequest** especifica se uma mensagem de solicitação de aprovação foi acionada.</span><span class="sxs-lookup"><span data-stu-id="33b63-104">The **IsUndecidedApprovalRequest** element specifies whether an approval request message has been acted on.</span></span> 
  
```XML
<IsUndecidedApprovalRequest> true | false </IsUndecidedApprovalRequest>
```

 <span data-ttu-id="33b63-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="33b63-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="33b63-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="33b63-106">Attributes and elements</span></span>

<span data-ttu-id="33b63-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="33b63-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="33b63-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="33b63-108">Attributes</span></span>

<span data-ttu-id="33b63-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="33b63-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="33b63-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="33b63-110">Child elements</span></span>

<span data-ttu-id="33b63-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="33b63-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="33b63-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="33b63-112">Parent elements</span></span>

[<span data-ttu-id="33b63-113">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="33b63-113">ApprovalRequestData</span></span>](approvalrequestdata.md)
  
## <a name="text-value"></a><span data-ttu-id="33b63-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="33b63-114">Text value</span></span>

<span data-ttu-id="33b63-115">O valor de texto do elemento **IsUndecidedApprovalRequest** será **true** se uma mensagem de solicitação de aprovação não tiver sido acionada.</span><span class="sxs-lookup"><span data-stu-id="33b63-115">The text value of the **IsUndecidedApprovalRequest** element is **true** if an approval request message has not been acted on.</span></span> <span data-ttu-id="33b63-116">Um valor **false** indica que a solicitação de aprovação foi decidida.</span><span class="sxs-lookup"><span data-stu-id="33b63-116">A value of **false** indicates that the approval request has been decided.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="33b63-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="33b63-117">Remarks</span></span>

<span data-ttu-id="33b63-118">Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="33b63-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="33b63-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="33b63-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="33b63-120">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="33b63-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="33b63-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="33b63-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="33b63-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="33b63-122">Schema Name</span></span>  <br/> |<span data-ttu-id="33b63-123">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="33b63-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="33b63-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="33b63-124">Validation File</span></span>  <br/> |<span data-ttu-id="33b63-125">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="33b63-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="33b63-126">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="33b63-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="33b63-127">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="33b63-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="33b63-128">Confira também</span><span class="sxs-lookup"><span data-stu-id="33b63-128">See also</span></span>



[<span data-ttu-id="33b63-129">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="33b63-129">ApprovalRequestData</span></span>](approvalrequestdata.md)


- [<span data-ttu-id="33b63-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="33b63-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

