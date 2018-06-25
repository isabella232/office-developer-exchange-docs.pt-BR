---
title: InvalidRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InvalidRecipients
api_type:
- schema
ms.assetid: e4e7b50e-2fa9-4649-94a6-6002f341ecc4
description: O elemento InvalidRecipients representa os destinatários de uma solicitação de compartilhamento de pasta que são inválidos.
ms.openlocfilehash: 02ad8935bde347c563875bf5bfb31968b70d81b6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823966"
---
# <a name="invalidrecipients"></a><span data-ttu-id="8a2eb-103">InvalidRecipients</span><span class="sxs-lookup"><span data-stu-id="8a2eb-103">InvalidRecipients</span></span>

<span data-ttu-id="8a2eb-104">O elemento **InvalidRecipients** representa os destinatários de uma solicitação de compartilhamento de pasta que são inválidos.</span><span class="sxs-lookup"><span data-stu-id="8a2eb-104">The **InvalidRecipients** element represents the recipients of a folder sharing request that are invalid.</span></span> 
  
```XML
<InvalidRecipients>
   <InvalidRecipient/>
</InvalidRecipients>
```

 <span data-ttu-id="8a2eb-105">**ArrayOfInvalidRecipientsType**</span><span class="sxs-lookup"><span data-stu-id="8a2eb-105">**ArrayOfInvalidRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8a2eb-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="8a2eb-106">Attributes and elements</span></span>

<span data-ttu-id="8a2eb-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8a2eb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8a2eb-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8a2eb-108">Attributes</span></span>

<span data-ttu-id="8a2eb-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8a2eb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8a2eb-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8a2eb-110">Child elements</span></span>

|<span data-ttu-id="8a2eb-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8a2eb-111">**Element**</span></span>|<span data-ttu-id="8a2eb-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8a2eb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8a2eb-113">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="8a2eb-113">InvalidRecipient</span></span>](invalidrecipient.md) <br/> |<span data-ttu-id="8a2eb-114">Contém o endereço SMTP do destinatário inválido e informações sobre por que o destinatário é inválido.</span><span class="sxs-lookup"><span data-stu-id="8a2eb-114">Contains the SMTP address of the invalid recipient and information about why the recipient is invalid.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8a2eb-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8a2eb-115">Parent elements</span></span>

|<span data-ttu-id="8a2eb-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8a2eb-116">**Element**</span></span>|<span data-ttu-id="8a2eb-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8a2eb-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8a2eb-118">GetSharingMetadataResponse</span><span class="sxs-lookup"><span data-stu-id="8a2eb-118">GetSharingMetadataResponse</span></span>](getsharingmetadataresponse.md) <br/> |<span data-ttu-id="8a2eb-119">Define uma resposta a uma solicitação de [operação GetSharingMetadata](getsharingmetadata-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="8a2eb-119">Defines a response to a [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="8a2eb-120">GetSharingMetadataResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8a2eb-120">GetSharingMetadataResponseMessage</span></span>](getsharingmetadataresponsemessage.md) <br/> |<span data-ttu-id="8a2eb-121">Contém o status e o resultado de uma única solicitação de [operação GetSharingMetadata](getsharingmetadata-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="8a2eb-121">Contains the status and result of a single [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8a2eb-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="8a2eb-122">Remarks</span></span>

<span data-ttu-id="8a2eb-123">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8a2eb-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8a2eb-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="8a2eb-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8a2eb-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="8a2eb-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8a2eb-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8a2eb-126">Schema Name</span></span>  <br/> |<span data-ttu-id="8a2eb-127">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="8a2eb-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8a2eb-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8a2eb-128">Validation File</span></span>  <br/> |<span data-ttu-id="8a2eb-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8a2eb-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8a2eb-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8a2eb-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="8a2eb-131">False</span><span class="sxs-lookup"><span data-stu-id="8a2eb-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8a2eb-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="8a2eb-132">See also</span></span>



[<span data-ttu-id="8a2eb-133">Operação GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="8a2eb-133">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="8a2eb-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8a2eb-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

