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
description: O elemento InvalidRecipient contém o endereço SMTP do destinatário inválido e as informações sobre o motivo pelo qual o destinatário é inválido.
ms.openlocfilehash: f301b31c1054625151ce90e41fca5e3efc21f473
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526547"
---
# <a name="invalidrecipient"></a><span data-ttu-id="943e9-103">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="943e9-103">InvalidRecipient</span></span>

<span data-ttu-id="943e9-104">O elemento **InvalidRecipient** contém o endereço SMTP do destinatário inválido e as informações sobre o motivo pelo qual o destinatário é inválido.</span><span class="sxs-lookup"><span data-stu-id="943e9-104">The **InvalidRecipient** element contains the SMTP address of the invalid recipient and information about why the recipient is invalid.</span></span> 
  
```XML
<InvalidRecipient>
   <SmtpAddress/>
   <ResponseCode/>
   <MessageText/>
</InvalidRecipient>

```

 <span data-ttu-id="943e9-105">**InvalidRecipientType**</span><span class="sxs-lookup"><span data-stu-id="943e9-105">**InvalidRecipientType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="943e9-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="943e9-106">Attributes and elements</span></span>

<span data-ttu-id="943e9-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="943e9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="943e9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="943e9-108">Attributes</span></span>

<span data-ttu-id="943e9-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="943e9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="943e9-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="943e9-110">Child elements</span></span>

|<span data-ttu-id="943e9-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="943e9-111">**Element**</span></span>|<span data-ttu-id="943e9-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="943e9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="943e9-113">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="943e9-113">SmtpAddress</span></span>](smtpaddress.md) <br/> |<span data-ttu-id="943e9-114">Contém o endereço SMTP do destinatário inválido.</span><span class="sxs-lookup"><span data-stu-id="943e9-114">Contains the SMTP address of the invalid recipient.</span></span> <span data-ttu-id="943e9-115">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="943e9-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="943e9-116">ResponseCode (InvalidRecipientResponseCodeType)</span><span class="sxs-lookup"><span data-stu-id="943e9-116">ResponseCode (InvalidRecipientResponseCodeType)</span></span>](responsecode-invalidrecipientresponsecodetype.md) <br/> |<span data-ttu-id="943e9-117">Fornece um código de erro que identifica o erro específico que a solicitação encontrou.</span><span class="sxs-lookup"><span data-stu-id="943e9-117">Provides an error code that identifies the specific error that the request encountered.</span></span> <span data-ttu-id="943e9-118">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="943e9-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="943e9-119">MessageText</span><span class="sxs-lookup"><span data-stu-id="943e9-119">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="943e9-120">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="943e9-120">Provides a text description of the status of the response.</span></span> <span data-ttu-id="943e9-121">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="943e9-121">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="943e9-122">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="943e9-122">Parent elements</span></span>

|<span data-ttu-id="943e9-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="943e9-123">**Element**</span></span>|<span data-ttu-id="943e9-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="943e9-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="943e9-125">InvalidRecipients</span><span class="sxs-lookup"><span data-stu-id="943e9-125">InvalidRecipients</span></span>](invalidrecipients.md) <br/> |<span data-ttu-id="943e9-126">Representa os destinatários de uma solicitação de compartilhamento de pasta que são inválidas.</span><span class="sxs-lookup"><span data-stu-id="943e9-126">Represents the recipients of a folder sharing request that are invalid.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="943e9-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="943e9-127">Remarks</span></span>

<span data-ttu-id="943e9-128">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="943e9-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="943e9-129">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="943e9-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="943e9-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="943e9-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="943e9-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="943e9-131">Schema Name</span></span>  <br/> |<span data-ttu-id="943e9-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="943e9-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="943e9-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="943e9-133">Validation File</span></span>  <br/> |<span data-ttu-id="943e9-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="943e9-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="943e9-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="943e9-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="943e9-136">False</span><span class="sxs-lookup"><span data-stu-id="943e9-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="943e9-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="943e9-137">See also</span></span>



[<span data-ttu-id="943e9-138">Operação GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="943e9-138">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="943e9-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="943e9-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

