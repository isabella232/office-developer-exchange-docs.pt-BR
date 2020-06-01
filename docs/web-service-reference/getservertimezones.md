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
description: O elemento GetServerTimeZones é o elemento raiz em uma solicitação para recuperar definições de fuso horário do Exchange Server.
ms.openlocfilehash: 797e4543c94b0628242bcf544fe9a735ebaa5a63
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460936"
---
# <a name="getservertimezones"></a><span data-ttu-id="f008e-103">GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="f008e-103">GetServerTimeZones</span></span>

<span data-ttu-id="f008e-104">O elemento **GetServerTimeZones** é o elemento raiz em uma solicitação para recuperar definições de fuso horário do Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="f008e-104">The **GetServerTimeZones** element is the root element in a request to retrieve time zone definitions from the Exchange server.</span></span> 
  
```xml
<GetServerTimeZones ReturnFullTimeZoneData="">   <Ids/></GetServerTimeZones>
```

 <span data-ttu-id="f008e-105">**GetServerTimeZonesType**</span><span class="sxs-lookup"><span data-stu-id="f008e-105">**GetServerTimeZonesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f008e-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="f008e-106">Attributes and elements</span></span>

<span data-ttu-id="f008e-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f008e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f008e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f008e-108">Attributes</span></span>

|<span data-ttu-id="f008e-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="f008e-109">**Attribute**</span></span>|<span data-ttu-id="f008e-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f008e-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f008e-111">**ReturnFullTimeZoneData**</span><span class="sxs-lookup"><span data-stu-id="f008e-111">**ReturnFullTimeZoneData**</span></span> <br/> |<span data-ttu-id="f008e-112">Especifica se a [operação GetServerTimeZones](getservertimezones-operation.md) retorna a definição completa ou apenas o nome e o identificador de cada fuso horário.</span><span class="sxs-lookup"><span data-stu-id="f008e-112">Specifies whether the [GetServerTimeZones operation](getservertimezones-operation.md) returns the complete definition or only the name and identifier for each time zone.</span></span> <span data-ttu-id="f008e-113">Esse atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="f008e-113">This attribute is optional.</span></span> <span data-ttu-id="f008e-114">O valor padrão é **true**.</span><span class="sxs-lookup"><span data-stu-id="f008e-114">The default value is **true**.</span></span>  <br/> |
   
#### <a name="returnfulltimezonedata-attribute"></a><span data-ttu-id="f008e-115">Atributo ReturnFullTimeZoneData</span><span class="sxs-lookup"><span data-stu-id="f008e-115">ReturnFullTimeZoneData Attribute</span></span>

|<span data-ttu-id="f008e-116">**Valor**</span><span class="sxs-lookup"><span data-stu-id="f008e-116">**Value**</span></span>|<span data-ttu-id="f008e-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f008e-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f008e-118">**verdadeiro**</span><span class="sxs-lookup"><span data-stu-id="f008e-118">**true**</span></span> <br/> |<span data-ttu-id="f008e-119">Retorna as definições completas de cada fuso horário.</span><span class="sxs-lookup"><span data-stu-id="f008e-119">Return the complete definitions for each time zone.</span></span>  <br/> |
|<span data-ttu-id="f008e-120">**false**</span><span class="sxs-lookup"><span data-stu-id="f008e-120">**false**</span></span> <br/> |<span data-ttu-id="f008e-121">Retornar apenas o nome e o identificador de cada fuso horário.</span><span class="sxs-lookup"><span data-stu-id="f008e-121">Return only the name and identifier for each time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f008e-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f008e-122">Child elements</span></span>

|<span data-ttu-id="f008e-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f008e-123">**Element**</span></span>|<span data-ttu-id="f008e-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f008e-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f008e-125">Código</span><span class="sxs-lookup"><span data-stu-id="f008e-125">Ids</span></span>](ids.md) <br/> |<span data-ttu-id="f008e-126">Contém uma matriz de identificadores de definição de fuso horário que especifica as definições de fuso horário solicitadas.</span><span class="sxs-lookup"><span data-stu-id="f008e-126">Contains an array of time zone definition identifiers that specifies the requested time zone definitions.</span></span> <span data-ttu-id="f008e-127">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="f008e-127">This element is optional.</span></span> <span data-ttu-id="f008e-128">Se esse elemento não estiver incluído na solicitação de [operação GetServerTimeZones](getservertimezones-operation.md) , todas as definições de fuso horário disponíveis no servidor serão retornadas na resposta.</span><span class="sxs-lookup"><span data-stu-id="f008e-128">If this element is not included in the [GetServerTimeZones operation](getservertimezones-operation.md) request, all time zone definitions that are available on the server are returned in the response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f008e-129">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f008e-129">Parent elements</span></span>

<span data-ttu-id="f008e-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f008e-130">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f008e-131">Comentários</span><span class="sxs-lookup"><span data-stu-id="f008e-131">Remarks</span></span>

<span data-ttu-id="f008e-132">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="f008e-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f008e-133">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="f008e-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f008e-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="f008e-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f008e-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f008e-135">Schema Name</span></span>  <br/> |<span data-ttu-id="f008e-136">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="f008e-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f008e-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f008e-137">Validation File</span></span>  <br/> |<span data-ttu-id="f008e-138">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f008e-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f008e-139">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f008e-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="f008e-140">False</span><span class="sxs-lookup"><span data-stu-id="f008e-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f008e-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="f008e-141">See also</span></span>



[<span data-ttu-id="f008e-142">Operação GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="f008e-142">GetServerTimeZones operation</span></span>](getservertimezones-operation.md)
  
[<span data-ttu-id="f008e-143">GetServerTimeZonesResponse</span><span class="sxs-lookup"><span data-stu-id="f008e-143">GetServerTimeZonesResponse</span></span>](getservertimezonesresponse.md)


- [<span data-ttu-id="f008e-144">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f008e-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

