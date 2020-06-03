---
title: AttachmentShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttachmentShape
api_type:
- schema
ms.assetid: 734914b5-3a16-4744-90a5-741fd30c4676
description: O elemento AttachmentShape identifica propriedades adicionais para retornar em uma resposta a uma solicitação GetAttachment.
ms.openlocfilehash: e70fbaad0f649c5afdc151b777efef0f8927ba1c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529662"
---
# <a name="attachmentshape"></a><span data-ttu-id="904a8-103">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="904a8-103">AttachmentShape</span></span>

<span data-ttu-id="904a8-104">O elemento **AttachmentShape** identifica propriedades adicionais para retornar em uma resposta a uma solicitação [GetAttachment](getattachment.md) .</span><span class="sxs-lookup"><span data-stu-id="904a8-104">The **AttachmentShape** element identifies additional properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span> 
  
- [<span data-ttu-id="904a8-105">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="904a8-105">GetAttachment</span></span>](getattachment.md)
  
- [<span data-ttu-id="904a8-106">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="904a8-106">AttachmentShape</span></span>](attachmentshape.md)
  
```xml
<AttachmentShape>
   <IncludeMimeContent/>
   <BodyType/>
   <FilterHtmlContent/>
   <AdditionalProperties/>
</AttachmentShape>
```

 <span data-ttu-id="904a8-107">**AttachmentResponseShapeType**</span><span class="sxs-lookup"><span data-stu-id="904a8-107">**AttachmentResponseShapeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="904a8-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="904a8-108">Attributes and elements</span></span>

<span data-ttu-id="904a8-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="904a8-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="904a8-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="904a8-110">Attributes</span></span>

<span data-ttu-id="904a8-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="904a8-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="904a8-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="904a8-112">Child elements</span></span>

|<span data-ttu-id="904a8-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="904a8-113">**Element**</span></span>|<span data-ttu-id="904a8-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="904a8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="904a8-115">IncludeMimeContent</span><span class="sxs-lookup"><span data-stu-id="904a8-115">IncludeMimeContent</span></span>](includemimecontent.md) <br/> |<span data-ttu-id="904a8-116">Especifica se o conteúdo MIME (Multipurpose Internet Mail Extensions) de um item ou anexo é retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="904a8-116">Specifies whether the Multipurpose Internet Mail Extensions (MIME) content of an item or attachment is returned in the response.</span></span> <span data-ttu-id="904a8-117">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="904a8-117">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="904a8-118">BodyType</span><span class="sxs-lookup"><span data-stu-id="904a8-118">BodyType</span></span>](bodytype.md) <br/> |<span data-ttu-id="904a8-119">Identifica como o corpo de texto é formatado na resposta.</span><span class="sxs-lookup"><span data-stu-id="904a8-119">Identifies how the body text is formatted in the response.</span></span> <span data-ttu-id="904a8-120">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="904a8-120">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="904a8-121">FilterHtmlContent</span><span class="sxs-lookup"><span data-stu-id="904a8-121">FilterHtmlContent</span></span>](filterhtmlcontent.md) <br/> |<span data-ttu-id="904a8-122">Especifica se o conteúdo HTML potencialmente não seguro é filtrado de um anexo.</span><span class="sxs-lookup"><span data-stu-id="904a8-122">Specifies whether potentially unsafe HTML content is filtered from an attachment.</span></span> <span data-ttu-id="904a8-123">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="904a8-123">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="904a8-124">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="904a8-124">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="904a8-125">Identifica propriedades adicionais a serem retornadas em uma resposta.</span><span class="sxs-lookup"><span data-stu-id="904a8-125">Identifies additional properties to return in a response.</span></span> <span data-ttu-id="904a8-126">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="904a8-126">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="904a8-127">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="904a8-127">Parent elements</span></span>

|<span data-ttu-id="904a8-128">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="904a8-128">**Element**</span></span>|<span data-ttu-id="904a8-129">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="904a8-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="904a8-130">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="904a8-130">GetAttachment</span></span>](getattachment.md) <br/> |<span data-ttu-id="904a8-131">O elemento que define uma solicitação para obter um anexo de uma caixa de correio no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="904a8-131">The element that defines a request to get an attachment from a mailbox in the Exchange store.</span></span>  <br/> <span data-ttu-id="904a8-132">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="904a8-132">The following is the XPath expression to this element:</span></span>  <br/>  `/GetAttachment` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="904a8-133">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="904a8-133">Text value</span></span>

<span data-ttu-id="904a8-134">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="904a8-134">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="904a8-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="904a8-135">Remarks</span></span>

<span data-ttu-id="904a8-136">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="904a8-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="904a8-137">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="904a8-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="904a8-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="904a8-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="904a8-139">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="904a8-139">Schema Name</span></span>  <br/> |<span data-ttu-id="904a8-140">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="904a8-140">Messages schema</span></span>  <br/> |
|<span data-ttu-id="904a8-141">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="904a8-141">Validation File</span></span>  <br/> |<span data-ttu-id="904a8-142">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="904a8-142">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="904a8-143">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="904a8-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="904a8-144">False</span><span class="sxs-lookup"><span data-stu-id="904a8-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="904a8-145">Confira também</span><span class="sxs-lookup"><span data-stu-id="904a8-145">See also</span></span>

- [<span data-ttu-id="904a8-146">Operação GetAttachment</span><span class="sxs-lookup"><span data-stu-id="904a8-146">GetAttachment operation</span></span>](getattachment-operation.md)
- [<span data-ttu-id="904a8-147">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="904a8-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

