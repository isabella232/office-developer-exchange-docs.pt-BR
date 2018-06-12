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
description: O elemento AttachmentShape identifica propriedades adicionais para retornar em resposta a uma solicitação de GetAttachment.
ms.openlocfilehash: dc6769faa5fd28ce31b796f86c507aec54abff7a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751223"
---
# <a name="attachmentshape"></a><span data-ttu-id="e2521-103">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="e2521-103">AttachmentShape</span></span>

<span data-ttu-id="e2521-104">O elemento **AttachmentShape** identifica propriedades adicionais para retornar em resposta a uma solicitação de [GetAttachment](getattachment.md) .</span><span class="sxs-lookup"><span data-stu-id="e2521-104">The **AttachmentShape** element identifies additional properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span> 
  
- [<span data-ttu-id="e2521-105">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="e2521-105">GetAttachment</span></span>](getattachment.md)
  
- [<span data-ttu-id="e2521-106">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="e2521-106">AttachmentShape</span></span>](attachmentshape.md)
  
```xml
<AttachmentShape>
   <IncludeMimeContent/>
   <BodyType/>
   <FilterHtmlContent/>
   <AdditionalProperties/>
</AttachmentShape>
```

 <span data-ttu-id="e2521-107">**AttachmentResponseShapeType**</span><span class="sxs-lookup"><span data-stu-id="e2521-107">**AttachmentResponseShapeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e2521-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e2521-108">Attributes and elements</span></span>

<span data-ttu-id="e2521-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e2521-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e2521-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="e2521-110">Attributes</span></span>

<span data-ttu-id="e2521-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e2521-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e2521-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e2521-112">Child elements</span></span>

|<span data-ttu-id="e2521-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e2521-113">**Element**</span></span>|<span data-ttu-id="e2521-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e2521-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e2521-115">IncludeMimeContent</span><span class="sxs-lookup"><span data-stu-id="e2521-115">IncludeMimeContent</span></span>](includemimecontent.md) <br/> |<span data-ttu-id="e2521-116">Especifica se o conteúdo de email extensões MIME (Multipurpose Internet) de um item ou de um anexo é retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="e2521-116">Specifies whether the Multipurpose Internet Mail Extensions (MIME) content of an item or attachment is returned in the response.</span></span> <span data-ttu-id="e2521-117">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="e2521-117">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e2521-118">BodyType</span><span class="sxs-lookup"><span data-stu-id="e2521-118">BodyType</span></span>](bodytype.md) <br/> |<span data-ttu-id="e2521-119">Identifica como o corpo de texto é formatado na resposta.</span><span class="sxs-lookup"><span data-stu-id="e2521-119">Identifies how the body text is formatted in the response.</span></span> <span data-ttu-id="e2521-120">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="e2521-120">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e2521-121">FilterHtmlContent</span><span class="sxs-lookup"><span data-stu-id="e2521-121">FilterHtmlContent</span></span>](filterhtmlcontent.md) <br/> |<span data-ttu-id="e2521-122">Especifica se o conteúdo potencialmente não seguro de HTML é filtrado de um anexo.</span><span class="sxs-lookup"><span data-stu-id="e2521-122">Specifies whether potentially unsafe HTML content is filtered from an attachment.</span></span> <span data-ttu-id="e2521-123">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="e2521-123">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="e2521-124">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="e2521-124">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="e2521-125">Identifica as propriedades adicionais para retornar em uma resposta.</span><span class="sxs-lookup"><span data-stu-id="e2521-125">Identifies additional properties to return in a response.</span></span> <span data-ttu-id="e2521-126">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="e2521-126">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e2521-127">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e2521-127">Parent elements</span></span>

|<span data-ttu-id="e2521-128">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e2521-128">**Element**</span></span>|<span data-ttu-id="e2521-129">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e2521-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e2521-130">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="e2521-130">GetAttachment</span></span>](getattachment.md) <br/> |<span data-ttu-id="e2521-131">O elemento que define uma solicitação para fazer um anexo a partir de uma caixa de correio no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e2521-131">The element that defines a request to get an attachment from a mailbox in the Exchange store.</span></span>  <br/> <span data-ttu-id="e2521-132">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="e2521-132">The following is the XPath expression to this element:</span></span>  <br/>  `/GetAttachment` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e2521-133">Text value</span><span class="sxs-lookup"><span data-stu-id="e2521-133">Text value</span></span>

<span data-ttu-id="e2521-134">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e2521-134">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e2521-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="e2521-135">Remarks</span></span>

<span data-ttu-id="e2521-136">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e2521-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e2521-137">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e2521-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e2521-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="e2521-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e2521-139">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e2521-139">Schema Name</span></span>  <br/> |<span data-ttu-id="e2521-140">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="e2521-140">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e2521-141">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e2521-141">Validation File</span></span>  <br/> |<span data-ttu-id="e2521-142">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e2521-142">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e2521-143">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e2521-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="e2521-144">False</span><span class="sxs-lookup"><span data-stu-id="e2521-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e2521-145">Ver também</span><span class="sxs-lookup"><span data-stu-id="e2521-145">See also</span></span>

- [<span data-ttu-id="e2521-146">Operação GetAttachment</span><span class="sxs-lookup"><span data-stu-id="e2521-146">GetAttachment operation</span></span>](getattachment-operation.md)
- [<span data-ttu-id="e2521-147">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e2521-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

