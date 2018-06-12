---
title: InvalidRecipient
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InvalidRecipient
api_type:
- schema
ms.assetid: 9e2d3433-22d7-444b-9883-e5649297d8fe
description: O elemento InvalidRecipient contém o endereço SMTP do destinatário inválido e informações sobre por que o destinatário é inválido.
ms.openlocfilehash: 800056666e486e9337dcd1c2786f7e6db1e060bb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823961"
---
# <a name="invalidrecipient"></a><span data-ttu-id="b589d-103">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="b589d-103">InvalidRecipient</span></span>

<span data-ttu-id="b589d-104">O elemento **InvalidRecipient** contém o endereço SMTP do destinatário inválido e informações sobre por que o destinatário é inválido.</span><span class="sxs-lookup"><span data-stu-id="b589d-104">The **InvalidRecipient** element contains the SMTP address of the invalid recipient and information about why the recipient is invalid.</span></span> 
  
```XML
<InvalidRecipient>
   <SmtpAddress/>
   <ResponseCode/>
   <MessageText/>
</InvalidRecipient>

```

 <span data-ttu-id="b589d-105">**InvalidRecipientType**</span><span class="sxs-lookup"><span data-stu-id="b589d-105">**InvalidRecipientType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b589d-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b589d-106">Attributes and elements</span></span>

<span data-ttu-id="b589d-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b589d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b589d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b589d-108">Attributes</span></span>

<span data-ttu-id="b589d-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b589d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b589d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b589d-110">Child elements</span></span>

|<span data-ttu-id="b589d-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b589d-111">**Element**</span></span>|<span data-ttu-id="b589d-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b589d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b589d-113">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="b589d-113">SmtpAddress</span></span>](smtpaddress.md) <br/> |<span data-ttu-id="b589d-114">Contém o endereço SMTP do destinatário inválido.</span><span class="sxs-lookup"><span data-stu-id="b589d-114">Contains the SMTP address of the invalid recipient.</span></span> <span data-ttu-id="b589d-115">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b589d-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="b589d-116">ResponseCode (InvalidRecipientResponseCodeType)</span><span class="sxs-lookup"><span data-stu-id="b589d-116">ResponseCode (InvalidRecipientResponseCodeType)</span></span>](responsecode-invalidrecipientresponsecodetype.md) <br/> |<span data-ttu-id="b589d-117">Fornece um código de erro que identifica o erro específico que enfrentaram a solicitação.</span><span class="sxs-lookup"><span data-stu-id="b589d-117">Provides an error code that identifies the specific error that the request encountered.</span></span> <span data-ttu-id="b589d-118">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b589d-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="b589d-119">MessageText</span><span class="sxs-lookup"><span data-stu-id="b589d-119">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="b589d-120">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="b589d-120">Provides a text description of the status of the response.</span></span> <span data-ttu-id="b589d-121">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="b589d-121">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b589d-122">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b589d-122">Parent elements</span></span>

|<span data-ttu-id="b589d-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b589d-123">**Element**</span></span>|<span data-ttu-id="b589d-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b589d-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b589d-125">InvalidRecipients</span><span class="sxs-lookup"><span data-stu-id="b589d-125">InvalidRecipients</span></span>](invalidrecipients.md) <br/> |<span data-ttu-id="b589d-126">Representa os destinatários de uma solicitação de compartilhamento de pasta que são inválidos.</span><span class="sxs-lookup"><span data-stu-id="b589d-126">Represents the recipients of a folder sharing request that are invalid.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b589d-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="b589d-127">Remarks</span></span>

<span data-ttu-id="b589d-128">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b589d-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b589d-129">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b589d-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b589d-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="b589d-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b589d-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b589d-131">Schema Name</span></span>  <br/> |<span data-ttu-id="b589d-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b589d-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="b589d-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b589d-133">Validation File</span></span>  <br/> |<span data-ttu-id="b589d-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b589d-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b589d-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b589d-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="b589d-136">False</span><span class="sxs-lookup"><span data-stu-id="b589d-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b589d-137">Ver também</span><span class="sxs-lookup"><span data-stu-id="b589d-137">See also</span></span>



[<span data-ttu-id="b589d-138">Operação GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="b589d-138">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="b589d-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b589d-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

