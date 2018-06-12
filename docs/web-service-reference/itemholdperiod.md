---
title: ItemHoldPeriod
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 30369db5-4d45-40e8-bc83-3236667fc404
description: O elemento ItemHoldPeriod Especifica a quantidade de tempo para armazenar o conteúdo que corresponda a consulta de caixa de correio.
ms.openlocfilehash: 212d765aa3f0493dd4f3051de483fa08a6fa8ac7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824144"
---
# <a name="itemholdperiod"></a><span data-ttu-id="ef6b0-103">ItemHoldPeriod</span><span class="sxs-lookup"><span data-stu-id="ef6b0-103">ItemHoldPeriod</span></span>

<span data-ttu-id="ef6b0-104">O elemento **ItemHoldPeriod** Especifica a quantidade de tempo para armazenar o conteúdo que corresponda a consulta de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="ef6b0-104">The **ItemHoldPeriod** element specifies the amount of time to hold content that matches the mailbox query.</span></span> 
  
```XML
<ItemHoldPeriod/>
```

 <span data-ttu-id="ef6b0-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="ef6b0-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ef6b0-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ef6b0-106">Attributes and elements</span></span>

<span data-ttu-id="ef6b0-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ef6b0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ef6b0-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ef6b0-108">Attributes</span></span>

<span data-ttu-id="ef6b0-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ef6b0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ef6b0-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ef6b0-110">Child elements</span></span>

<span data-ttu-id="ef6b0-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ef6b0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ef6b0-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ef6b0-112">Parent elements</span></span>

[<span data-ttu-id="ef6b0-113">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="ef6b0-113">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
  
## <a name="text-value"></a><span data-ttu-id="ef6b0-114">Text value</span><span class="sxs-lookup"><span data-stu-id="ef6b0-114">Text value</span></span>

<span data-ttu-id="ef6b0-115">O valor de texto pode ser "Unlimited" ou o valor de cadeia de caracteres de qualquer valor [Timespan](http://msdn.microsoft.com/en-us/library/1ecy8h51%28v=vs.110%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ef6b0-115">The text value can be "Unlimited" or the string value of any [Timespan](http://msdn.microsoft.com/en-us/library/1ecy8h51%28v=vs.110%29.aspx) value.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ef6b0-116">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="ef6b0-116">Remarks</span></span>

<span data-ttu-id="ef6b0-117">Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ef6b0-117">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="ef6b0-118">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ef6b0-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ef6b0-119">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ef6b0-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ef6b0-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="ef6b0-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ef6b0-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ef6b0-121">Schema Name</span></span>  <br/> |<span data-ttu-id="ef6b0-122">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="ef6b0-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ef6b0-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ef6b0-123">Validation File</span></span>  <br/> |<span data-ttu-id="ef6b0-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ef6b0-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ef6b0-125">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ef6b0-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="ef6b0-126">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="ef6b0-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ef6b0-127">Ver também</span><span class="sxs-lookup"><span data-stu-id="ef6b0-127">See also</span></span>



[<span data-ttu-id="ef6b0-128">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="ef6b0-128">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)


- [<span data-ttu-id="ef6b0-129">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ef6b0-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

