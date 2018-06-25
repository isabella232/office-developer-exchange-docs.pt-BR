---
title: FileAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FileAttachment
api_type:
- schema
ms.assetid: 3ecea174-73d1-47fd-8917-6065cef1d565
description: O elemento FileAttachment representa um arquivo anexado a um item no armazenamento do Exchange.
ms.openlocfilehash: 5ce7aef753313aa9430f640bb3c26f652b8c1c43
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752252"
---
# <a name="fileattachment"></a><span data-ttu-id="b7848-103">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="b7848-103">FileAttachment</span></span>

<span data-ttu-id="b7848-104">O elemento **FileAttachment** representa um arquivo anexado a um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b7848-104">The **FileAttachment** element represents a file that is attached to an item in the Exchange store.</span></span> 
  
```XML
<FileAttachment>
   <AttachmentId/>
   <Name/>
   <ContentType/>
   <ContentId/>
   <ContentLocation/>
   <Size/>
   <LastModifiedTime/>
   <IsInline/>
   <IsContactPhoto/>
   <Content/>
</FileAttachment>
```

 <span data-ttu-id="b7848-105">**FileAttachmentType**</span><span class="sxs-lookup"><span data-stu-id="b7848-105">**FileAttachmentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b7848-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b7848-106">Attributes and elements</span></span>

<span data-ttu-id="b7848-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b7848-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b7848-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b7848-108">Attributes</span></span>

<span data-ttu-id="b7848-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b7848-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b7848-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b7848-110">Child elements</span></span>

|<span data-ttu-id="b7848-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b7848-111">**Element**</span></span>|<span data-ttu-id="b7848-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b7848-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b7848-113">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="b7848-113">AttachmentId</span></span>](attachmentid.md) <br/> |<span data-ttu-id="b7848-114">Identifica o anexo de arquivo.</span><span class="sxs-lookup"><span data-stu-id="b7848-114">Identifies the file attachment.</span></span>  <br/> |
|[<span data-ttu-id="b7848-115">Nome (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="b7848-115">Name (AttachmentType)</span></span>](name-attachmenttype.md) <br/> |<span data-ttu-id="b7848-116">Representa o nome do anexo.</span><span class="sxs-lookup"><span data-stu-id="b7848-116">Represents the name of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="b7848-117">ContentType</span><span class="sxs-lookup"><span data-stu-id="b7848-117">ContentType</span></span>](contenttype.md) <br/> |<span data-ttu-id="b7848-118">Descreve o tipo de email extensões MIME (Multipurpose Internet) do conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="b7848-118">Describes the Multipurpose Internet Mail Extensions (MIME) type of the attachment content.</span></span>  <br/> |
|[<span data-ttu-id="b7848-119">ContentId</span><span class="sxs-lookup"><span data-stu-id="b7848-119">ContentId</span></span>](contentid.md) <br/> |<span data-ttu-id="b7848-120">Representa um identificador para o conteúdo de um anexo.</span><span class="sxs-lookup"><span data-stu-id="b7848-120">Represents an identifier for the contents of an attachment.</span></span> <span data-ttu-id="b7848-121">[ContentId](contentid.md) pode ser definido como qualquer valor de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="b7848-121">[ContentId](contentid.md) can be set to any string value.</span></span> <span data-ttu-id="b7848-122">Aplicativos podem usar [ContentId](contentid.md) implementar seus próprios mecanismos de identificação.</span><span class="sxs-lookup"><span data-stu-id="b7848-122">Applications can use [ContentId](contentid.md) to implement their own identification mechanisms.</span></span>  <br/> |
|[<span data-ttu-id="b7848-123">ContentLocation</span><span class="sxs-lookup"><span data-stu-id="b7848-123">ContentLocation</span></span>](contentlocation.md) <br/> |<span data-ttu-id="b7848-124">Contém o identificador de URI (Uniform Resource) que corresponde ao local do conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="b7848-124">Contains the Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="b7848-125">Size</span><span class="sxs-lookup"><span data-stu-id="b7848-125">Size</span></span>](size.md) <br/> |<span data-ttu-id="b7848-126">Representa o tamanho em bytes de arquivo do anexo.</span><span class="sxs-lookup"><span data-stu-id="b7848-126">Represents the size in bytes of the file attachment.</span></span>  <br/> |
|[<span data-ttu-id="b7848-127">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="b7848-127">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="b7848-128">Representa quando o anexo de arquivo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="b7848-128">Represents when the file attachment was last modified.</span></span>  <br/> |
|[<span data-ttu-id="b7848-129">IsInline</span><span class="sxs-lookup"><span data-stu-id="b7848-129">IsInline</span></span>](isinline.md) <br/> |<span data-ttu-id="b7848-130">Indica se o anexo é exibido embutida dentro de um item.</span><span class="sxs-lookup"><span data-stu-id="b7848-130">Represents whether the attachment appears inline within an item.</span></span>  <br/> |
|[<span data-ttu-id="b7848-131">IsContactPhoto</span><span class="sxs-lookup"><span data-stu-id="b7848-131">IsContactPhoto</span></span>](iscontactphoto.md) <br/> |<span data-ttu-id="b7848-132">Indica se o anexo de arquivo é uma imagem do contato.</span><span class="sxs-lookup"><span data-stu-id="b7848-132">Indicates whether the file attachment is a contact picture.</span></span>  <br/> |
|[<span data-ttu-id="b7848-133">Conteúdo</span><span class="sxs-lookup"><span data-stu-id="b7848-133">Content</span></span>](content.md) <br/> |<span data-ttu-id="b7848-134">Contém o conteúdo codificado na Base64 de arquivo do anexo.</span><span class="sxs-lookup"><span data-stu-id="b7848-134">Contains the Base64-encoded contents of the file attachment.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b7848-135">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b7848-135">Parent elements</span></span>

|<span data-ttu-id="b7848-136">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b7848-136">**Element**</span></span>|<span data-ttu-id="b7848-137">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b7848-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b7848-138">Anexos</span><span class="sxs-lookup"><span data-stu-id="b7848-138">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="b7848-139">Contém os itens ou arquivos que estejam anexados a um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b7848-139">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b7848-140">Text value</span><span class="sxs-lookup"><span data-stu-id="b7848-140">Text value</span></span>

<span data-ttu-id="b7848-141">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b7848-141">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b7848-142">Comentários</span><span class="sxs-lookup"><span data-stu-id="b7848-142">Remarks</span></span>

<span data-ttu-id="b7848-143">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b7848-143">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b7848-144">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b7848-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b7848-145">Namespace</span><span class="sxs-lookup"><span data-stu-id="b7848-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b7848-146">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b7848-146">Schema name</span></span>  <br/> |<span data-ttu-id="b7848-147">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b7848-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="b7848-148">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b7848-148">Validation file</span></span>  <br/> |<span data-ttu-id="b7848-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b7848-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b7848-150">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="b7848-150">Can be empty</span></span>  <br/> |<span data-ttu-id="b7848-151">False</span><span class="sxs-lookup"><span data-stu-id="b7848-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b7848-152">Ver também</span><span class="sxs-lookup"><span data-stu-id="b7848-152">See also</span></span>



- [<span data-ttu-id="b7848-153">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b7848-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

