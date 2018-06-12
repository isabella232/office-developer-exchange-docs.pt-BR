---
title: AttachmentIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttachmentIds
api_type:
- schema
ms.assetid: 46ce3ad7-4b20-43ae-8c63-39f1e3c2666b
description: O elemento AttachmentIds contém uma matriz de identificadores de anexo.
ms.openlocfilehash: f205aefe6a7dc4ec208e8a96b8a6b47094aa741b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751222"
---
# <a name="attachmentids"></a><span data-ttu-id="5b79d-103">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="5b79d-103">AttachmentIds</span></span>

<span data-ttu-id="5b79d-104">O elemento **AttachmentIds** contém uma matriz de identificadores de anexo.</span><span class="sxs-lookup"><span data-stu-id="5b79d-104">The **AttachmentIds** element contains an array of attachment identifiers.</span></span> 
  
```xml
<AttachmentIds>
   <AttachmentId Id=""/>
</AttachmentIds>
```

 <span data-ttu-id="5b79d-105">**NonEmptyArrayOfRequestAttachmentIdsType**</span><span class="sxs-lookup"><span data-stu-id="5b79d-105">**NonEmptyArrayOfRequestAttachmentIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5b79d-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="5b79d-106">Attributes and elements</span></span>

<span data-ttu-id="5b79d-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5b79d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5b79d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5b79d-108">Attributes</span></span>

<span data-ttu-id="5b79d-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5b79d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5b79d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5b79d-110">Child elements</span></span>

|<span data-ttu-id="5b79d-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5b79d-111">**Element**</span></span>|<span data-ttu-id="5b79d-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5b79d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5b79d-113">AttachmentId (GetAttachment e DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="5b79d-113">AttachmentId (GetAttachment and DeleteAttachment)</span></span>](attachmentid-getattachment-and-deleteattachment.md) <br/> |<span data-ttu-id="5b79d-114">O elemento que identifica um único anexo.</span><span class="sxs-lookup"><span data-stu-id="5b79d-114">The element that identifies a single attachment.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5b79d-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5b79d-115">Parent elements</span></span>

|<span data-ttu-id="5b79d-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5b79d-116">**Element**</span></span>|<span data-ttu-id="5b79d-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5b79d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5b79d-118">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="5b79d-118">DeleteAttachment</span></span>](deleteattachment.md) <br/> |<span data-ttu-id="5b79d-119">O elemento que define uma solicitação para excluir um anexo do armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5b79d-119">The element that defines a request to delete an attachment from the Exchange store.</span></span>  <br/> <span data-ttu-id="5b79d-120">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="5b79d-120">The following is the XPath expression to this element:</span></span>  <br/>  `/DeleteAttachment` <br/> |
|[<span data-ttu-id="5b79d-121">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="5b79d-121">GetAttachment</span></span>](getattachment.md) <br/> |<span data-ttu-id="5b79d-122">O elemento que define uma solicitação para obter um anexo do armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5b79d-122">The element that defines a request to get an attachment from the Exchange store.</span></span>  <br/> <span data-ttu-id="5b79d-123">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="5b79d-123">The following is the XPath expression to this element:</span></span>  <br/>  `/GetAttachment` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5b79d-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="5b79d-124">Remarks</span></span>

<span data-ttu-id="5b79d-125">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="5b79d-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5b79d-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="5b79d-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5b79d-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="5b79d-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5b79d-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5b79d-128">Schema Name</span></span>  <br/> |<span data-ttu-id="5b79d-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="5b79d-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5b79d-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5b79d-130">Validation File</span></span>  <br/> |<span data-ttu-id="5b79d-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5b79d-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5b79d-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5b79d-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="5b79d-133">False</span><span class="sxs-lookup"><span data-stu-id="5b79d-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5b79d-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="5b79d-134">See also</span></span>

- [<span data-ttu-id="5b79d-135">Operação DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="5b79d-135">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
- [<span data-ttu-id="5b79d-136">Operação GetAttachment</span><span class="sxs-lookup"><span data-stu-id="5b79d-136">GetAttachment operation</span></span>](getattachment-operation.md)

