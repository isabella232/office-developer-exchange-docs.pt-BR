---
title: Attachmentid
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
description: O elemento attachmentid identifica um item ou anexo de arquivo. Este elemento é usado em respostas de CreateAttachment.
ms.openlocfilehash: b5dc9299b615f0fc01b8afcbaabf0ec7996e53d1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459108"
---
# <a name="attachmentid"></a><span data-ttu-id="3f34b-104">Attachmentid</span><span class="sxs-lookup"><span data-stu-id="3f34b-104">AttachmentId</span></span>

<span data-ttu-id="3f34b-105">O elemento **attachmentid** identifica um item ou anexo de arquivo.</span><span class="sxs-lookup"><span data-stu-id="3f34b-105">The **AttachmentId** element identifies an item or file attachment.</span></span> <span data-ttu-id="3f34b-106">Este elemento é usado em respostas de CreateAttachment.</span><span class="sxs-lookup"><span data-stu-id="3f34b-106">This element is used in CreateAttachment responses.</span></span> 
  
```xml
<AttachmentId Id="" RootItemId="" RootItemChangeKey="" />
```

 <span data-ttu-id="3f34b-107">**AttachmentIdType**</span><span class="sxs-lookup"><span data-stu-id="3f34b-107">**AttachmentIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3f34b-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="3f34b-108">Attributes and elements</span></span>

<span data-ttu-id="3f34b-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3f34b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3f34b-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="3f34b-110">Attributes</span></span>

|<span data-ttu-id="3f34b-111">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="3f34b-111">**Attribute**</span></span>|<span data-ttu-id="3f34b-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3f34b-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3f34b-113">**Id**</span><span class="sxs-lookup"><span data-stu-id="3f34b-113">**Id**</span></span> <br/> |<span data-ttu-id="3f34b-114">Identifica o identificador exclusivo do anexo.</span><span class="sxs-lookup"><span data-stu-id="3f34b-114">Identifies the unique identifier of the attachment.</span></span>  <br/> |
|<span data-ttu-id="3f34b-115">**RootItemId**</span><span class="sxs-lookup"><span data-stu-id="3f34b-115">**RootItemId**</span></span> <br/> |<span data-ttu-id="3f34b-116">Identifica o identificador exclusivo do item de repositório raiz ao qual o anexo está anexado.</span><span class="sxs-lookup"><span data-stu-id="3f34b-116">Identifies the unique identifier of the root store item to which the attachment is attached.</span></span>  <br/> |
|<span data-ttu-id="3f34b-117">**RootItemChangeKey**</span><span class="sxs-lookup"><span data-stu-id="3f34b-117">**RootItemChangeKey**</span></span> <br/> |<span data-ttu-id="3f34b-118">Identifica a chave de alteração do item de armazenamento raiz ao qual o anexo está anexado.</span><span class="sxs-lookup"><span data-stu-id="3f34b-118">Identifies the change key of the root store item to which the attachment is attached.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="3f34b-119">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3f34b-119">Child elements</span></span>

<span data-ttu-id="3f34b-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3f34b-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3f34b-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3f34b-121">Parent elements</span></span>

|<span data-ttu-id="3f34b-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3f34b-122">**Element**</span></span>|<span data-ttu-id="3f34b-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3f34b-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3f34b-124">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="3f34b-124">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="3f34b-125">Representa um item do Exchange anexado a outro item do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3f34b-125">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="3f34b-126">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="3f34b-126">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="3f34b-127">Representa um arquivo anexado a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3f34b-127">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3f34b-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="3f34b-128">Remarks</span></span>

<span data-ttu-id="3f34b-129">É importante observar que, quando um anexo é criado, a chave de alteração do item raiz é alterada.</span><span class="sxs-lookup"><span data-stu-id="3f34b-129">It is important to note that when an attachment is created, the change key of the root item is altered.</span></span>
  
<span data-ttu-id="3f34b-130">O elemento [attachmentid (GetAttachment e DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md) é usado em solicitações DeleteAttachment e GetAttachment.</span><span class="sxs-lookup"><span data-stu-id="3f34b-130">The [AttachmentId (GetAttachment and DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md) element is used in DeleteAttachment and GetAttachment requests.</span></span> 
  
<span data-ttu-id="3f34b-131">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="3f34b-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3f34b-132">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="3f34b-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3f34b-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="3f34b-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3f34b-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3f34b-134">Schema name</span></span>  <br/> |<span data-ttu-id="3f34b-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3f34b-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="3f34b-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3f34b-136">Validation file</span></span>  <br/> |<span data-ttu-id="3f34b-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="3f34b-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3f34b-138">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="3f34b-138">Can be empty</span></span>  <br/> |<span data-ttu-id="3f34b-139">False</span><span class="sxs-lookup"><span data-stu-id="3f34b-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3f34b-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="3f34b-140">See also</span></span>

- [<span data-ttu-id="3f34b-141">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3f34b-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

