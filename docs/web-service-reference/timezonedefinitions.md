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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468758"
---
# <a name="timezonedefinitions"></a><span data-ttu-id="f4995-103">TimeZoneDefinitions</span><span class="sxs-lookup"><span data-stu-id="f4995-103">TimeZoneDefinitions</span></span>

<span data-ttu-id="f4995-104">O elemento **TimeZoneDefinitions** representa uma matriz de definições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="f4995-104">The **TimeZoneDefinitions** element represents an array of time zone definitions.</span></span> 
  
```XML
<TimeZoneDefinitions>
   <TimeZoneDefinition/>
</TimeZoneDefinitions>
```

 <span data-ttu-id="f4995-105">**ArrayOfTimeZoneDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="f4995-105">**ArrayOfTimeZoneDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f4995-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="f4995-106">Attributes and elements</span></span>

<span data-ttu-id="f4995-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f4995-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f4995-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f4995-108">Attributes</span></span>

<span data-ttu-id="f4995-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f4995-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f4995-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f4995-110">Child elements</span></span>

|<span data-ttu-id="f4995-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f4995-111">**Element**</span></span>|<span data-ttu-id="f4995-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f4995-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f4995-113">TimeZoneDefinition</span><span class="sxs-lookup"><span data-stu-id="f4995-113">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="f4995-114">Especifica os períodos e as transições que definem um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="f4995-114">Specifies the periods and transitions that define a time zone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f4995-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f4995-115">Parent elements</span></span>

|<span data-ttu-id="f4995-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f4995-116">**Element**</span></span>|<span data-ttu-id="f4995-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f4995-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f4995-118">GetServerTimeZonesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f4995-118">GetServerTimeZonesResponseMessage</span></span>](getservertimezonesresponsemessage.md) <br/> |<span data-ttu-id="f4995-119">Contém o status e o resultado de uma solicitação de [operação GetServerTimeZones](getservertimezones-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="f4995-119">Contains the status and result of a [GetServerTimeZones operation](getservertimezones-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f4995-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="f4995-120">Remarks</span></span>

<span data-ttu-id="f4995-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f4995-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f4995-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="f4995-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f4995-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="f4995-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f4995-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f4995-124">Schema Name</span></span>  <br/> |<span data-ttu-id="f4995-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="f4995-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f4995-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f4995-126">Validation File</span></span>  <br/> |<span data-ttu-id="f4995-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f4995-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f4995-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f4995-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="f4995-129">False</span><span class="sxs-lookup"><span data-stu-id="f4995-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f4995-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="f4995-130">See also</span></span>



- [<span data-ttu-id="f4995-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f4995-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

