---
title: OutOfOffice
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OutOfOffice
api_type:
- schema
ms.assetid: fe1256ab-5c0f-467d-abb3-b38a2dc312ae
description: O elemento de fora do escritório representa a mensagem de resposta e um tempo de duração para enviar a mensagem de resposta.
ms.openlocfilehash: f35b84d7a8a37c7a57b58c97fd0d37318bb50a33
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354264"
---
# <a name="outofoffice"></a><span data-ttu-id="692eb-103">OutOfOffice</span><span class="sxs-lookup"><span data-stu-id="692eb-103">OutOfOffice</span></span>

<span data-ttu-id="692eb-104">O elemento de **fora do escritório** representa a mensagem de resposta e um tempo de duração para enviar a mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="692eb-104">The **OutOfOffice** element represents the response message and a duration time for sending the response message.</span></span> 
  
```XML
<OutOfOffice>
   <ReplyBody/>
   <Duration/>
</OutOfOffice>
```

```XML
<OutOfOffice>
   <ReplyBody/>
</OutOfOffice>
```

<span data-ttu-id="692eb-105">**OutOfOfficeMailTip**</span><span class="sxs-lookup"><span data-stu-id="692eb-105">**OutOfOfficeMailTip**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="692eb-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="692eb-106">Attributes and elements</span></span>

<span data-ttu-id="692eb-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="692eb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="692eb-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="692eb-108">Attributes</span></span>

<span data-ttu-id="692eb-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="692eb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="692eb-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="692eb-110">Child elements</span></span>

|<span data-ttu-id="692eb-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="692eb-111">**Element**</span></span>|<span data-ttu-id="692eb-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="692eb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="692eb-113">ReplyBody</span><span class="sxs-lookup"><span data-stu-id="692eb-113">ReplyBody</span></span>](replybody.md) <br/> |<span data-ttu-id="692eb-114">Contém uma mensagem de fora do escritório (OOF) e o idioma usado para a mensagem.</span><span class="sxs-lookup"><span data-stu-id="692eb-114">Contains an Out of Office (OOF) message and the language used for the message.</span></span>  <br/> |
|[<span data-ttu-id="692eb-115">Duration (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="692eb-115">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> |<span data-ttu-id="692eb-116">Contém a duração em que o status de ausência temporária será habilitado se o elemento [OofState](oofstate.md) for definido como agendado.</span><span class="sxs-lookup"><span data-stu-id="692eb-116">Contains the duration that the OOF status is enabled if the [OofState](oofstate.md) element is set to Scheduled.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="692eb-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="692eb-117">Parent elements</span></span>

|<span data-ttu-id="692eb-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="692eb-118">**Element**</span></span>|<span data-ttu-id="692eb-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="692eb-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="692eb-120">MailTips</span><span class="sxs-lookup"><span data-stu-id="692eb-120">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="692eb-121">Representa os valores para os vários tipos de dicas de email.</span><span class="sxs-lookup"><span data-stu-id="692eb-121">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="692eb-122">Text value</span><span class="sxs-lookup"><span data-stu-id="692eb-122">Text value</span></span>

<span data-ttu-id="692eb-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="692eb-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="692eb-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="692eb-124">Remarks</span></span>

<span data-ttu-id="692eb-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="692eb-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="692eb-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="692eb-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="692eb-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="692eb-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="692eb-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="692eb-128">Schema Name</span></span>  <br/> |<span data-ttu-id="692eb-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="692eb-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="692eb-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="692eb-130">Validation File</span></span>  <br/> |<span data-ttu-id="692eb-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="692eb-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="692eb-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="692eb-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="692eb-133">False</span><span class="sxs-lookup"><span data-stu-id="692eb-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="692eb-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="692eb-134">See also</span></span>

- [<span data-ttu-id="692eb-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="692eb-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

