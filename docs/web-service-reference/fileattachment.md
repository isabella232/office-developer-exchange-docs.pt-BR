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
description: O elemento fileattachment representa um arquivo anexado a um item no repositório do Exchange.
ms.openlocfilehash: db9b541fb2527ae3c09cbdb33bedea7fb215bd30
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461013"
---
# <a name="fileattachment"></a><span data-ttu-id="aab99-103">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="aab99-103">FileAttachment</span></span>

<span data-ttu-id="aab99-104">O elemento **Fileattachment** representa um arquivo anexado a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="aab99-104">The **FileAttachment** element represents a file that is attached to an item in the Exchange store.</span></span> 
  
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

 <span data-ttu-id="aab99-105">**FileAttachmentType**</span><span class="sxs-lookup"><span data-stu-id="aab99-105">**FileAttachmentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aab99-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="aab99-106">Attributes and elements</span></span>

<span data-ttu-id="aab99-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="aab99-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aab99-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="aab99-108">Attributes</span></span>

<span data-ttu-id="aab99-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="aab99-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aab99-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="aab99-110">Child elements</span></span>

|<span data-ttu-id="aab99-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="aab99-111">**Element**</span></span>|<span data-ttu-id="aab99-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="aab99-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aab99-113">Attachmentid</span><span class="sxs-lookup"><span data-stu-id="aab99-113">AttachmentId</span></span>](attachmentid.md) <br/> |<span data-ttu-id="aab99-114">Identifica o anexo de arquivo.</span><span class="sxs-lookup"><span data-stu-id="aab99-114">Identifies the file attachment.</span></span>  <br/> |
|[<span data-ttu-id="aab99-115">Nome (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="aab99-115">Name (AttachmentType)</span></span>](name-attachmenttype.md) <br/> |<span data-ttu-id="aab99-116">Representa o nome do anexo.</span><span class="sxs-lookup"><span data-stu-id="aab99-116">Represents the name of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="aab99-117">ContentType</span><span class="sxs-lookup"><span data-stu-id="aab99-117">ContentType</span></span>](contenttype.md) <br/> |<span data-ttu-id="aab99-118">Descreve o tipo de MIME (Multipurpose Internet Mail Extensions) do conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="aab99-118">Describes the Multipurpose Internet Mail Extensions (MIME) type of the attachment content.</span></span>  <br/> |
|[<span data-ttu-id="aab99-119">ContentId</span><span class="sxs-lookup"><span data-stu-id="aab99-119">ContentId</span></span>](contentid.md) <br/> |<span data-ttu-id="aab99-120">Representa um identificador para o conteúdo de um anexo.</span><span class="sxs-lookup"><span data-stu-id="aab99-120">Represents an identifier for the contents of an attachment.</span></span> <span data-ttu-id="aab99-121">[ContentId](contentid.md) pode ser definido como qualquer valor de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="aab99-121">[ContentId](contentid.md) can be set to any string value.</span></span> <span data-ttu-id="aab99-122">Os aplicativos podem usar [ContentId](contentid.md) para implementar seus próprios mecanismos de identificação.</span><span class="sxs-lookup"><span data-stu-id="aab99-122">Applications can use [ContentId](contentid.md) to implement their own identification mechanisms.</span></span>  <br/> |
|[<span data-ttu-id="aab99-123">ContentLocation</span><span class="sxs-lookup"><span data-stu-id="aab99-123">ContentLocation</span></span>](contentlocation.md) <br/> |<span data-ttu-id="aab99-124">Contém o URI (Uniform Resource Identifier) que corresponde ao local do conteúdo do anexo.</span><span class="sxs-lookup"><span data-stu-id="aab99-124">Contains the Uniform Resource Identifier (URI) that corresponds to the location of the content of the attachment.</span></span>  <br/> |
|[<span data-ttu-id="aab99-125">Tamanho</span><span class="sxs-lookup"><span data-stu-id="aab99-125">Size</span></span>](size.md) <br/> |<span data-ttu-id="aab99-126">Representa o tamanho em bytes do anexo de arquivo.</span><span class="sxs-lookup"><span data-stu-id="aab99-126">Represents the size in bytes of the file attachment.</span></span>  <br/> |
|[<span data-ttu-id="aab99-127">LastModifiedTime</span><span class="sxs-lookup"><span data-stu-id="aab99-127">LastModifiedTime</span></span>](lastmodifiedtime.md) <br/> |<span data-ttu-id="aab99-128">Representa quando o anexo de arquivo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="aab99-128">Represents when the file attachment was last modified.</span></span>  <br/> |
|[<span data-ttu-id="aab99-129">IsInline</span><span class="sxs-lookup"><span data-stu-id="aab99-129">IsInline</span></span>](isinline.md) <br/> |<span data-ttu-id="aab99-130">Indica se o anexo aparece embutido em um item.</span><span class="sxs-lookup"><span data-stu-id="aab99-130">Represents whether the attachment appears inline within an item.</span></span>  <br/> |
|[<span data-ttu-id="aab99-131">IsContactPhoto</span><span class="sxs-lookup"><span data-stu-id="aab99-131">IsContactPhoto</span></span>](iscontactphoto.md) <br/> |<span data-ttu-id="aab99-132">Indica se o anexo de arquivo é uma imagem de contato.</span><span class="sxs-lookup"><span data-stu-id="aab99-132">Indicates whether the file attachment is a contact picture.</span></span>  <br/> |
|[<span data-ttu-id="aab99-133">Conteúdo</span><span class="sxs-lookup"><span data-stu-id="aab99-133">Content</span></span>](content.md) <br/> |<span data-ttu-id="aab99-134">Contém o conteúdo codificado em base64 do anexo de arquivo.</span><span class="sxs-lookup"><span data-stu-id="aab99-134">Contains the Base64-encoded contents of the file attachment.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aab99-135">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="aab99-135">Parent elements</span></span>

|<span data-ttu-id="aab99-136">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="aab99-136">**Element**</span></span>|<span data-ttu-id="aab99-137">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="aab99-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aab99-138">Anexos</span><span class="sxs-lookup"><span data-stu-id="aab99-138">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="aab99-139">Contém os itens ou arquivos anexados a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="aab99-139">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="aab99-140">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="aab99-140">Text value</span></span>

<span data-ttu-id="aab99-141">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="aab99-141">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="aab99-142">Comentários</span><span class="sxs-lookup"><span data-stu-id="aab99-142">Remarks</span></span>

<span data-ttu-id="aab99-143">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="aab99-143">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aab99-144">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="aab99-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aab99-145">Namespace</span><span class="sxs-lookup"><span data-stu-id="aab99-145">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="aab99-146">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="aab99-146">Schema name</span></span>  <br/> |<span data-ttu-id="aab99-147">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="aab99-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="aab99-148">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="aab99-148">Validation file</span></span>  <br/> |<span data-ttu-id="aab99-149">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="aab99-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="aab99-150">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="aab99-150">Can be empty</span></span>  <br/> |<span data-ttu-id="aab99-151">False</span><span class="sxs-lookup"><span data-stu-id="aab99-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aab99-152">Confira também</span><span class="sxs-lookup"><span data-stu-id="aab99-152">See also</span></span>



- [<span data-ttu-id="aab99-153">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="aab99-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

