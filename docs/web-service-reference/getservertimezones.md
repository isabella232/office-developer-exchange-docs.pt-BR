---
title: GetServerTimeZones
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServerTimeZones
api_type:
- schema
ms.assetid: 2a89098b-d89b-4d01-827b-50be00f7cbe9
description: O GetServerTimeZones é o elemento raiz em uma solicitação para recuperar as definições de fuso horário do servidor Exchange.
ms.openlocfilehash: 1ad503ff312497189f57bce9a3670571aedad5ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752630"
---
# <a name="getservertimezones"></a><span data-ttu-id="608c8-103">GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="608c8-103">GetServerTimeZones</span></span>

<span data-ttu-id="608c8-104">O **GetServerTimeZones** é o elemento raiz em uma solicitação para recuperar as definições de fuso horário do servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="608c8-104">The **GetServerTimeZones** element is the root element in a request to retrieve time zone definitions from the Exchange server.</span></span> 
  
```xml
<GetServerTimeZones ReturnFullTimeZoneData="">   <Ids/></GetServerTimeZones>
```

 <span data-ttu-id="608c8-105">**GetServerTimeZonesType**</span><span class="sxs-lookup"><span data-stu-id="608c8-105">**GetServerTimeZonesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="608c8-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="608c8-106">Attributes and elements</span></span>

<span data-ttu-id="608c8-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="608c8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="608c8-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="608c8-108">Attributes</span></span>

|<span data-ttu-id="608c8-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="608c8-109">**Attribute**</span></span>|<span data-ttu-id="608c8-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="608c8-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="608c8-111">**ReturnFullTimeZoneData**</span><span class="sxs-lookup"><span data-stu-id="608c8-111">**ReturnFullTimeZoneData**</span></span> <br/> |<span data-ttu-id="608c8-112">Especifica se a [operação GetServerTimeZones](getservertimezones-operation.md) retorna a definição completa ou apenas o nome e o identificador de cada fuso horário.</span><span class="sxs-lookup"><span data-stu-id="608c8-112">Specifies whether the [GetServerTimeZones operation](getservertimezones-operation.md) returns the complete definition or only the name and identifier for each time zone.</span></span> <span data-ttu-id="608c8-113">Este atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="608c8-113">This attribute is optional.</span></span> <span data-ttu-id="608c8-114">O valor padrão é **true**.</span><span class="sxs-lookup"><span data-stu-id="608c8-114">The default value is **true**.</span></span>  <br/> |
   
#### <a name="returnfulltimezonedata-attribute"></a><span data-ttu-id="608c8-115">Atributo ReturnFullTimeZoneData</span><span class="sxs-lookup"><span data-stu-id="608c8-115">ReturnFullTimeZoneData Attribute</span></span>

|<span data-ttu-id="608c8-116">**Valor**</span><span class="sxs-lookup"><span data-stu-id="608c8-116">**Value**</span></span>|<span data-ttu-id="608c8-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="608c8-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="608c8-118">**True**</span><span class="sxs-lookup"><span data-stu-id="608c8-118">**true**</span></span> <br/> |<span data-ttu-id="608c8-119">Retorne as definições de completas para cada fuso horário.</span><span class="sxs-lookup"><span data-stu-id="608c8-119">Return the complete definitions for each time zone.</span></span>  <br/> |
|<span data-ttu-id="608c8-120">**False**</span><span class="sxs-lookup"><span data-stu-id="608c8-120">**false**</span></span> <br/> |<span data-ttu-id="608c8-121">Retorne somente o nome e o identificador de cada fuso horário.</span><span class="sxs-lookup"><span data-stu-id="608c8-121">Return only the name and identifier for each time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="608c8-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="608c8-122">Child elements</span></span>

|<span data-ttu-id="608c8-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="608c8-123">**Element**</span></span>|<span data-ttu-id="608c8-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="608c8-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="608c8-125">IDs</span><span class="sxs-lookup"><span data-stu-id="608c8-125">Ids</span></span>](ids.md) <br/> |<span data-ttu-id="608c8-126">Contém uma matriz de identificadores de definição de fuso horário que especifica as definições de fuso solicitada.</span><span class="sxs-lookup"><span data-stu-id="608c8-126">Contains an array of time zone definition identifiers that specifies the requested time zone definitions.</span></span> <span data-ttu-id="608c8-127">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="608c8-127">This element is optional.</span></span> <span data-ttu-id="608c8-128">Se esse elemento não estiver incluído na solicitação de [operação GetServerTimeZones](getservertimezones-operation.md) , todas as definições de fuso horário que estão disponíveis no servidor são retornadas na resposta.</span><span class="sxs-lookup"><span data-stu-id="608c8-128">If this element is not included in the [GetServerTimeZones operation](getservertimezones-operation.md) request, all time zone definitions that are available on the server are returned in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="608c8-129">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="608c8-129">Parent elements</span></span>

<span data-ttu-id="608c8-130">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="608c8-130">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="608c8-131">Comentários</span><span class="sxs-lookup"><span data-stu-id="608c8-131">Remarks</span></span>

<span data-ttu-id="608c8-132">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="608c8-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="608c8-133">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="608c8-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="608c8-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="608c8-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="608c8-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="608c8-135">Schema Name</span></span>  <br/> |<span data-ttu-id="608c8-136">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="608c8-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="608c8-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="608c8-137">Validation File</span></span>  <br/> |<span data-ttu-id="608c8-138">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="608c8-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="608c8-139">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="608c8-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="608c8-140">False</span><span class="sxs-lookup"><span data-stu-id="608c8-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="608c8-141">Ver também</span><span class="sxs-lookup"><span data-stu-id="608c8-141">See also</span></span>



[<span data-ttu-id="608c8-142">Operação GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="608c8-142">GetServerTimeZones operation</span></span>](getservertimezones-operation.md)
  
[<span data-ttu-id="608c8-143">GetServerTimeZonesResponse</span><span class="sxs-lookup"><span data-stu-id="608c8-143">GetServerTimeZonesResponse</span></span>](getservertimezonesresponse.md)


- [<span data-ttu-id="608c8-144">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="608c8-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

