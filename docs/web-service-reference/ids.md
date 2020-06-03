---
title: Código
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Ids
api_type:
- schema
ms.assetid: c54cdeaf-6761-4d1a-a329-fb279f0e2a64
description: O elemento IDs contém uma matriz de identificadores de definição de fuso horário.
ms.openlocfilehash: 1c5a6974c8d3abc318ff122f3db09d8c3472dc65
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457617"
---
# <a name="ids"></a><span data-ttu-id="3b339-103">Código</span><span class="sxs-lookup"><span data-stu-id="3b339-103">Ids</span></span>

<span data-ttu-id="3b339-104">O elemento **IDs** contém uma matriz de identificadores de definição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="3b339-104">The **Ids** element contains an array of time zone definition identifiers.</span></span> 
  
```XML
<Ids>
   <Id/>
</Ids>
```

 <span data-ttu-id="3b339-105">**NonEmptyArrayOfTimeZoneIdType**</span><span class="sxs-lookup"><span data-stu-id="3b339-105">**NonEmptyArrayOfTimeZoneIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3b339-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="3b339-106">Attributes and elements</span></span>

<span data-ttu-id="3b339-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3b339-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3b339-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3b339-108">Attributes</span></span>

<span data-ttu-id="3b339-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3b339-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3b339-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3b339-110">Child elements</span></span>

|<span data-ttu-id="3b339-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3b339-111">**Element**</span></span>|<span data-ttu-id="3b339-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3b339-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3b339-113">ID (TimeZone)</span><span class="sxs-lookup"><span data-stu-id="3b339-113">Id (TimeZone)</span></span>](id-timezone.md) <br/> |<span data-ttu-id="3b339-114">O elemento que identifica uma única definição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="3b339-114">The element that identifies a single time zone definition.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3b339-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3b339-115">Parent elements</span></span>

|<span data-ttu-id="3b339-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3b339-116">**Element**</span></span>|<span data-ttu-id="3b339-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3b339-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3b339-118">GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="3b339-118">GetServerTimeZones</span></span>](getservertimezones.md) <br/> |<span data-ttu-id="3b339-119">Define uma solicitação para recuperar definições de fuso horário do Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="3b339-119">Defines a request to retrieve time zone definitions from the Exchange server.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="3b339-120">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="3b339-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3b339-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="3b339-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3b339-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3b339-122">Schema Name</span></span>  <br/> |<span data-ttu-id="3b339-123">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="3b339-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3b339-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3b339-124">Validation File</span></span>  <br/> |<span data-ttu-id="3b339-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3b339-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3b339-126">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3b339-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="3b339-127">False</span><span class="sxs-lookup"><span data-stu-id="3b339-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3b339-128">Confira também</span><span class="sxs-lookup"><span data-stu-id="3b339-128">See also</span></span>



- [<span data-ttu-id="3b339-129">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3b339-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

