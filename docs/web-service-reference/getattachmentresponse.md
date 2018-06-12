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
description: O elemento de GetAttachmentResponse define uma resposta a uma solicitação de GetAttachment.
ms.openlocfilehash: 05a9e84236c791dcec99182dfca0352e44efca46
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752410"
---
# <a name="getattachmentresponse"></a><span data-ttu-id="ffcca-103">GetAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="ffcca-103">GetAttachmentResponse</span></span>

<span data-ttu-id="ffcca-104">O elemento de **GetAttachmentResponse** define uma resposta a uma solicitação de GetAttachment.</span><span class="sxs-lookup"><span data-stu-id="ffcca-104">The **GetAttachmentResponse** element defines a response to a GetAttachment request.</span></span> 
  
```xml
<GetAttachmentResponse>
   <ResponseMessages/>
</GetAttachmentResponse>
```

 <span data-ttu-id="ffcca-105">**GetAttachmentResponseType**</span><span class="sxs-lookup"><span data-stu-id="ffcca-105">**GetAttachmentResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ffcca-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ffcca-106">Attributes and elements</span></span>

<span data-ttu-id="ffcca-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ffcca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ffcca-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ffcca-108">Attributes</span></span>

<span data-ttu-id="ffcca-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ffcca-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ffcca-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ffcca-110">Child elements</span></span>

|<span data-ttu-id="ffcca-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ffcca-111">**Element**</span></span>|<span data-ttu-id="ffcca-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ffcca-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ffcca-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ffcca-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="ffcca-114">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ffcca-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ffcca-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ffcca-115">Parent elements</span></span>

<span data-ttu-id="ffcca-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ffcca-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ffcca-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="ffcca-117">Remarks</span></span>

<span data-ttu-id="ffcca-118">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="ffcca-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ffcca-119">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ffcca-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ffcca-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="ffcca-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ffcca-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ffcca-121">Schema name</span></span>  <br/> |<span data-ttu-id="ffcca-122">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="ffcca-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ffcca-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ffcca-123">Validation file</span></span>  <br/> |<span data-ttu-id="ffcca-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ffcca-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ffcca-125">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="ffcca-125">Can be empty</span></span>  <br/> |<span data-ttu-id="ffcca-126">False</span><span class="sxs-lookup"><span data-stu-id="ffcca-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ffcca-127">Ver também</span><span class="sxs-lookup"><span data-stu-id="ffcca-127">See also</span></span>



[<span data-ttu-id="ffcca-128">Operação GetAttachment</span><span class="sxs-lookup"><span data-stu-id="ffcca-128">GetAttachment operation</span></span>](getattachment-operation.md)
  
[<span data-ttu-id="ffcca-129">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="ffcca-129">GetAttachment</span></span>](getattachment.md)

