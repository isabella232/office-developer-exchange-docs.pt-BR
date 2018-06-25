---
title: ReplyBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReplyBody
api_type:
- schema
ms.assetid: bb184144-3e4b-4419-a883-cc9fab1085e6
description: O elemento ReplyBody contém uma mensagem de fora do escritório (OOF) e o idioma usado para a mensagem.
ms.openlocfilehash: 8400dda1ee810781e129fcc44fd3cd5d6c15cbbe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825116"
---
# <a name="replybody"></a><span data-ttu-id="72e4f-103">ReplyBody</span><span class="sxs-lookup"><span data-stu-id="72e4f-103">ReplyBody</span></span>

<span data-ttu-id="72e4f-104">O elemento **ReplyBody** contém uma mensagem de fora do escritório (OOF) e o idioma usado para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="72e4f-104">The **ReplyBody** element contains an Out of Office (OOF) message and the language used for the message.</span></span> 
  
```XML
<ReplyBody xml:lang="">
   <Message/>
</ReplyBody>
```

 <span data-ttu-id="72e4f-105">**ReplyBody**</span><span class="sxs-lookup"><span data-stu-id="72e4f-105">**ReplyBody**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="72e4f-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="72e4f-106">Attributes and elements</span></span>

<span data-ttu-id="72e4f-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="72e4f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="72e4f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="72e4f-108">Attributes</span></span>

|<span data-ttu-id="72e4f-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="72e4f-109">**Attribute**</span></span>|<span data-ttu-id="72e4f-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="72e4f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="72e4f-111">XML: lang</span><span class="sxs-lookup"><span data-stu-id="72e4f-111">xml:lang</span></span>  <br/> |<span data-ttu-id="72e4f-112">Especifica o idioma usado no conteúdo da **ReplyBody** .</span><span class="sxs-lookup"><span data-stu-id="72e4f-112">Specifies the language used in the **ReplyBody** contents.</span></span> <span data-ttu-id="72e4f-113">Este atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="72e4f-113">This attribute is optional.</span></span> <span data-ttu-id="72e4f-114">Os valores possíveis desse atributo são definidos por IETF RFC 3066.</span><span class="sxs-lookup"><span data-stu-id="72e4f-114">The possible values of this attribute are defined by IETF RFC 3066.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="72e4f-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="72e4f-115">Child elements</span></span>

|<span data-ttu-id="72e4f-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="72e4f-116">**Element**</span></span>|<span data-ttu-id="72e4f-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="72e4f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="72e4f-118">Mensagem (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="72e4f-118">Message (Availability)</span></span>](message-availability.md) <br/> |<span data-ttu-id="72e4f-119">Contém o limite de resposta de ausência temporária.</span><span class="sxs-lookup"><span data-stu-id="72e4f-119">Contains the out of office (OOF) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="72e4f-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="72e4f-120">Parent elements</span></span>

|<span data-ttu-id="72e4f-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="72e4f-121">**Element**</span></span>|<span data-ttu-id="72e4f-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="72e4f-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="72e4f-123">Fora do escritório</span><span class="sxs-lookup"><span data-stu-id="72e4f-123">OutOfOffice</span></span>](outofoffice.md) <br/> |<span data-ttu-id="72e4f-124">Define a mensagem de resposta de ausência temporária e um tempo de duração para enviar a mensagem de resposta para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="72e4f-124">Defines the OOF response message and a duration time for sending the response message for a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="72e4f-125">Text value</span><span class="sxs-lookup"><span data-stu-id="72e4f-125">Text value</span></span>

<span data-ttu-id="72e4f-126">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="72e4f-126">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="72e4f-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="72e4f-127">Remarks</span></span>

<span data-ttu-id="72e4f-128">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="72e4f-128">This element is required.</span></span>
  
<span data-ttu-id="72e4f-129">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="72e4f-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="72e4f-130">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="72e4f-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="72e4f-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="72e4f-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="72e4f-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="72e4f-132">Schema Name</span></span>  <br/> |<span data-ttu-id="72e4f-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="72e4f-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="72e4f-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="72e4f-134">Validation File</span></span>  <br/> |<span data-ttu-id="72e4f-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="72e4f-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="72e4f-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="72e4f-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="72e4f-137">False</span><span class="sxs-lookup"><span data-stu-id="72e4f-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="72e4f-138">Ver também</span><span class="sxs-lookup"><span data-stu-id="72e4f-138">See also</span></span>



- [<span data-ttu-id="72e4f-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="72e4f-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

