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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751223"
---
# <a name="attachmentshape"></a><span data-ttu-id="0bc25-103">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="0bc25-103">AttachmentShape</span></span>

<span data-ttu-id="0bc25-104">O elemento **AttachmentShape** identifica propriedades adicionais para retornar em resposta a uma solicitação de [GetAttachment](getattachment.md) .</span><span class="sxs-lookup"><span data-stu-id="0bc25-104">The **AttachmentShape** element identifies additional properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span> 
  
- [<span data-ttu-id="0bc25-105">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="0bc25-105">GetAttachment</span></span>](getattachment.md)
  
- [<span data-ttu-id="0bc25-106">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="0bc25-106">AttachmentShape</span></span>](attachmentshape.md)
  
```xml
<AttachmentShape>
   <IncludeMimeContent/>
   <BodyType/>
   <FilterHtmlContent/>
   <AdditionalProperties/>
</AttachmentShape>
```

 <span data-ttu-id="0bc25-107">**AttachmentResponseShapeType**</span><span class="sxs-lookup"><span data-stu-id="0bc25-107">**AttachmentResponseShapeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0bc25-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="0bc25-108">Attributes and elements</span></span>

<span data-ttu-id="0bc25-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0bc25-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0bc25-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="0bc25-110">Attributes</span></span>

<span data-ttu-id="0bc25-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0bc25-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0bc25-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0bc25-112">Child elements</span></span>

|<span data-ttu-id="0bc25-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0bc25-113">**Element**</span></span>|<span data-ttu-id="0bc25-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0bc25-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0bc25-115">IncludeMimeContent</span><span class="sxs-lookup"><span data-stu-id="0bc25-115">IncludeMimeContent</span></span>](includemimecontent.md) <br/> |<span data-ttu-id="0bc25-116">Especifica se o conteúdo de email extensões MIME (Multipurpose Internet) de um item ou de um anexo é retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="0bc25-116">Specifies whether the Multipurpose Internet Mail Extensions (MIME) content of an item or attachment is returned in the response.</span></span> <span data-ttu-id="0bc25-117">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="0bc25-117">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="0bc25-118">BodyType</span><span class="sxs-lookup"><span data-stu-id="0bc25-118">BodyType</span></span>](bodytype.md) <br/> |<span data-ttu-id="0bc25-119">Identifica como o corpo de texto é formatado na resposta.</span><span class="sxs-lookup"><span data-stu-id="0bc25-119">Identifies how the body text is formatted in the response.</span></span> <span data-ttu-id="0bc25-120">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="0bc25-120">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="0bc25-121">FilterHtmlContent</span><span class="sxs-lookup"><span data-stu-id="0bc25-121">FilterHtmlContent</span></span>](filterhtmlcontent.md) <br/> |<span data-ttu-id="0bc25-122">Especifica se o conteúdo potencialmente não seguro de HTML é filtrado de um anexo.</span><span class="sxs-lookup"><span data-stu-id="0bc25-122">Specifies whether potentially unsafe HTML content is filtered from an attachment.</span></span> <span data-ttu-id="0bc25-123">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="0bc25-123">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="0bc25-124">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="0bc25-124">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="0bc25-125">Identifica as propriedades adicionais para retornar em uma resposta.</span><span class="sxs-lookup"><span data-stu-id="0bc25-125">Identifies additional properties to return in a response.</span></span> <span data-ttu-id="0bc25-126">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="0bc25-126">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0bc25-127">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0bc25-127">Parent elements</span></span>

|<span data-ttu-id="0bc25-128">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0bc25-128">**Element**</span></span>|<span data-ttu-id="0bc25-129">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0bc25-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0bc25-130">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="0bc25-130">GetAttachment</span></span>](getattachment.md) <br/> |<span data-ttu-id="0bc25-131">O elemento que define uma solicitação para fazer um anexo a partir de uma caixa de correio no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0bc25-131">The element that defines a request to get an attachment from a mailbox in the Exchange store.</span></span>  <br/> <span data-ttu-id="0bc25-132">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="0bc25-132">The following is the XPath expression to this element:</span></span>  <br/>  `/GetAttachment` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0bc25-133">Text value</span><span class="sxs-lookup"><span data-stu-id="0bc25-133">Text value</span></span>

<span data-ttu-id="0bc25-134">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0bc25-134">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0bc25-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="0bc25-135">Remarks</span></span>

<span data-ttu-id="0bc25-136">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0bc25-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0bc25-137">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="0bc25-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0bc25-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="0bc25-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0bc25-139">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0bc25-139">Schema Name</span></span>  <br/> |<span data-ttu-id="0bc25-140">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="0bc25-140">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0bc25-141">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0bc25-141">Validation File</span></span>  <br/> |<span data-ttu-id="0bc25-142">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0bc25-142">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0bc25-143">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0bc25-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="0bc25-144">False</span><span class="sxs-lookup"><span data-stu-id="0bc25-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0bc25-145">Ver também</span><span class="sxs-lookup"><span data-stu-id="0bc25-145">See also</span></span>

- [<span data-ttu-id="0bc25-146">Operação GetAttachment</span><span class="sxs-lookup"><span data-stu-id="0bc25-146">GetAttachment operation</span></span>](getattachment-operation.md)
- [<span data-ttu-id="0bc25-147">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0bc25-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

