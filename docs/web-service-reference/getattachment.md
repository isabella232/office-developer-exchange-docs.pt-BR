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
description: O elemento GetAttachment é o elemento raiz em uma solicitação para obter um anexo do repositório do Exchange.
ms.openlocfilehash: d03d086ff443db87b0104a2ec83599eb9eaea6b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463976"
---
# <a name="getattachment"></a><span data-ttu-id="2f047-103">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="2f047-103">GetAttachment</span></span>

<span data-ttu-id="2f047-104">O elemento **GetAttachment** é o elemento raiz em uma solicitação para obter um anexo do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2f047-104">The **GetAttachment** element is the root element in a request to get an attachment from the Exchange store.</span></span> 
  
```xml
<GetAttachment>
   <AttachmentShape/>
   <AttachmentIds/>
</GetAttachment>
```

 <span data-ttu-id="2f047-105">**GetAttachmentType**</span><span class="sxs-lookup"><span data-stu-id="2f047-105">**GetAttachmentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2f047-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="2f047-106">Attributes and elements</span></span>

<span data-ttu-id="2f047-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2f047-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2f047-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2f047-108">Attributes</span></span>

<span data-ttu-id="2f047-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2f047-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2f047-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2f047-110">Child elements</span></span>

|<span data-ttu-id="2f047-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2f047-111">**Element**</span></span>|<span data-ttu-id="2f047-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2f047-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2f047-113">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="2f047-113">AttachmentShape</span></span>](attachmentshape.md) <br/> |<span data-ttu-id="2f047-114">Identifica Propriedades de item estendido adicionais para retornar em uma resposta a uma solicitação [GetAttachment](getattachment.md) .</span><span class="sxs-lookup"><span data-stu-id="2f047-114">Identifies additional extended item properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span> <span data-ttu-id="2f047-115">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="2f047-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="2f047-116">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="2f047-116">AttachmentIds</span></span>](attachmentids.md) <br/> |<span data-ttu-id="2f047-117">Contém uma matriz de identificadores de anexo.</span><span class="sxs-lookup"><span data-stu-id="2f047-117">Contains an array of attachment identifiers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2f047-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2f047-118">Parent elements</span></span>

<span data-ttu-id="2f047-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2f047-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2f047-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="2f047-120">Remarks</span></span>

<span data-ttu-id="2f047-121">O elemento [AttachmentShape](attachmentshape.md) não é necessário para identificar as propriedades retornadas na resposta.</span><span class="sxs-lookup"><span data-stu-id="2f047-121">The [AttachmentShape](attachmentshape.md) element is not required to identify the properties returned in the response.</span></span> <span data-ttu-id="2f047-122">A [operação GetAttachment](getattachment-operation.md) retorna o nome, ContentType, ContentId, ContentLocation e as propriedades de conteúdo para anexos de arquivo.</span><span class="sxs-lookup"><span data-stu-id="2f047-122">The [GetAttachment operation](getattachment-operation.md) returns the Name, ContentType, ContentId, ContentLocation, and the Content properties for file attachments.</span></span> <span data-ttu-id="2f047-123">Para anexos de item, as propriedades retornadas são o nome, ContentType, ContentId, ContentLocation e todas as propriedades do item anexado.</span><span class="sxs-lookup"><span data-stu-id="2f047-123">For item attachments, the returned properties are the Name, ContentType, ContentId, ContentLocation, and all the attached item's properties.</span></span> <span data-ttu-id="2f047-124">Isso equivale a usar a forma base de propriedades em uma solicitação [GetItem](getitem.md) .</span><span class="sxs-lookup"><span data-stu-id="2f047-124">This is equivalent to using the AllProperties base shape in a [GetItem](getitem.md) request.</span></span> 
  
<span data-ttu-id="2f047-125">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="2f047-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2f047-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="2f047-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2f047-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="2f047-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2f047-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2f047-128">Schema Name</span></span>  <br/> |<span data-ttu-id="2f047-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="2f047-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2f047-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2f047-130">Validation File</span></span>  <br/> |<span data-ttu-id="2f047-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2f047-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2f047-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="2f047-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="2f047-133">False</span><span class="sxs-lookup"><span data-stu-id="2f047-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2f047-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="2f047-134">See also</span></span>



[<span data-ttu-id="2f047-135">Operação GetAttachment</span><span class="sxs-lookup"><span data-stu-id="2f047-135">GetAttachment operation</span></span>](getattachment-operation.md)
  
[<span data-ttu-id="2f047-136">GetAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="2f047-136">GetAttachmentResponse</span></span>](getattachmentresponse.md)

