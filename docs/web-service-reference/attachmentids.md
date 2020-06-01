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
ms.openlocfilehash: cff1cb5658690fd6dd2c6a7812e1f600a4c80e29
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464249"
---
# <a name="attachmentids"></a><span data-ttu-id="2f2ac-103">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="2f2ac-103">AttachmentIds</span></span>

<span data-ttu-id="2f2ac-104">O elemento **AttachmentIds** contém uma matriz de identificadores de anexo.</span><span class="sxs-lookup"><span data-stu-id="2f2ac-104">The **AttachmentIds** element contains an array of attachment identifiers.</span></span> 
  
```xml
<AttachmentIds>
   <AttachmentId Id=""/>
</AttachmentIds>
```

 <span data-ttu-id="2f2ac-105">**NonEmptyArrayOfRequestAttachmentIdsType**</span><span class="sxs-lookup"><span data-stu-id="2f2ac-105">**NonEmptyArrayOfRequestAttachmentIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2f2ac-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="2f2ac-106">Attributes and elements</span></span>

<span data-ttu-id="2f2ac-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2f2ac-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2f2ac-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2f2ac-108">Attributes</span></span>

<span data-ttu-id="2f2ac-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2f2ac-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2f2ac-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2f2ac-110">Child elements</span></span>

|<span data-ttu-id="2f2ac-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2f2ac-111">**Element**</span></span>|<span data-ttu-id="2f2ac-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2f2ac-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2f2ac-113">Attachmentid (GetAttachment e DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="2f2ac-113">AttachmentId (GetAttachment and DeleteAttachment)</span></span>](attachmentid-getattachment-and-deleteattachment.md) <br/> |<span data-ttu-id="2f2ac-114">O elemento que identifica um único anexo.</span><span class="sxs-lookup"><span data-stu-id="2f2ac-114">The element that identifies a single attachment.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2f2ac-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2f2ac-115">Parent elements</span></span>

|<span data-ttu-id="2f2ac-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2f2ac-116">**Element**</span></span>|<span data-ttu-id="2f2ac-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2f2ac-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2f2ac-118">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="2f2ac-118">DeleteAttachment</span></span>](deleteattachment.md) <br/> |<span data-ttu-id="2f2ac-119">O elemento que define uma solicitação para excluir um anexo do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2f2ac-119">The element that defines a request to delete an attachment from the Exchange store.</span></span>  <br/> <span data-ttu-id="2f2ac-120">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="2f2ac-120">The following is the XPath expression to this element:</span></span>  <br/>  `/DeleteAttachment` <br/> |
|[<span data-ttu-id="2f2ac-121">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="2f2ac-121">GetAttachment</span></span>](getattachment.md) <br/> |<span data-ttu-id="2f2ac-122">O elemento que define uma solicitação para obter um anexo do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2f2ac-122">The element that defines a request to get an attachment from the Exchange store.</span></span>  <br/> <span data-ttu-id="2f2ac-123">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="2f2ac-123">The following is the XPath expression to this element:</span></span>  <br/>  `/GetAttachment` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2f2ac-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="2f2ac-124">Remarks</span></span>

<span data-ttu-id="2f2ac-125">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="2f2ac-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2f2ac-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="2f2ac-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2f2ac-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="2f2ac-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2f2ac-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2f2ac-128">Schema Name</span></span>  <br/> |<span data-ttu-id="2f2ac-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="2f2ac-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2f2ac-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2f2ac-130">Validation File</span></span>  <br/> |<span data-ttu-id="2f2ac-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2f2ac-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2f2ac-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="2f2ac-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="2f2ac-133">False</span><span class="sxs-lookup"><span data-stu-id="2f2ac-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2f2ac-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="2f2ac-134">See also</span></span>

- [<span data-ttu-id="2f2ac-135">Operação DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="2f2ac-135">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
- [<span data-ttu-id="2f2ac-136">Operação GetAttachment</span><span class="sxs-lookup"><span data-stu-id="2f2ac-136">GetAttachment operation</span></span>](getattachment-operation.md)

