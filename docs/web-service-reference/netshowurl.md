---
title: NetShowUrl
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NetShowUrl
api_type:
- schema
ms.assetid: a5d48fc1-b141-422c-bcb0-05d0f9ba90dd
description: O elemento NetShowUrl especifica a URL para uma reunião online do Microsoft NetShow.
ms.openlocfilehash: 66e288a5e66eecf404698135cc3257085b852034
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466329"
---
# <a name="netshowurl"></a><span data-ttu-id="58626-103">NetShowUrl</span><span class="sxs-lookup"><span data-stu-id="58626-103">NetShowUrl</span></span>

<span data-ttu-id="58626-104">O elemento **NetShowUrl** especifica a URL para uma reunião online do Microsoft NetShow.</span><span class="sxs-lookup"><span data-stu-id="58626-104">The **NetShowUrl** element specifies the URL for a Microsoft NetShow online meeting.</span></span> 
  
```xml
<NetShowUrl/>
```

 <span data-ttu-id="58626-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="58626-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="58626-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="58626-106">Attributes and elements</span></span>

<span data-ttu-id="58626-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="58626-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="58626-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="58626-108">Attributes</span></span>

<span data-ttu-id="58626-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="58626-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="58626-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="58626-110">Child elements</span></span>

<span data-ttu-id="58626-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="58626-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="58626-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="58626-112">Parent elements</span></span>

|<span data-ttu-id="58626-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="58626-113">**Element**</span></span>|<span data-ttu-id="58626-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="58626-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="58626-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="58626-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="58626-116">Representa uma reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="58626-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="58626-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="58626-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="58626-118">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="58626-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="58626-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="58626-119">Text value</span></span>

<span data-ttu-id="58626-120">Um valor de texto que representa uma URL será necessário se esse elemento for usado.</span><span class="sxs-lookup"><span data-stu-id="58626-120">A text value that represents a URL is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="58626-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="58626-121">Remarks</span></span>

<span data-ttu-id="58626-122">Esta propriedade NetShowUrl é leitura/gravação para o item de calendário do organizador.</span><span class="sxs-lookup"><span data-stu-id="58626-122">This NetShowUrl property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="58626-123">É somente leitura para solicitações de reunião e participantes.</span><span class="sxs-lookup"><span data-stu-id="58626-123">It is read-only for meeting requests and for attendees.</span></span>
  
<span data-ttu-id="58626-124">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="58626-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="58626-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="58626-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="58626-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="58626-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="58626-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="58626-127">Schema name</span></span>  <br/> |<span data-ttu-id="58626-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="58626-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="58626-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="58626-129">Validation file</span></span>  <br/> |<span data-ttu-id="58626-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="58626-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="58626-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="58626-131">Can be empty</span></span>  <br/> |<span data-ttu-id="58626-132">False</span><span class="sxs-lookup"><span data-stu-id="58626-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="58626-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="58626-133">See also</span></span>



- [<span data-ttu-id="58626-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="58626-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

