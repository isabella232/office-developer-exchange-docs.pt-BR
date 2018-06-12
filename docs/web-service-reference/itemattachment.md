---
title: ItemAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemAttachment
api_type:
- schema
ms.assetid: 089ee599-f45e-46f5-a18a-5cfb3d2851ff
description: O elemento ItemAttachment representa um item do Exchange que está anexado a outro item do Exchange.
ms.openlocfilehash: 87e0331664f1fdf8857afc78500014d138f05401
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824137"
---
# <a name="itemattachment"></a><span data-ttu-id="ac440-103">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="ac440-103">ItemAttachment</span></span>

<span data-ttu-id="ac440-104">O elemento **ItemAttachment** representa um item do Exchange que está anexado a outro item do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ac440-104">The **ItemAttachment** element represents an Exchange item that is attached to another Exchange item.</span></span> 
  
```xml
<ItemAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <Item/>
</ItemAttachment>
```

 <span data-ttu-id="ac440-105">**ItemAttachmentType**</span><span class="sxs-lookup"><span data-stu-id="ac440-105">**ItemAttachmentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ac440-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ac440-106">Attributes and elements</span></span>

<span data-ttu-id="ac440-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ac440-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ac440-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ac440-108">Attributes</span></span>

<span data-ttu-id="ac440-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ac440-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ac440-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ac440-110">Child elements</span></span>

