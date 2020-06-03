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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466854"
---
# <a name="newbodycontent"></a><span data-ttu-id="b64e0-103">NewBodyContent</span><span class="sxs-lookup"><span data-stu-id="b64e0-103">NewBodyContent</span></span>

<span data-ttu-id="b64e0-104">O elemento **NewBodyContent** representa o novo conteúdo do corpo de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="b64e0-104">The **NewBodyContent** element represents the new body content of a message.</span></span> 
  
```xml
<NewBodyContent BodyType=""/>
```

 <span data-ttu-id="b64e0-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="b64e0-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b64e0-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b64e0-106">Attributes and elements</span></span>

<span data-ttu-id="b64e0-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b64e0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b64e0-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b64e0-108">Attributes</span></span>

|<span data-ttu-id="b64e0-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="b64e0-109">**Attribute**</span></span>|<span data-ttu-id="b64e0-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b64e0-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b64e0-111">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="b64e0-111">**BodyType**</span></span> <br/> |<span data-ttu-id="b64e0-112">Representa o conteúdo real do corpo de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="b64e0-112">Represents the actual body content of a message.</span></span>  <br/> |
   
#### <a name="bodytype-attribute"></a><span data-ttu-id="b64e0-113">Atributo BodyType</span><span class="sxs-lookup"><span data-stu-id="b64e0-113">BodyType Attribute</span></span>

|<span data-ttu-id="b64e0-114">**Valor**</span><span class="sxs-lookup"><span data-stu-id="b64e0-114">**Value**</span></span>|<span data-ttu-id="b64e0-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b64e0-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b64e0-116">**HTML**</span><span class="sxs-lookup"><span data-stu-id="b64e0-116">**HTML**</span></span> <br/> |<span data-ttu-id="b64e0-117">Converte todos os corpos em HTML.</span><span class="sxs-lookup"><span data-stu-id="b64e0-117">Converts all bodies to HTML.</span></span>  <br/> |
|<span data-ttu-id="b64e0-118">**Text**</span><span class="sxs-lookup"><span data-stu-id="b64e0-118">**Text**</span></span> <br/> |<span data-ttu-id="b64e0-119">Converte todos os corpos em texto sem formatação.</span><span class="sxs-lookup"><span data-stu-id="b64e0-119">Converts all bodies to plain text.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b64e0-120">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b64e0-120">Child elements</span></span>

<span data-ttu-id="b64e0-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b64e0-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b64e0-122">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b64e0-122">Parent elements</span></span>

|<span data-ttu-id="b64e0-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b64e0-123">**Element**</span></span>|<span data-ttu-id="b64e0-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b64e0-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b64e0-125">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="b64e0-125">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="b64e0-126">Contém uma resposta para o remetente de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b64e0-126">Contains a reply to the sender of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b64e0-127">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="b64e0-127">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="b64e0-128">Contém uma resposta para o remetente e todos os destinatários identificados de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b64e0-128">Contains a reply to the sender and all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b64e0-129">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="b64e0-129">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="b64e0-130">Contém um item de repositório do Exchange para encaminhar aos destinatários.</span><span class="sxs-lookup"><span data-stu-id="b64e0-130">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="b64e0-131">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="b64e0-131">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="b64e0-132">Representa o objeto Response que é usado para cancelar uma reunião.</span><span class="sxs-lookup"><span data-stu-id="b64e0-132">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="b64e0-133">PostReplyItem</span><span class="sxs-lookup"><span data-stu-id="b64e0-133">PostReplyItem</span></span>](postreplyitem.md) <br/> |<span data-ttu-id="b64e0-134">Contém uma resposta a um item de postagem.</span><span class="sxs-lookup"><span data-stu-id="b64e0-134">Contains a reply to a post item.</span></span> <span data-ttu-id="b64e0-135">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="b64e0-135">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b64e0-136">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="b64e0-136">Text value</span></span>

<span data-ttu-id="b64e0-137">O valor de texto representa o novo conteúdo do corpo de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="b64e0-137">The text value represents the new body content of a message.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b64e0-138">Comentários</span><span class="sxs-lookup"><span data-stu-id="b64e0-138">Remarks</span></span>

<span data-ttu-id="b64e0-139">O esquema que descreve este elemento está localizado no diretório virtual do EWS do servidor Exchange que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="b64e0-139">The schema that describes this element is located in the EWS virtual directory of the Exchange server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b64e0-140">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="b64e0-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b64e0-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="b64e0-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b64e0-142">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b64e0-142">Schema Name</span></span>  <br/> |<span data-ttu-id="b64e0-143">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b64e0-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="b64e0-144">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b64e0-144">Validation File</span></span>  <br/> |<span data-ttu-id="b64e0-145">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b64e0-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b64e0-146">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b64e0-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="b64e0-147">False</span><span class="sxs-lookup"><span data-stu-id="b64e0-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b64e0-148">Confira também</span><span class="sxs-lookup"><span data-stu-id="b64e0-148">See also</span></span>



- [<span data-ttu-id="b64e0-149">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b64e0-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

