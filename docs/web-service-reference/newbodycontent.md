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
description: O elemento NewBodyContent representa o novo conteúdo do corpo de uma mensagem.
ms.openlocfilehash: dcfa927bb284ff00e510d8c7b4b31910a70b3cbb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466854"
---
# <a name="newbodycontent"></a><span data-ttu-id="3adaf-103">NewBodyContent</span><span class="sxs-lookup"><span data-stu-id="3adaf-103">NewBodyContent</span></span>

<span data-ttu-id="3adaf-104">O elemento **NewBodyContent** representa o novo conteúdo do corpo de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="3adaf-104">The **NewBodyContent** element represents the new body content of a message.</span></span> 
  
```xml
<NewBodyContent BodyType=""/>
```

 <span data-ttu-id="3adaf-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="3adaf-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3adaf-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="3adaf-106">Attributes and elements</span></span>

<span data-ttu-id="3adaf-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3adaf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3adaf-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3adaf-108">Attributes</span></span>

|<span data-ttu-id="3adaf-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="3adaf-109">**Attribute**</span></span>|<span data-ttu-id="3adaf-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3adaf-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3adaf-111">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="3adaf-111">**BodyType**</span></span> <br/> |<span data-ttu-id="3adaf-112">Representa o conteúdo real do corpo de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="3adaf-112">Represents the actual body content of a message.</span></span>  <br/> |
   
#### <a name="bodytype-attribute"></a><span data-ttu-id="3adaf-113">Atributo BodyType</span><span class="sxs-lookup"><span data-stu-id="3adaf-113">BodyType Attribute</span></span>

|<span data-ttu-id="3adaf-114">**Valor**</span><span class="sxs-lookup"><span data-stu-id="3adaf-114">**Value**</span></span>|<span data-ttu-id="3adaf-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3adaf-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3adaf-116">**HTML**</span><span class="sxs-lookup"><span data-stu-id="3adaf-116">**HTML**</span></span> <br/> |<span data-ttu-id="3adaf-117">Converte todos os corpos em HTML.</span><span class="sxs-lookup"><span data-stu-id="3adaf-117">Converts all bodies to HTML.</span></span>  <br/> |
|<span data-ttu-id="3adaf-118">**Text**</span><span class="sxs-lookup"><span data-stu-id="3adaf-118">**Text**</span></span> <br/> |<span data-ttu-id="3adaf-119">Converte todos os corpos em texto sem formatação.</span><span class="sxs-lookup"><span data-stu-id="3adaf-119">Converts all bodies to plain text.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="3adaf-120">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3adaf-120">Child elements</span></span>

<span data-ttu-id="3adaf-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3adaf-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3adaf-122">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3adaf-122">Parent elements</span></span>

|<span data-ttu-id="3adaf-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3adaf-123">**Element**</span></span>|<span data-ttu-id="3adaf-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3adaf-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3adaf-125">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="3adaf-125">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="3adaf-126">Contém uma resposta para o remetente de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3adaf-126">Contains a reply to the sender of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3adaf-127">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="3adaf-127">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="3adaf-128">Contém uma resposta para o remetente e todos os destinatários identificados de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3adaf-128">Contains a reply to the sender and all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3adaf-129">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="3adaf-129">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="3adaf-130">Contém um item de repositório do Exchange para encaminhar aos destinatários.</span><span class="sxs-lookup"><span data-stu-id="3adaf-130">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="3adaf-131">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="3adaf-131">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="3adaf-132">Representa o objeto Response que é usado para cancelar uma reunião.</span><span class="sxs-lookup"><span data-stu-id="3adaf-132">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="3adaf-133">PostReplyItem</span><span class="sxs-lookup"><span data-stu-id="3adaf-133">PostReplyItem</span></span>](postreplyitem.md) <br/> |<span data-ttu-id="3adaf-134">Contém uma resposta a um item de postagem.</span><span class="sxs-lookup"><span data-stu-id="3adaf-134">Contains a reply to a post item.</span></span> <span data-ttu-id="3adaf-135">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="3adaf-135">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3adaf-136">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="3adaf-136">Text value</span></span>

<span data-ttu-id="3adaf-137">O valor de texto representa o novo conteúdo do corpo de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="3adaf-137">The text value represents the new body content of a message.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3adaf-138">Comentários</span><span class="sxs-lookup"><span data-stu-id="3adaf-138">Remarks</span></span>

<span data-ttu-id="3adaf-139">O esquema que descreve este elemento está localizado no diretório virtual do EWS do servidor Exchange que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="3adaf-139">The schema that describes this element is located in the EWS virtual directory of the Exchange server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3adaf-140">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="3adaf-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3adaf-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="3adaf-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3adaf-142">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3adaf-142">Schema Name</span></span>  <br/> |<span data-ttu-id="3adaf-143">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3adaf-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="3adaf-144">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3adaf-144">Validation File</span></span>  <br/> |<span data-ttu-id="3adaf-145">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="3adaf-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3adaf-146">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3adaf-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="3adaf-147">False</span><span class="sxs-lookup"><span data-stu-id="3adaf-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3adaf-148">Confira também</span><span class="sxs-lookup"><span data-stu-id="3adaf-148">See also</span></span>



- [<span data-ttu-id="3adaf-149">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3adaf-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

