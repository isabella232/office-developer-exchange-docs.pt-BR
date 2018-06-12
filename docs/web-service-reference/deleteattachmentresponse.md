---
title: DeleteAttachmentResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteAttachmentResponse
api_type:
- schema
ms.assetid: 24099a88-4ab6-4bf3-8ed5-efec8e07b9b9
description: O DeleteAttachmentResponse define uma resposta a uma solicitação de DeleteAttachment.
ms.openlocfilehash: f1a6b0ebba7257d02ceeea024486dc002d299dff
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751729"
---
# <a name="deleteattachmentresponse"></a><span data-ttu-id="b11fd-103">DeleteAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="b11fd-103">DeleteAttachmentResponse</span></span>

<span data-ttu-id="b11fd-104">O **DeleteAttachmentResponse** define uma resposta a uma solicitação de DeleteAttachment.</span><span class="sxs-lookup"><span data-stu-id="b11fd-104">The **DeleteAttachmentResponse** defines a response to a DeleteAttachment request.</span></span> 
  
```xml
<DeleteAttachmentResponse>
   <ResponseMessages/>
</DeleteAttachmentResponse>
```

<span data-ttu-id="b11fd-105">**DeleteAttachmentResponseType**</span><span class="sxs-lookup"><span data-stu-id="b11fd-105">**DeleteAttachmentResponseType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b11fd-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b11fd-106">Attributes and elements</span></span>

<span data-ttu-id="b11fd-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b11fd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b11fd-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b11fd-108">Attributes</span></span>

<span data-ttu-id="b11fd-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b11fd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b11fd-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b11fd-110">Child elements</span></span>

|<span data-ttu-id="b11fd-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b11fd-111">**Element**</span></span>|<span data-ttu-id="b11fd-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b11fd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b11fd-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b11fd-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="b11fd-114">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b11fd-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b11fd-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b11fd-115">Parent elements</span></span>

<span data-ttu-id="b11fd-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b11fd-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b11fd-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="b11fd-117">Remarks</span></span>

<span data-ttu-id="b11fd-118">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="b11fd-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b11fd-119">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b11fd-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b11fd-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="b11fd-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b11fd-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b11fd-121">Schema name</span></span>  <br/> |<span data-ttu-id="b11fd-122">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="b11fd-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b11fd-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b11fd-123">Validation file</span></span>  <br/> |<span data-ttu-id="b11fd-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b11fd-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b11fd-125">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="b11fd-125">Can be empty</span></span>  <br/> |<span data-ttu-id="b11fd-126">False</span><span class="sxs-lookup"><span data-stu-id="b11fd-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b11fd-127">Ver também</span><span class="sxs-lookup"><span data-stu-id="b11fd-127">See also</span></span>

- [<span data-ttu-id="b11fd-128">Operação DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="b11fd-128">DeleteAttachment operation</span></span>](deleteattachment-operation.md)  
- [<span data-ttu-id="b11fd-129">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="b11fd-129">DeleteAttachment</span></span>](deleteattachment.md)
- [<span data-ttu-id="b11fd-130">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b11fd-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

