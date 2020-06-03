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
description: O elemento item anexo representa um item do Exchange anexado a outro item do Exchange.
ms.openlocfilehash: c3a07fa091c05654a03cbff58fb20204c26c9061
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526435"
---
# <a name="itemattachment"></a><span data-ttu-id="b0f9b-103">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="b0f9b-103">ItemAttachment</span></span>

<span data-ttu-id="b0f9b-104">O elemento item **anexo** representa um item do Exchange anexado a outro item do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b0f9b-104">The **ItemAttachment** element represents an Exchange item that is attached to another Exchange item.</span></span> 
  
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
   <Message/>
</ItemAttachment>
```

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
   <CalendarItem/>
</ItemAttachment>
```

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
   <Contact/>
</ItemAttachment>
```

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
   <Task/>
</ItemAttachment>
```

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
   <MeetingMessage/>
</ItemAttachment>
```

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
   <MeetingRequest/>
</ItemAttachment>
```

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
   <MeetingResponse/>
</ItemAttachment>
```

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
   <MeetingCancellation/>
</ItemAttachment>
```

<span data-ttu-id="b0f9b-105">**Objectattachmenttype**</span><span class="sxs-lookup"><span data-stu-id="b0f9b-105">**ItemAttachmentType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b0f9b-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b0f9b-106">Attributes and elements</span></span>

<span data-ttu-id="b0f9b-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b0f9b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b0f9b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b0f9b-108">Attributes</span></span>

<span data-ttu-id="b0f9b-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b0f9b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b0f9b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b0f9b-110">Child elements</span></span>

