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
description: O elemento ReplyBody contém uma mensagem de ausência temporária (OOF) e o idioma usado para a mensagem.
ms.openlocfilehash: 496d336d1f87d9ea493ba7da362eef5a416fd899
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465300"
---
# <a name="replybody"></a><span data-ttu-id="90ee2-103">ReplyBody</span><span class="sxs-lookup"><span data-stu-id="90ee2-103">ReplyBody</span></span>

<span data-ttu-id="90ee2-104">O elemento **ReplyBody** contém uma mensagem de ausência temporária (OOF) e o idioma usado para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="90ee2-104">The **ReplyBody** element contains an Out of Office (OOF) message and the language used for the message.</span></span> 
  
```XML
<ReplyBody xml:lang="">
   <Message/>
</ReplyBody>
```

 <span data-ttu-id="90ee2-105">**ReplyBody**</span><span class="sxs-lookup"><span data-stu-id="90ee2-105">**ReplyBody**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="90ee2-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="90ee2-106">Attributes and elements</span></span>

<span data-ttu-id="90ee2-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="90ee2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="90ee2-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="90ee2-108">Attributes</span></span>

|<span data-ttu-id="90ee2-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="90ee2-109">**Attribute**</span></span>|<span data-ttu-id="90ee2-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="90ee2-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="90ee2-111">XML: lang</span><span class="sxs-lookup"><span data-stu-id="90ee2-111">xml:lang</span></span>  <br/> |<span data-ttu-id="90ee2-112">Especifica o idioma usado no conteúdo do **ReplyBody** .</span><span class="sxs-lookup"><span data-stu-id="90ee2-112">Specifies the language used in the **ReplyBody** contents.</span></span> <span data-ttu-id="90ee2-113">Esse atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="90ee2-113">This attribute is optional.</span></span> <span data-ttu-id="90ee2-114">Os valores possíveis desse atributo são definidos pela IETF RFC 3066.</span><span class="sxs-lookup"><span data-stu-id="90ee2-114">The possible values of this attribute are defined by IETF RFC 3066.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="90ee2-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="90ee2-115">Child elements</span></span>

|<span data-ttu-id="90ee2-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="90ee2-116">**Element**</span></span>|<span data-ttu-id="90ee2-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="90ee2-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="90ee2-118">Mensagem (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="90ee2-118">Message (Availability)</span></span>](message-availability.md) <br/> |<span data-ttu-id="90ee2-119">Contém a resposta de ausência temporária (OOF).</span><span class="sxs-lookup"><span data-stu-id="90ee2-119">Contains the out of office (OOF) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="90ee2-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="90ee2-120">Parent elements</span></span>

|<span data-ttu-id="90ee2-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="90ee2-121">**Element**</span></span>|<span data-ttu-id="90ee2-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="90ee2-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="90ee2-123">Fora</span><span class="sxs-lookup"><span data-stu-id="90ee2-123">OutOfOffice</span></span>](outofoffice.md) <br/> |<span data-ttu-id="90ee2-124">Define a mensagem de resposta de ausência temporária e um tempo de duração para enviar a mensagem de resposta para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="90ee2-124">Defines the OOF response message and a duration time for sending the response message for a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="90ee2-125">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="90ee2-125">Text value</span></span>

<span data-ttu-id="90ee2-126">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="90ee2-126">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="90ee2-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="90ee2-127">Remarks</span></span>

<span data-ttu-id="90ee2-128">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90ee2-128">This element is required.</span></span>
  
<span data-ttu-id="90ee2-129">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="90ee2-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="90ee2-130">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="90ee2-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="90ee2-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="90ee2-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="90ee2-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="90ee2-132">Schema Name</span></span>  <br/> |<span data-ttu-id="90ee2-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="90ee2-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="90ee2-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="90ee2-134">Validation File</span></span>  <br/> |<span data-ttu-id="90ee2-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="90ee2-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="90ee2-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="90ee2-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="90ee2-137">False</span><span class="sxs-lookup"><span data-stu-id="90ee2-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="90ee2-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="90ee2-138">See also</span></span>



- [<span data-ttu-id="90ee2-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="90ee2-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

