---
title: IDs
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
description: O elemento de Ids contém uma matriz de identificadores de definição de fuso horário.
ms.openlocfilehash: e4f8afb1292b3cb9f3990d4613b7461050976a59
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823856"
---
# <a name="ids"></a><span data-ttu-id="74022-103">IDs</span><span class="sxs-lookup"><span data-stu-id="74022-103">Ids</span></span>

<span data-ttu-id="74022-104">O elemento de **Ids** contém uma matriz de identificadores de definição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="74022-104">The **Ids** element contains an array of time zone definition identifiers.</span></span> 
  
```XML
<Ids>
   <Id/>
</Ids>
```

 <span data-ttu-id="74022-105">**NonEmptyArrayOfTimeZoneIdType**</span><span class="sxs-lookup"><span data-stu-id="74022-105">**NonEmptyArrayOfTimeZoneIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="74022-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="74022-106">Attributes and elements</span></span>

<span data-ttu-id="74022-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="74022-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="74022-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="74022-108">Attributes</span></span>

<span data-ttu-id="74022-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="74022-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="74022-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="74022-110">Child elements</span></span>

|<span data-ttu-id="74022-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="74022-111">**Element**</span></span>|<span data-ttu-id="74022-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="74022-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74022-113">ID (TimeZone)</span><span class="sxs-lookup"><span data-stu-id="74022-113">Id (TimeZone)</span></span>](id-timezone.md) <br/> |<span data-ttu-id="74022-114">O elemento que identifica a definição de um único fuso horário.</span><span class="sxs-lookup"><span data-stu-id="74022-114">The element that identifies a single time zone definition.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="74022-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="74022-115">Parent elements</span></span>

|<span data-ttu-id="74022-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="74022-116">**Element**</span></span>|<span data-ttu-id="74022-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="74022-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74022-118">GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="74022-118">GetServerTimeZones</span></span>](getservertimezones.md) <br/> |<span data-ttu-id="74022-119">Define uma solicitação para recuperar as definições de fuso horário do servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="74022-119">Defines a request to retrieve time zone definitions from the Exchange server.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="74022-120">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="74022-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="74022-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="74022-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="74022-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="74022-122">Schema Name</span></span>  <br/> |<span data-ttu-id="74022-123">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="74022-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="74022-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="74022-124">Validation File</span></span>  <br/> |<span data-ttu-id="74022-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="74022-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="74022-126">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="74022-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="74022-127">False</span><span class="sxs-lookup"><span data-stu-id="74022-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="74022-128">Ver também</span><span class="sxs-lookup"><span data-stu-id="74022-128">See also</span></span>



- [<span data-ttu-id="74022-129">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="74022-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