|<span data-ttu-id="b0f9b-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b0f9b-111">**Element**</span></span>|<span data-ttu-id="b0f9b-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b0f9b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0f9b-113">Attachmentid</span><span class="sxs-lookup"><span data-stu-id="b0f9b-113">AttachmentId</span></span>](attachmentid.md) <br/> |<span data-ttu-id="b0f9b-114">Identifica o anexo.</span><span class="sxs-lookup"><span data-stu-id="b0f9b-114">Identifies the attachment.</span></span>  <br/> |
|[<span data-ttu-id="b0f9b-115">Nome (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="b0f9b-115">Name (AttachmentType)</span></span>](name-attachmenttype.md) <br/> |<span data-ttu-id="b0f9b-116">Representa o nome do anexo.</span><span class="sxs-lookup"><span data-stu-id="b0f9b-116">Represents the name of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="b0f9b-117">ContentType</span><span class="sxs-lookup"><span data-stu-id="b0f9b-117">ContentType</span></span>](contenttype.md) <br/> |<span data-ttu-id="b0f9b-118">Descreve o tipo de MIME (Multipurpose Internet Mail Extensions) do conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="b0f9b-118">Describes the Multipurpose Internet Mail Extensions (MIME) type of the attachment content.</span></span>  <br/> |
|[<span data-ttu-id="b0f9b-119">ContentId</span><span class="sxs-lookup"><span data-stu-id="b0f9b-119">ContentId</span></span>](contentid.md) <br/> |<span data-ttu-id="b0f9b-120">Representa um identificador para o conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="b0f9b-120">Represents an identifier to the contents of the attachment.</span></span> <span data-ttu-id="b0f9b-121">[ContentId](contentid.md) pode ser definido como qualquer valor de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="b0f9b-121">[ContentId](contentid.md) can be set to any string value.</span></span> <span data-ttu-id="b0f9b-122">Os aplicativos podem usar [ContentId](contentid.md) para implementar seus próprios mecanismos de identificação.</span><span class="sxs-lookup"><span data-stu-id="b0f9b-122">Applications can use [ContentId](contentid.md) to implement their own identification mechanisms.</span></span>  <br/> |
|[<span data-ttu-id="b0f9b-123">ContentLocation</span><span class="sxs-lookup"><span data-stu-id="b0f9b-123">ContentLocation</span></span>](contentlocation.md) <br/> |<span data-ttu-id="b0f9b-124">Contém o URI (Uniform Resource Identifier) que corresponde ao local do conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="b0f9b-124">Contains the Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="b0f9b-125">Tamanho</span><span class="sxs-lookup"><span data-stu-id="b0f9b-125">Size</span></span>](size.md) <br/> |<span data-ttu-id="b0f9b-126">Representa o tamanho em bytes do anexo de arquivo.</span><span class="sxs-lookup"><span data-stu-id="b0f9b-126">Represents the size in bytes of the file attachment.</span></span>  <br/> |
|[<span data-ttu-id="b0f9b-127">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="b0f9b-127">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="b0f9b-128">Representa quando o anexo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b0f9b-128">Represents when the attachment was last modified.</span></span>  <br/> |
|[<span data-ttu-id="b0f9b-129">IsInline</span><span class="sxs-lookup"><span data-stu-id="b0f9b-129">IsInline</span></span>](isinline.md) <br/> |<span data-ttu-id="b0f9b-130">Indica se o anexo aparece embutido em um item.</span><span class="sxs-lookup"><span data-stu-id="b0f9b-130">Represents whether the attachment appears inline within an item.</span></span>  <br/> |
|[<span data-ttu-id="b0f9b-131">Item</span><span class="sxs-lookup"><span data-stu-id="b0f9b-131">Item</span></span>](item.md) <br/> |<span data-ttu-id="b0f9b-132">Representa um anexo de item genérico do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b0f9b-132">Represents a generic Exchange item attachment.</span></span>  <br/> |
|[<span data-ttu-id="b0f9b-133">Mensagem</span><span class="sxs-lookup"><span data-stu-id="b0f9b-133">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="b0f9b-134">Representa um anexo de mensagem de email do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b0f9b-134">Represents an Exchange e-mail message attachment.</span></span>  <br/> |
|[<span data-ttu-id="b0f9b-135">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="b0f9b-135">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="b0f9b-136">Representa um anexo de item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b0f9b-136">Represents an Exchange calendar item attachment.</span></span>  <br/> |
|[<span data-ttu-id="b0f9b-137">Contato</span><span class="sxs-lookup"><span data-stu-id="b0f9b-137">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="b0f9b-138">Representa um anexo de item de contato do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b0f9b-138">Represents an Exchange contact item attachment.</span></span>  <br/> |
|[<span data-ttu-id="b0f9b-139">Tarefa</span><span class="sxs-lookup"><span data-stu-id="b0f9b-139">Task</span></span>](task.md) <br/> |<span data-ttu-id="b0f9b-140">Representa um anexo de tarefa do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b0f9b-140">Represents an Exchange task attachment.</span></span>  <br/> |
|[<span data-ttu-id="b0f9b-141">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="b0f9b-141">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="b0f9b-142">Representa uma reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b0f9b-142">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b0f9b-143">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="b0f9b-143">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="b0f9b-144">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b0f9b-144">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b0f9b-145">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="b0f9b-145">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="b0f9b-146">Representa uma resposta de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b0f9b-146">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b0f9b-147">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="b0f9b-147">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="b0f9b-148">Representa um cancelamento de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b0f9b-148">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b0f9b-149">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b0f9b-149">Parent elements</span></span>

|<span data-ttu-id="b0f9b-150">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b0f9b-150">**Element**</span></span>|<span data-ttu-id="b0f9b-151">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b0f9b-151">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0f9b-152">Anexos</span><span class="sxs-lookup"><span data-stu-id="b0f9b-152">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="b0f9b-153">Contém os itens e/ou arquivos anexados a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b0f9b-153">Contains the items and/or files that are attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b0f9b-154">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="b0f9b-154">Text value</span></span>

<span data-ttu-id="b0f9b-155">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b0f9b-155">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b0f9b-156">Comentários</span><span class="sxs-lookup"><span data-stu-id="b0f9b-156">Remarks</span></span>

<span data-ttu-id="b0f9b-157">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b0f9b-157">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b0f9b-158">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="b0f9b-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b0f9b-159">Namespace</span><span class="sxs-lookup"><span data-stu-id="b0f9b-159">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b0f9b-160">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b0f9b-160">Schema Name</span></span>  <br/> |<span data-ttu-id="b0f9b-161">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b0f9b-161">Types schema</span></span>  <br/> |
|<span data-ttu-id="b0f9b-162">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b0f9b-162">Validation File</span></span>  <br/> |<span data-ttu-id="b0f9b-163">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b0f9b-163">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b0f9b-164">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b0f9b-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="b0f9b-165">False</span><span class="sxs-lookup"><span data-stu-id="b0f9b-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b0f9b-166">Confira também</span><span class="sxs-lookup"><span data-stu-id="b0f9b-166">See also</span></span>

- [<span data-ttu-id="b0f9b-167">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b0f9b-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

