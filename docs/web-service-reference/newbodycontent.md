---
title: NewBodyContent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NewBodyContent
api_type:
- schema
ms.assetid: 0303600d-16d8-4685-88f2-980c5ca7e9a6
description: O elemento NewBodyContent representa o novo conteúdo de corpo de uma mensagem.
ms.openlocfilehash: b87393e460b1eee1c13efebf38e898d17915bd71
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824516"
---
# <a name="newbodycontent"></a><span data-ttu-id="2b45c-103">NewBodyContent</span><span class="sxs-lookup"><span data-stu-id="2b45c-103">NewBodyContent</span></span>

<span data-ttu-id="2b45c-104">O elemento **NewBodyContent** representa o novo conteúdo de corpo de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="2b45c-104">The **NewBodyContent** element represents the new body content of a message.</span></span> 
  
```xml
<NewBodyContent BodyType=""/>
```

 <span data-ttu-id="2b45c-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="2b45c-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2b45c-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="2b45c-106">Attributes and elements</span></span>

<span data-ttu-id="2b45c-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2b45c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2b45c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2b45c-108">Attributes</span></span>

|<span data-ttu-id="2b45c-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="2b45c-109">**Attribute**</span></span>|<span data-ttu-id="2b45c-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2b45c-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2b45c-111">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="2b45c-111">**BodyType**</span></span> <br/> |<span data-ttu-id="2b45c-112">Representa o conteúdo real do corpo de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="2b45c-112">Represents the actual body content of a message.</span></span>  <br/> |
   
#### <a name="bodytype-attribute"></a><span data-ttu-id="2b45c-113">Atributo BodyType</span><span class="sxs-lookup"><span data-stu-id="2b45c-113">BodyType Attribute</span></span>

|<span data-ttu-id="2b45c-114">**Valor**</span><span class="sxs-lookup"><span data-stu-id="2b45c-114">**Value**</span></span>|<span data-ttu-id="2b45c-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2b45c-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2b45c-116">**HTML**</span><span class="sxs-lookup"><span data-stu-id="2b45c-116">**HTML**</span></span> <br/> |<span data-ttu-id="2b45c-117">Converte todos os corpos em HTML.</span><span class="sxs-lookup"><span data-stu-id="2b45c-117">Converts all bodies to HTML.</span></span>  <br/> |
|<span data-ttu-id="2b45c-118">**Text**</span><span class="sxs-lookup"><span data-stu-id="2b45c-118">**Text**</span></span> <br/> |<span data-ttu-id="2b45c-119">Converte todos os corpos de texto sem formatação.</span><span class="sxs-lookup"><span data-stu-id="2b45c-119">Converts all bodies to plain text.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="2b45c-120">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2b45c-120">Child elements</span></span>

<span data-ttu-id="2b45c-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2b45c-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2b45c-122">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2b45c-122">Parent elements</span></span>

|<span data-ttu-id="2b45c-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2b45c-123">**Element**</span></span>|<span data-ttu-id="2b45c-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2b45c-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2b45c-125">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="2b45c-125">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="2b45c-126">Contém uma resposta ao remetente de um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2b45c-126">Contains a reply to the sender of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2b45c-127">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="2b45c-127">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="2b45c-128">Contém uma resposta para o remetente e identificados todos os destinatários de um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2b45c-128">Contains a reply to the sender and all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2b45c-129">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="2b45c-129">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="2b45c-130">Contém um item de armazenamento do Exchange para encaminhar para destinatários.</span><span class="sxs-lookup"><span data-stu-id="2b45c-130">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="2b45c-131">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="2b45c-131">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="2b45c-132">Representa o objeto de resposta é usado para cancelar uma reunião.</span><span class="sxs-lookup"><span data-stu-id="2b45c-132">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="2b45c-133">PostReplyItem</span><span class="sxs-lookup"><span data-stu-id="2b45c-133">PostReplyItem</span></span>](postreplyitem.md) <br/> |<span data-ttu-id="2b45c-134">Contém uma resposta para um item de postagem.</span><span class="sxs-lookup"><span data-stu-id="2b45c-134">Contains a reply to a post item.</span></span> <span data-ttu-id="2b45c-135">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="2b45c-135">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2b45c-136">Text value</span><span class="sxs-lookup"><span data-stu-id="2b45c-136">Text value</span></span>

<span data-ttu-id="2b45c-137">O valor de texto representa o novo conteúdo de corpo de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="2b45c-137">The text value represents the new body content of a message.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2b45c-138">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="2b45c-138">Remarks</span></span>

<span data-ttu-id="2b45c-139">O esquema que descreve este elemento está localizado no diretório virtual EWS do servidor do Exchange que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="2b45c-139">The schema that describes this element is located in the EWS virtual directory of the Exchange server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2b45c-140">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="2b45c-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2b45c-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="2b45c-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2b45c-142">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2b45c-142">Schema Name</span></span>  <br/> |<span data-ttu-id="2b45c-143">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="2b45c-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="2b45c-144">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2b45c-144">Validation File</span></span>  <br/> |<span data-ttu-id="2b45c-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2b45c-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2b45c-146">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="2b45c-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="2b45c-147">False</span><span class="sxs-lookup"><span data-stu-id="2b45c-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2b45c-148">Ver também</span><span class="sxs-lookup"><span data-stu-id="2b45c-148">See also</span></span>



- [<span data-ttu-id="2b45c-149">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2b45c-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

