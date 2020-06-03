---
title: Attachmentid (GetAttachment e DeleteAttachment)
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
ms.assetid: 4bea1cb5-0a0f-4e14-9b09-f91af8cf9899
description: O elemento attachmentid identifica um único anexo.
ms.openlocfilehash: 1096487490f6066f70d2da861b3015f0fbf5a68f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460852"
---
# <a name="attachmentid-getattachment-and-deleteattachment"></a><span data-ttu-id="533fe-103">Attachmentid (GetAttachment e DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="533fe-103">AttachmentId (GetAttachment and DeleteAttachment)</span></span>

<span data-ttu-id="533fe-104">O elemento **attachmentid** identifica um único anexo.</span><span class="sxs-lookup"><span data-stu-id="533fe-104">The **AttachmentId** element identifies a single attachment.</span></span> 
  
```xml
<AttachmentId Id="" />
```

 <span data-ttu-id="533fe-105">**RequestAttachmentIdType**</span><span class="sxs-lookup"><span data-stu-id="533fe-105">**RequestAttachmentIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="533fe-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="533fe-106">Attributes and elements</span></span>

<span data-ttu-id="533fe-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="533fe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="533fe-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="533fe-108">Attributes</span></span>

|<span data-ttu-id="533fe-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="533fe-109">**Attribute**</span></span>|<span data-ttu-id="533fe-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="533fe-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="533fe-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="533fe-111">**Id**</span></span> <br/> |<span data-ttu-id="533fe-112">Especifica o identificador do anexo.</span><span class="sxs-lookup"><span data-stu-id="533fe-112">Specifies the attachment identifier.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="533fe-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="533fe-113">Child elements</span></span>

<span data-ttu-id="533fe-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="533fe-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="533fe-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="533fe-115">Parent elements</span></span>

|<span data-ttu-id="533fe-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="533fe-116">**Element**</span></span>|<span data-ttu-id="533fe-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="533fe-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="533fe-118">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="533fe-118">AttachmentIds</span></span>](attachmentids.md) <br/> | <span data-ttu-id="533fe-119">Contém uma matriz de identificadores de anexo.</span><span class="sxs-lookup"><span data-stu-id="533fe-119">Contains an array of attachment identifiers.</span></span><br/><br/>  <span data-ttu-id="533fe-120">A seguir estão as expressões XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="533fe-120">The following are the XPath expressions to this element:</span></span><br/><br/>`/DeleteAttachment/AttachmentIds`<br/><br/>`/GetAttachment/AttachmentIds` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="533fe-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="533fe-121">Remarks</span></span>

<span data-ttu-id="533fe-122">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="533fe-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="533fe-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="533fe-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="533fe-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="533fe-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="533fe-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="533fe-125">Schema Name</span></span>  <br/> |<span data-ttu-id="533fe-126">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="533fe-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="533fe-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="533fe-127">Validation File</span></span>  <br/> |<span data-ttu-id="533fe-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="533fe-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="533fe-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="533fe-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="533fe-130">False</span><span class="sxs-lookup"><span data-stu-id="533fe-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="533fe-131">Confira também</span><span class="sxs-lookup"><span data-stu-id="533fe-131">See also</span></span>

- [<span data-ttu-id="533fe-132">Operação DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="533fe-132">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
- [<span data-ttu-id="533fe-133">Operação GetAttachment</span><span class="sxs-lookup"><span data-stu-id="533fe-133">GetAttachment operation</span></span>](getattachment-operation.md)

