---
title: AttachmentId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttachmentId
api_type:
- schema
ms.assetid: 55a5fd77-60d1-40fa-8144-770600cedc6a
description: O elemento AttachmentId identifica um anexo de arquivo ou item. Este elemento é usado nas respostas CreateAttachment.
ms.openlocfilehash: 2910503d1661ca3aaeeb4e319deb39f6b57c5c0a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751219"
---
# <a name="attachmentid"></a><span data-ttu-id="f810c-104">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="f810c-104">AttachmentId</span></span>

<span data-ttu-id="f810c-105">O elemento **AttachmentId** identifica um anexo de arquivo ou item.</span><span class="sxs-lookup"><span data-stu-id="f810c-105">The **AttachmentId** element identifies an item or file attachment.</span></span> <span data-ttu-id="f810c-106">Este elemento é usado nas respostas CreateAttachment.</span><span class="sxs-lookup"><span data-stu-id="f810c-106">This element is used in CreateAttachment responses.</span></span> 
  
```xml
<AttachmentId Id="" RootItemId="" RootItemChangeKey="" />
```

 <span data-ttu-id="f810c-107">**AttachmentIdType**</span><span class="sxs-lookup"><span data-stu-id="f810c-107">**AttachmentIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f810c-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f810c-108">Attributes and elements</span></span>

<span data-ttu-id="f810c-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f810c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f810c-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="f810c-110">Attributes</span></span>

|<span data-ttu-id="f810c-111">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="f810c-111">**Attribute**</span></span>|<span data-ttu-id="f810c-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f810c-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f810c-113">**ID de**</span><span class="sxs-lookup"><span data-stu-id="f810c-113">**Id**</span></span> <br/> |<span data-ttu-id="f810c-114">Identifica o identificador exclusivo do anexo.</span><span class="sxs-lookup"><span data-stu-id="f810c-114">Identifies the unique identifier of the attachment.</span></span>  <br/> |
|<span data-ttu-id="f810c-115">**RootItemId**</span><span class="sxs-lookup"><span data-stu-id="f810c-115">**RootItemId**</span></span> <br/> |<span data-ttu-id="f810c-116">Identifica o identificador exclusivo do item raiz repositório à qual o anexo está vinculado.</span><span class="sxs-lookup"><span data-stu-id="f810c-116">Identifies the unique identifier of the root store item to which the attachment is attached.</span></span>  <br/> |
|<span data-ttu-id="f810c-117">**RootItemChangeKey**</span><span class="sxs-lookup"><span data-stu-id="f810c-117">**RootItemChangeKey**</span></span> <br/> |<span data-ttu-id="f810c-118">Identifica a chave de alteração do item raiz repositório à qual o anexo está vinculado.</span><span class="sxs-lookup"><span data-stu-id="f810c-118">Identifies the change key of the root store item to which the attachment is attached.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f810c-119">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f810c-119">Child elements</span></span>

<span data-ttu-id="f810c-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f810c-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f810c-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f810c-121">Parent elements</span></span>

|<span data-ttu-id="f810c-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f810c-122">**Element**</span></span>|<span data-ttu-id="f810c-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f810c-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f810c-124">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="f810c-124">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="f810c-125">Representa um item do Exchange que está anexado a outro item do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f810c-125">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="f810c-126">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="f810c-126">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="f810c-127">Representa um arquivo anexado a um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f810c-127">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f810c-128">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="f810c-128">Remarks</span></span>

<span data-ttu-id="f810c-129">É importante observar que, quando um anexo é criado, a chave de alteração do item raiz seja alterada.</span><span class="sxs-lookup"><span data-stu-id="f810c-129">It is important to note that when an attachment is created, the change key of the root item is altered.</span></span>
  
<span data-ttu-id="f810c-130">O elemento [AttachmentId (GetAttachment e DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md) é usado em solicitações DeleteAttachment e GetAttachment.</span><span class="sxs-lookup"><span data-stu-id="f810c-130">The [AttachmentId (GetAttachment and DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md) element is used in DeleteAttachment and GetAttachment requests.</span></span> 
  
<span data-ttu-id="f810c-131">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="f810c-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f810c-132">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f810c-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f810c-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="f810c-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f810c-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f810c-134">Schema name</span></span>  <br/> |<span data-ttu-id="f810c-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f810c-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="f810c-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f810c-136">Validation file</span></span>  <br/> |<span data-ttu-id="f810c-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f810c-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f810c-138">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="f810c-138">Can be empty</span></span>  <br/> |<span data-ttu-id="f810c-139">False</span><span class="sxs-lookup"><span data-stu-id="f810c-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f810c-140">Ver também</span><span class="sxs-lookup"><span data-stu-id="f810c-140">See also</span></span>

- [<span data-ttu-id="f810c-141">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f810c-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

