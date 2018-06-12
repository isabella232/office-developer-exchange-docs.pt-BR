---
title: RootItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RootItemId
api_type:
- schema
ms.assetid: f613c705-17ce-48ce-aa64-4dc2cea25e31
description: O elemento RootItemId identifica o item de raiz de um anexo excluído.
ms.openlocfilehash: 484b185db63c9692eaca7e43c49d6e95375a1a98
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825251"
---
# <a name="rootitemid"></a><span data-ttu-id="0b25f-103">RootItemId</span><span class="sxs-lookup"><span data-stu-id="0b25f-103">RootItemId</span></span>

<span data-ttu-id="0b25f-104">O elemento **RootItemId** identifica o item de raiz de um anexo excluído.</span><span class="sxs-lookup"><span data-stu-id="0b25f-104">The **RootItemId** element identifies the root item of a deleted attachment.</span></span> 
  
[<span data-ttu-id="0b25f-105">DeleteAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="0b25f-105">DeleteAttachmentResponse</span></span>](deleteattachmentresponse.md)
  
[<span data-ttu-id="0b25f-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0b25f-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="0b25f-107">DeleteAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0b25f-107">DeleteAttachmentResponseMessage</span></span>](deleteattachmentresponsemessage.md)
  
[<span data-ttu-id="0b25f-108">RootItemId</span><span class="sxs-lookup"><span data-stu-id="0b25f-108">RootItemId</span></span>](rootitemid.md)
  
```xml
<RootItemId RootItemId="" RootItemChangeKey="" />
```

 <span data-ttu-id="0b25f-109">**RootItemIdType**</span><span class="sxs-lookup"><span data-stu-id="0b25f-109">**RootItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0b25f-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="0b25f-110">Attributes and elements</span></span>

<span data-ttu-id="0b25f-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0b25f-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0b25f-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="0b25f-112">Attributes</span></span>

|<span data-ttu-id="0b25f-113">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="0b25f-113">**Attribute**</span></span>|<span data-ttu-id="0b25f-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0b25f-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0b25f-115">**RootItemId**</span><span class="sxs-lookup"><span data-stu-id="0b25f-115">**RootItemId**</span></span> <br/> |<span data-ttu-id="0b25f-116">Identifica o item raiz de um anexo excluído.</span><span class="sxs-lookup"><span data-stu-id="0b25f-116">Identifies the root item of a deleted attachment.</span></span>  <br/> |
|<span data-ttu-id="0b25f-117">**RootItemChangeKey**</span><span class="sxs-lookup"><span data-stu-id="0b25f-117">**RootItemChangeKey**</span></span> <br/> |<span data-ttu-id="0b25f-118">Identifica a nova chave de alteração do item raiz de um anexo excluído.</span><span class="sxs-lookup"><span data-stu-id="0b25f-118">Identifies the new change key of the root item of a deleted attachment.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0b25f-119">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0b25f-119">Child elements</span></span>

<span data-ttu-id="0b25f-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0b25f-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0b25f-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0b25f-121">Parent elements</span></span>

|<span data-ttu-id="0b25f-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0b25f-122">**Element**</span></span>|<span data-ttu-id="0b25f-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0b25f-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b25f-124">DeleteAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0b25f-124">DeleteAttachmentResponseMessage</span></span>](deleteattachmentresponsemessage.md) <br/> |<span data-ttu-id="0b25f-125">Contém o status e o resultado de uma solicitação de DeleteAttachment.</span><span class="sxs-lookup"><span data-stu-id="0b25f-125">Contains the status and result of a DeleteAttachment request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0b25f-126">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="0b25f-126">Remarks</span></span>

<span data-ttu-id="0b25f-127">O elemento **RootItemId** é usado apenas em DeleteAttachment respostas.</span><span class="sxs-lookup"><span data-stu-id="0b25f-127">The **RootItemId** element is only used in DeleteAttachment responses.</span></span> <span data-ttu-id="0b25f-128">Isso identifica o identificador de item raiz e mais importante, a nova chave de alteração para o item pai.</span><span class="sxs-lookup"><span data-stu-id="0b25f-128">This identifies the root item identifier, and more importantly, the new change key to the parent item.</span></span> 
  
<span data-ttu-id="0b25f-129">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="0b25f-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0b25f-130">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="0b25f-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0b25f-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="0b25f-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0b25f-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0b25f-132">Schema name</span></span>  <br/> |<span data-ttu-id="0b25f-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="0b25f-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="0b25f-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0b25f-134">Validation file</span></span>  <br/> |<span data-ttu-id="0b25f-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0b25f-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0b25f-136">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="0b25f-136">Can be empty</span></span>  <br/> |<span data-ttu-id="0b25f-137">False</span><span class="sxs-lookup"><span data-stu-id="0b25f-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0b25f-138">Ver também</span><span class="sxs-lookup"><span data-stu-id="0b25f-138">See also</span></span>



[<span data-ttu-id="0b25f-139">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="0b25f-139">DeleteAttachment</span></span>](deleteattachment.md)
  
[<span data-ttu-id="0b25f-140">Operação DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="0b25f-140">DeleteAttachment operation</span></span>](deleteattachment-operation.md)


- [<span data-ttu-id="0b25f-141">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0b25f-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

