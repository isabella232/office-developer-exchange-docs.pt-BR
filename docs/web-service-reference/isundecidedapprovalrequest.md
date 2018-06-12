---
title: IsUndecidedApprovalRequest
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 90841617-3b83-4124-8125-0293c9470f4a
description: O elemento IsUndecidedApprovalRequest Especifica se uma mensagem de solicitação de aprovação tiver sido acionada.
ms.openlocfilehash: 82b4624df5b2fe7ca212fdf76248e1ccfa3a081f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824127"
---
# <a name="isundecidedapprovalrequest"></a><span data-ttu-id="3c788-103">IsUndecidedApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="3c788-103">IsUndecidedApprovalRequest</span></span>

<span data-ttu-id="3c788-104">O elemento **IsUndecidedApprovalRequest** Especifica se uma mensagem de solicitação de aprovação tiver sido acionada.</span><span class="sxs-lookup"><span data-stu-id="3c788-104">The **IsUndecidedApprovalRequest** element specifies whether an approval request message has been acted on.</span></span> 
  
```XML
<IsUndecidedApprovalRequest> true | false </IsUndecidedApprovalRequest>
```

 <span data-ttu-id="3c788-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="3c788-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3c788-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3c788-106">Attributes and elements</span></span>

<span data-ttu-id="3c788-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3c788-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3c788-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3c788-108">Attributes</span></span>

<span data-ttu-id="3c788-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3c788-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3c788-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3c788-110">Child elements</span></span>

<span data-ttu-id="3c788-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3c788-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3c788-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3c788-112">Parent elements</span></span>

[<span data-ttu-id="3c788-113">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="3c788-113">ApprovalRequestData</span></span>](approvalrequestdata.md)
  
## <a name="text-value"></a><span data-ttu-id="3c788-114">Text value</span><span class="sxs-lookup"><span data-stu-id="3c788-114">Text value</span></span>

<span data-ttu-id="3c788-115">O valor de texto do elemento **IsUndecidedApprovalRequest** é **true** se uma mensagem de solicitação de aprovação não tiver sido realizada.</span><span class="sxs-lookup"><span data-stu-id="3c788-115">The text value of the **IsUndecidedApprovalRequest** element is **true** if an approval request message has not been acted on.</span></span> <span data-ttu-id="3c788-116">Um valor **false** indica que a solicitação de aprovação foi decidida.</span><span class="sxs-lookup"><span data-stu-id="3c788-116">A value of **false** indicates that the approval request has been decided.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3c788-117">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="3c788-117">Remarks</span></span>

<span data-ttu-id="3c788-118">Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="3c788-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="3c788-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3c788-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3c788-120">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3c788-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3c788-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="3c788-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3c788-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3c788-122">Schema Name</span></span>  <br/> |<span data-ttu-id="3c788-123">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3c788-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="3c788-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3c788-124">Validation File</span></span>  <br/> |<span data-ttu-id="3c788-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3c788-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3c788-126">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3c788-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="3c788-127">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="3c788-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3c788-128">Ver também</span><span class="sxs-lookup"><span data-stu-id="3c788-128">See also</span></span>



[<span data-ttu-id="3c788-129">ApprovalRequestData</span><span class="sxs-lookup"><span data-stu-id="3c788-129">ApprovalRequestData</span></span>](approvalrequestdata.md)


- [<span data-ttu-id="3c788-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3c788-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

