---
title: GetAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetAttachment
api_type:
- schema
ms.assetid: 9443cf96-b451-4530-b868-490dff798673
description: O elemento GetAttachment é o elemento raiz em uma solicitação para obter um anexo do armazenamento do Exchange.
ms.openlocfilehash: fb639c86a0654e8f9e9601310f7c2f5b0fc7d729
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752408"
---
# <a name="getattachment"></a><span data-ttu-id="ca94d-103">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="ca94d-103">GetAttachment</span></span>

<span data-ttu-id="ca94d-104">O elemento **GetAttachment** é o elemento raiz em uma solicitação para obter um anexo do armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ca94d-104">The **GetAttachment** element is the root element in a request to get an attachment from the Exchange store.</span></span> 
  
```xml
<GetAttachment>
   <AttachmentShape/>
   <AttachmentIds/>
</GetAttachment>
```

 <span data-ttu-id="ca94d-105">**GetAttachmentType**</span><span class="sxs-lookup"><span data-stu-id="ca94d-105">**GetAttachmentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ca94d-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ca94d-106">Attributes and elements</span></span>

<span data-ttu-id="ca94d-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ca94d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ca94d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ca94d-108">Attributes</span></span>

<span data-ttu-id="ca94d-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ca94d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ca94d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ca94d-110">Child elements</span></span>

|<span data-ttu-id="ca94d-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ca94d-111">**Element**</span></span>|<span data-ttu-id="ca94d-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ca94d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ca94d-113">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="ca94d-113">AttachmentShape</span></span>](attachmentshape.md) <br/> |<span data-ttu-id="ca94d-114">Identifica as propriedades de item estendido adicional para retornar em resposta a uma solicitação de [GetAttachment](getattachment.md) .</span><span class="sxs-lookup"><span data-stu-id="ca94d-114">Identifies additional extended item properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span> <span data-ttu-id="ca94d-115">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="ca94d-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="ca94d-116">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="ca94d-116">AttachmentIds</span></span>](attachmentids.md) <br/> |<span data-ttu-id="ca94d-117">Contém uma matriz de identificadores de anexo.</span><span class="sxs-lookup"><span data-stu-id="ca94d-117">Contains an array of attachment identifiers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ca94d-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ca94d-118">Parent elements</span></span>

<span data-ttu-id="ca94d-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ca94d-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ca94d-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="ca94d-120">Remarks</span></span>

<span data-ttu-id="ca94d-121">O elemento [AttachmentShape](attachmentshape.md) não é necessário para identificar as propriedades retornadas na resposta.</span><span class="sxs-lookup"><span data-stu-id="ca94d-121">The [AttachmentShape](attachmentshape.md) element is not required to identify the properties returned in the response.</span></span> <span data-ttu-id="ca94d-122">A [operação GetAttachment](getattachment-operation.md) retorna o nome, ContentType, ContentId, ContentLocation e as propriedades de conteúdo de anexos de arquivo.</span><span class="sxs-lookup"><span data-stu-id="ca94d-122">The [GetAttachment operation](getattachment-operation.md) returns the Name, ContentType, ContentId, ContentLocation, and the Content properties for file attachments.</span></span> <span data-ttu-id="ca94d-123">Anexos de item, as propriedades retornadas são o nome, ContentType, ContentId, ContentLocation e todas as anexado propriedades do item.</span><span class="sxs-lookup"><span data-stu-id="ca94d-123">For item attachments, the returned properties are the Name, ContentType, ContentId, ContentLocation, and all the attached item's properties.</span></span> <span data-ttu-id="ca94d-124">Isso equivale a usar a forma de base AllProperties em uma solicitação de [GetItem](getitem.md) .</span><span class="sxs-lookup"><span data-stu-id="ca94d-124">This is equivalent to using the AllProperties base shape in a [GetItem](getitem.md) request.</span></span> 
  
<span data-ttu-id="ca94d-125">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="ca94d-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ca94d-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ca94d-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ca94d-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="ca94d-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ca94d-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ca94d-128">Schema Name</span></span>  <br/> |<span data-ttu-id="ca94d-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="ca94d-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ca94d-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ca94d-130">Validation File</span></span>  <br/> |<span data-ttu-id="ca94d-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ca94d-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ca94d-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ca94d-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="ca94d-133">False</span><span class="sxs-lookup"><span data-stu-id="ca94d-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ca94d-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="ca94d-134">See also</span></span>



[<span data-ttu-id="ca94d-135">Operação GetAttachment</span><span class="sxs-lookup"><span data-stu-id="ca94d-135">GetAttachment operation</span></span>](getattachment-operation.md)
  
[<span data-ttu-id="ca94d-136">GetAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="ca94d-136">GetAttachmentResponse</span></span>](getattachmentresponse.md)

