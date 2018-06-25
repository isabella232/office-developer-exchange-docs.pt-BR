---
title: AppointmentSequenceNumber
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AppointmentSequenceNumber
api_type:
- schema
ms.assetid: eb4c48bd-f905-48dc-ae16-53a080b9b025
description: O elemento AppointmentSequenceNumber Especifica o número de sequência de uma versão de um compromisso.
ms.openlocfilehash: bc186170ccca06669ea7d20cea06c542f9ce274a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751188"
---
# <a name="appointmentsequencenumber"></a><span data-ttu-id="ce30d-103">AppointmentSequenceNumber</span><span class="sxs-lookup"><span data-stu-id="ce30d-103">AppointmentSequenceNumber</span></span>

<span data-ttu-id="ce30d-104">O elemento **AppointmentSequenceNumber** Especifica o número de sequência de uma versão de um compromisso.</span><span class="sxs-lookup"><span data-stu-id="ce30d-104">The **AppointmentSequenceNumber** element specifies the sequence number of a version of an appointment.</span></span> 
  
```xml
<AppointmentSequenceNumber/>
```

 <span data-ttu-id="ce30d-105">**int**</span><span class="sxs-lookup"><span data-stu-id="ce30d-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ce30d-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ce30d-106">Attributes and elements</span></span>

<span data-ttu-id="ce30d-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ce30d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ce30d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ce30d-108">Attributes</span></span>

<span data-ttu-id="ce30d-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ce30d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ce30d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ce30d-110">Child elements</span></span>

<span data-ttu-id="ce30d-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ce30d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ce30d-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ce30d-112">Parent elements</span></span>

|<span data-ttu-id="ce30d-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ce30d-113">**Element**</span></span>|<span data-ttu-id="ce30d-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ce30d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ce30d-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="ce30d-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="ce30d-116">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce30d-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ce30d-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="ce30d-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="ce30d-118">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce30d-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ce30d-119">Text value</span><span class="sxs-lookup"><span data-stu-id="ce30d-119">Text value</span></span>

<span data-ttu-id="ce30d-120">O valor de texto representa um número de versão.</span><span class="sxs-lookup"><span data-stu-id="ce30d-120">The text value represents a version number.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ce30d-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="ce30d-121">Remarks</span></span>

<span data-ttu-id="ce30d-122">Esse valor é atualizado quando o compromisso é atualizado com novas informações.</span><span class="sxs-lookup"><span data-stu-id="ce30d-122">This value is updated when the appointment is updated with new information.</span></span> 
  
<span data-ttu-id="ce30d-123">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="ce30d-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ce30d-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ce30d-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ce30d-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="ce30d-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ce30d-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ce30d-126">Schema Name</span></span>  <br/> |<span data-ttu-id="ce30d-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ce30d-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="ce30d-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ce30d-128">Validation File</span></span>  <br/> |<span data-ttu-id="ce30d-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ce30d-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ce30d-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ce30d-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="ce30d-131">False</span><span class="sxs-lookup"><span data-stu-id="ce30d-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ce30d-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="ce30d-132">See also</span></span>

- [<span data-ttu-id="ce30d-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ce30d-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

