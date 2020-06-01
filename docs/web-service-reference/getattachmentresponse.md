---
title: GetAttachmentResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetAttachmentResponse
api_type:
- schema
ms.assetid: cb65f449-309b-4b6e-8d22-d1967135490c
description: O elemento GetAttachmentResponse define uma resposta a uma solicitação GetAttachment.
ms.openlocfilehash: f0daf778f1248eabc5d51ee6155c460d9248549f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461251"
---
# <a name="getattachmentresponse"></a><span data-ttu-id="993dd-103">GetAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="993dd-103">GetAttachmentResponse</span></span>

<span data-ttu-id="993dd-104">O elemento **GetAttachmentResponse** define uma resposta a uma solicitação GetAttachment.</span><span class="sxs-lookup"><span data-stu-id="993dd-104">The **GetAttachmentResponse** element defines a response to a GetAttachment request.</span></span> 
  
```xml
<GetAttachmentResponse>
   <ResponseMessages/>
</GetAttachmentResponse>
```

 <span data-ttu-id="993dd-105">**GetAttachmentResponseType**</span><span class="sxs-lookup"><span data-stu-id="993dd-105">**GetAttachmentResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="993dd-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="993dd-106">Attributes and elements</span></span>

<span data-ttu-id="993dd-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="993dd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="993dd-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="993dd-108">Attributes</span></span>

<span data-ttu-id="993dd-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="993dd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="993dd-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="993dd-110">Child elements</span></span>

|<span data-ttu-id="993dd-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="993dd-111">**Element**</span></span>|<span data-ttu-id="993dd-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="993dd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="993dd-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="993dd-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="993dd-114">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="993dd-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="993dd-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="993dd-115">Parent elements</span></span>

<span data-ttu-id="993dd-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="993dd-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="993dd-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="993dd-117">Remarks</span></span>

<span data-ttu-id="993dd-118">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="993dd-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="993dd-119">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="993dd-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="993dd-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="993dd-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="993dd-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="993dd-121">Schema name</span></span>  <br/> |<span data-ttu-id="993dd-122">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="993dd-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="993dd-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="993dd-123">Validation file</span></span>  <br/> |<span data-ttu-id="993dd-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="993dd-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="993dd-125">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="993dd-125">Can be empty</span></span>  <br/> |<span data-ttu-id="993dd-126">False</span><span class="sxs-lookup"><span data-stu-id="993dd-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="993dd-127">Confira também</span><span class="sxs-lookup"><span data-stu-id="993dd-127">See also</span></span>



[<span data-ttu-id="993dd-128">Operação GetAttachment</span><span class="sxs-lookup"><span data-stu-id="993dd-128">GetAttachment operation</span></span>](getattachment-operation.md)
  
[<span data-ttu-id="993dd-129">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="993dd-129">GetAttachment</span></span>](getattachment.md)

