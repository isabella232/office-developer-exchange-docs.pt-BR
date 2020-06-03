---
title: IsDelegated foi removida
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsDelegated
api_type:
- schema
ms.assetid: c12907db-be80-4924-9469-8e58612cf42c
description: O elemento IsDelegated indica se uma reunião foi tratada por uma conta que tenha acesso de representante.
ms.openlocfilehash: 2c62b59665431d5ea203e972a506aa90afc76601
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456441"
---
# <a name="isdelegated"></a><span data-ttu-id="92bba-103">IsDelegated foi removida</span><span class="sxs-lookup"><span data-stu-id="92bba-103">IsDelegated</span></span>

<span data-ttu-id="92bba-104">O elemento **IsDelegated** indica se uma reunião foi tratada por uma conta que tenha acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="92bba-104">The **IsDelegated** element indicates whether a meeting was handled by an account that has delegate access.</span></span> 
  
```xml
<IsDelegated/>
```

 <span data-ttu-id="92bba-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="92bba-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="92bba-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="92bba-106">Attributes and elements</span></span>

<span data-ttu-id="92bba-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="92bba-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="92bba-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="92bba-108">Attributes</span></span>

<span data-ttu-id="92bba-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="92bba-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="92bba-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="92bba-110">Child elements</span></span>

<span data-ttu-id="92bba-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="92bba-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="92bba-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="92bba-112">Parent elements</span></span>

|<span data-ttu-id="92bba-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="92bba-113">**Element**</span></span>|<span data-ttu-id="92bba-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="92bba-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="92bba-115">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="92bba-115">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="92bba-116">Representa um cancelamento de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="92bba-116">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="92bba-117">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="92bba-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="92bba-118">Representa uma reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="92bba-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="92bba-119">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="92bba-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="92bba-120">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="92bba-120">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="92bba-121">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="92bba-121">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="92bba-122">Representa uma resposta de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="92bba-122">Represents a meeting response in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="92bba-123">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="92bba-123">Text value</span></span>

<span data-ttu-id="92bba-124">Um valor de texto **true** indica que a reunião foi tratada por uma conta que tenha acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="92bba-124">A text value of **true** indicates that the meeting was handled by an account that has delegate access.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="92bba-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="92bba-125">Remarks</span></span>

<span data-ttu-id="92bba-126">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="92bba-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="92bba-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="92bba-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="92bba-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="92bba-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="92bba-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="92bba-129">Schema Name</span></span>  <br/> |<span data-ttu-id="92bba-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="92bba-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="92bba-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="92bba-131">Validation File</span></span>  <br/> |<span data-ttu-id="92bba-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="92bba-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="92bba-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="92bba-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="92bba-134">False</span><span class="sxs-lookup"><span data-stu-id="92bba-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="92bba-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="92bba-135">See also</span></span>



- [<span data-ttu-id="92bba-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="92bba-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

