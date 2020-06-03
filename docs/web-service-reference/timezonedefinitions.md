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
ms.openlocfilehash: 16a25eb4fdcad2554ebd19626d0a0bc7f6391ac5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468758"
---
# <a name="timezonedefinitions"></a><span data-ttu-id="54f0f-103">TimeZoneDefinitions</span><span class="sxs-lookup"><span data-stu-id="54f0f-103">TimeZoneDefinitions</span></span>

<span data-ttu-id="54f0f-104">O elemento **TimeZoneDefinitions** representa uma matriz de definições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="54f0f-104">The **TimeZoneDefinitions** element represents an array of time zone definitions.</span></span> 
  
```XML
<TimeZoneDefinitions>
   <TimeZoneDefinition/>
</TimeZoneDefinitions>
```

 <span data-ttu-id="54f0f-105">**ArrayOfTimeZoneDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="54f0f-105">**ArrayOfTimeZoneDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="54f0f-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="54f0f-106">Attributes and elements</span></span>

<span data-ttu-id="54f0f-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="54f0f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="54f0f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="54f0f-108">Attributes</span></span>

<span data-ttu-id="54f0f-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="54f0f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="54f0f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="54f0f-110">Child elements</span></span>

|<span data-ttu-id="54f0f-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="54f0f-111">**Element**</span></span>|<span data-ttu-id="54f0f-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="54f0f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54f0f-113">TimeZoneDefinition</span><span class="sxs-lookup"><span data-stu-id="54f0f-113">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="54f0f-114">Especifica os períodos e as transições que definem um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="54f0f-114">Specifies the periods and transitions that define a time zone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="54f0f-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="54f0f-115">Parent elements</span></span>

|<span data-ttu-id="54f0f-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="54f0f-116">**Element**</span></span>|<span data-ttu-id="54f0f-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="54f0f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54f0f-118">GetServerTimeZonesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="54f0f-118">GetServerTimeZonesResponseMessage</span></span>](getservertimezonesresponsemessage.md) <br/> |<span data-ttu-id="54f0f-119">Contém o status e o resultado de uma solicitação de [operação GetServerTimeZones](getservertimezones-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="54f0f-119">Contains the status and result of a [GetServerTimeZones operation](getservertimezones-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="54f0f-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="54f0f-120">Remarks</span></span>

<span data-ttu-id="54f0f-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="54f0f-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="54f0f-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="54f0f-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="54f0f-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="54f0f-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="54f0f-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="54f0f-124">Schema Name</span></span>  <br/> |<span data-ttu-id="54f0f-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="54f0f-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="54f0f-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="54f0f-126">Validation File</span></span>  <br/> |<span data-ttu-id="54f0f-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="54f0f-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="54f0f-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="54f0f-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="54f0f-129">False</span><span class="sxs-lookup"><span data-stu-id="54f0f-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="54f0f-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="54f0f-130">See also</span></span>



- [<span data-ttu-id="54f0f-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="54f0f-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