|<span data-ttu-id="ac440-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ac440-111">**Element**</span></span>|<span data-ttu-id="ac440-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ac440-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ac440-113">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="ac440-113">AttachmentId</span></span>](attachmentid.md) <br/> |<span data-ttu-id="ac440-114">Identifica o anexo.</span><span class="sxs-lookup"><span data-stu-id="ac440-114">Identifies the attachment.</span></span>  <br/> |
|[<span data-ttu-id="ac440-115">Nome (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="ac440-115">Name (AttachmentType)</span></span>](name-attachmenttype.md) <br/> |<span data-ttu-id="ac440-116">Representa o nome do anexo.</span><span class="sxs-lookup"><span data-stu-id="ac440-116">Represents the name of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="ac440-117">ContentType</span><span class="sxs-lookup"><span data-stu-id="ac440-117">ContentType</span></span>](contenttype.md) <br/> |<span data-ttu-id="ac440-118">Descreve o tipo de email extensões MIME (Multipurpose Internet) do conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="ac440-118">Describes the Multipurpose Internet Mail Extensions (MIME) type of the attachment content.</span></span>  <br/> |
|[<span data-ttu-id="ac440-119">ContentId</span><span class="sxs-lookup"><span data-stu-id="ac440-119">ContentId</span></span>](contentid.md) <br/> |<span data-ttu-id="ac440-120">Representa um identificador para o conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="ac440-120">Represents an identifier to the contents of the attachment.</span></span> <span data-ttu-id="ac440-121">[ContentId](contentid.md) pode ser definido como qualquer valor de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="ac440-121">[ContentId](contentid.md) can be set to any string value.</span></span> <span data-ttu-id="ac440-122">Aplicativos podem usar [ContentId](contentid.md) implementar seus próprios mecanismos de identificação.</span><span class="sxs-lookup"><span data-stu-id="ac440-122">Applications can use [ContentId](contentid.md) to implement their own identification mechanisms.</span></span>  <br/> |
|[<span data-ttu-id="ac440-123">ContentLocation</span><span class="sxs-lookup"><span data-stu-id="ac440-123">ContentLocation</span></span>](contentlocation.md) <br/> |<span data-ttu-id="ac440-124">Contém o identificador de URI (Uniform Resource) que corresponde ao local do conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="ac440-124">Contains the Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="ac440-125">Size</span><span class="sxs-lookup"><span data-stu-id="ac440-125">Size</span></span>](size.md) <br/> |<span data-ttu-id="ac440-126">Representa o tamanho em bytes de arquivo do anexo.</span><span class="sxs-lookup"><span data-stu-id="ac440-126">Represents the size in bytes of the file attachment.</span></span>  <br/> |
|[<span data-ttu-id="ac440-127">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="ac440-127">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="ac440-128">Representa quando o anexo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="ac440-128">Represents when the attachment was last modified.</span></span>  <br/> |
|[<span data-ttu-id="ac440-129">IsInline</span><span class="sxs-lookup"><span data-stu-id="ac440-129">IsInline</span></span>](isinline.md) <br/> |<span data-ttu-id="ac440-130">Indica se o anexo é exibido embutida dentro de um item.</span><span class="sxs-lookup"><span data-stu-id="ac440-130">Represents whether the attachment appears inline within an item.</span></span>  <br/> |
|[<span data-ttu-id="ac440-131">1.1</span><span class="sxs-lookup"><span data-stu-id="ac440-131">Item</span></span>](item.md) <br/> |<span data-ttu-id="ac440-132">Representa um anexo de item genérico do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ac440-132">Represents a generic Exchange item attachment.</span></span>  <br/> |
|[<span data-ttu-id="ac440-133">Mensagem</span><span class="sxs-lookup"><span data-stu-id="ac440-133">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ac440-134">Representa um anexo de mensagem de email do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ac440-134">Represents an Exchange e-mail message attachment.</span></span>  <br/> |
|[<span data-ttu-id="ac440-135">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="ac440-135">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="ac440-136">Representa um anexo de item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ac440-136">Represents an Exchange calendar item attachment.</span></span>  <br/> |
|[<span data-ttu-id="ac440-137">Contato</span><span class="sxs-lookup"><span data-stu-id="ac440-137">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="ac440-138">Representa um anexo de item de contato do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ac440-138">Represents an Exchange contact item attachment.</span></span>  <br/> |
|[<span data-ttu-id="ac440-139">Task</span><span class="sxs-lookup"><span data-stu-id="ac440-139">Task</span></span>](task.md) <br/> |<span data-ttu-id="ac440-140">Representa um anexo de tarefa do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ac440-140">Represents an Exchange task attachment.</span></span>  <br/> |
|[<span data-ttu-id="ac440-141">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="ac440-141">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="ac440-142">Representa uma reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ac440-142">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ac440-143">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="ac440-143">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="ac440-144">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ac440-144">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ac440-145">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="ac440-145">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="ac440-146">Representa uma resposta de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ac440-146">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ac440-147">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="ac440-147">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="ac440-148">Representa o cancelamento da reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ac440-148">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ac440-149">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ac440-149">Parent elements</span></span>

|<span data-ttu-id="ac440-150">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ac440-150">**Element**</span></span>|<span data-ttu-id="ac440-151">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ac440-151">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ac440-152">Anexos</span><span class="sxs-lookup"><span data-stu-id="ac440-152">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ac440-153">Contém os arquivos que estejam anexados a um item no armazenamento do Exchange e/ou itens.</span><span class="sxs-lookup"><span data-stu-id="ac440-153">Contains the items and/or files that are attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ac440-154">Text value</span><span class="sxs-lookup"><span data-stu-id="ac440-154">Text value</span></span>

<span data-ttu-id="ac440-155">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ac440-155">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ac440-156">Comentários</span><span class="sxs-lookup"><span data-stu-id="ac440-156">Remarks</span></span>

<span data-ttu-id="ac440-157">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ac440-157">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ac440-158">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ac440-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ac440-159">Namespace</span><span class="sxs-lookup"><span data-stu-id="ac440-159">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ac440-160">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ac440-160">Schema Name</span></span>  <br/> |<span data-ttu-id="ac440-161">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ac440-161">Types schema</span></span>  <br/> |
|<span data-ttu-id="ac440-162">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ac440-162">Validation File</span></span>  <br/> |<span data-ttu-id="ac440-163">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ac440-163">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ac440-164">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ac440-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="ac440-165">False</span><span class="sxs-lookup"><span data-stu-id="ac440-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ac440-166">Ver também</span><span class="sxs-lookup"><span data-stu-id="ac440-166">See also</span></span>



- [<span data-ttu-id="ac440-167">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ac440-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
