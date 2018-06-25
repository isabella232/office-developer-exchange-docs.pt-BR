---
title: TimeZoneDefinitions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeZoneDefinitions
api_type:
- schema
ms.assetid: 9ca1584e-65b8-49ba-a408-e3e8597e6607
description: O elemento TimeZoneDefinitions representa uma matriz de definições de fuso horário.
ms.openlocfilehash: 0bc1b69ef564bb4e239d9845a4b1a0133292ff12
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837750"
---
# <a name="timezonedefinitions"></a><span data-ttu-id="2d1b4-103">TimeZoneDefinitions</span><span class="sxs-lookup"><span data-stu-id="2d1b4-103">TimeZoneDefinitions</span></span>

<span data-ttu-id="2d1b4-104">O elemento **TimeZoneDefinitions** representa uma matriz de definições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="2d1b4-104">The **TimeZoneDefinitions** element represents an array of time zone definitions.</span></span> 
  
```XML
<TimeZoneDefinitions>
   <TimeZoneDefinition/>
</TimeZoneDefinitions>
```

 <span data-ttu-id="2d1b4-105">**ArrayOfTimeZoneDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="2d1b4-105">**ArrayOfTimeZoneDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2d1b4-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="2d1b4-106">Attributes and elements</span></span>

<span data-ttu-id="2d1b4-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2d1b4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2d1b4-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2d1b4-108">Attributes</span></span>

<span data-ttu-id="2d1b4-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2d1b4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2d1b4-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2d1b4-110">Child elements</span></span>

|<span data-ttu-id="2d1b4-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2d1b4-111">**Element**</span></span>|<span data-ttu-id="2d1b4-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2d1b4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2d1b4-113">Timezonedefinition pela última vez</span><span class="sxs-lookup"><span data-stu-id="2d1b4-113">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="2d1b4-114">Especifica os períodos e transições que definem um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="2d1b4-114">Specifies the periods and transitions that define a time zone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2d1b4-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2d1b4-115">Parent elements</span></span>

|<span data-ttu-id="2d1b4-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2d1b4-116">**Element**</span></span>|<span data-ttu-id="2d1b4-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2d1b4-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2d1b4-118">GetServerTimeZonesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="2d1b4-118">GetServerTimeZonesResponseMessage</span></span>](getservertimezonesresponsemessage.md) <br/> |<span data-ttu-id="2d1b4-119">Contém o status e o resultado de uma solicitação de [operação GetServerTimeZones](getservertimezones-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="2d1b4-119">Contains the status and result of a [GetServerTimeZones operation](getservertimezones-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2d1b4-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="2d1b4-120">Remarks</span></span>

<span data-ttu-id="2d1b4-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2d1b4-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2d1b4-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="2d1b4-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2d1b4-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="2d1b4-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2d1b4-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2d1b4-124">Schema Name</span></span>  <br/> |<span data-ttu-id="2d1b4-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="2d1b4-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2d1b4-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2d1b4-126">Validation File</span></span>  <br/> |<span data-ttu-id="2d1b4-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2d1b4-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2d1b4-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="2d1b4-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="2d1b4-129">False</span><span class="sxs-lookup"><span data-stu-id="2d1b4-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2d1b4-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="2d1b4-130">See also</span></span>



- [<span data-ttu-id="2d1b4-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2d1b4-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

