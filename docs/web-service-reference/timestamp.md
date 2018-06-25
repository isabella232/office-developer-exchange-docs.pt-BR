---
title: Carimbo de hora
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeStamp
api_type:
- schema
ms.assetid: 5eae859a-5a74-4bf6-b196-d1b2fd38501a
description: O elemento de carimbo de hora representa o carimbo de hora de um evento de caixa de correio.
ms.openlocfilehash: d020d9a4cf3a128d26e0ff2b83be9f3deb024339
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837791"
---
# <a name="timestamp"></a><span data-ttu-id="091d0-103">Carimbo de hora</span><span class="sxs-lookup"><span data-stu-id="091d0-103">TimeStamp</span></span>

<span data-ttu-id="091d0-104">O elemento de **carimbo de hora** representa o carimbo de hora de um evento de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="091d0-104">The **Timestamp** element represents the timestamp of a mailbox event.</span></span> 
  
```xml
<TimeStamp/>
```

 <span data-ttu-id="091d0-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="091d0-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="091d0-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="091d0-106">Attributes and elements</span></span>

<span data-ttu-id="091d0-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="091d0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="091d0-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="091d0-108">Attributes</span></span>

<span data-ttu-id="091d0-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="091d0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="091d0-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="091d0-110">Child elements</span></span>

<span data-ttu-id="091d0-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="091d0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="091d0-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="091d0-112">Parent elements</span></span>

|<span data-ttu-id="091d0-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="091d0-113">**Element**</span></span>|<span data-ttu-id="091d0-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="091d0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="091d0-115">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="091d0-115">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="091d0-116">Representa um evento onde uma pasta ou um item é copiada.</span><span class="sxs-lookup"><span data-stu-id="091d0-116">Represents an event where an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="091d0-117">CreatedEvent</span><span class="sxs-lookup"><span data-stu-id="091d0-117">CreatedEvent</span></span>](createdevent.md) <br/> |<span data-ttu-id="091d0-118">Representa um evento onde uma pasta ou um item é criada.</span><span class="sxs-lookup"><span data-stu-id="091d0-118">Represents an event where an item or folder is created.</span></span>  <br/> |
|[<span data-ttu-id="091d0-119">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="091d0-119">DeletedEvent</span></span>](deletedevent.md) <br/> |<span data-ttu-id="091d0-120">Representa um evento onde uma pasta ou um item é excluída.</span><span class="sxs-lookup"><span data-stu-id="091d0-120">Represents an event where an item or folder is deleted.</span></span>  <br/> |
|[<span data-ttu-id="091d0-121">ModifiedEvent</span><span class="sxs-lookup"><span data-stu-id="091d0-121">ModifiedEvent</span></span>](modifiedevent.md) <br/> |<span data-ttu-id="091d0-122">Representa um evento onde um item ou pasta é modificada.</span><span class="sxs-lookup"><span data-stu-id="091d0-122">Represents an event where an item or folder is modified.</span></span>  <br/> |
|[<span data-ttu-id="091d0-123">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="091d0-123">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="091d0-124">Representa um evento onde uma pasta ou um item é movida da pasta pai de um para outra pasta pai.</span><span class="sxs-lookup"><span data-stu-id="091d0-124">Represents an event where an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
|[<span data-ttu-id="091d0-125">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="091d0-125">NewMailEvent</span></span>](newmailevent.md) <br/> |<span data-ttu-id="091d0-126">Representa um evento disparado por um novo item de email em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="091d0-126">Represents an event triggered by a new mail item in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="091d0-127">Text value</span><span class="sxs-lookup"><span data-stu-id="091d0-127">Text value</span></span>

<span data-ttu-id="091d0-128">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="091d0-128">This property is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="091d0-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="091d0-129">Remarks</span></span>

<span data-ttu-id="091d0-130">Este elemento está disponível principalmente para uso na determinação do cliente da frequência de evento.</span><span class="sxs-lookup"><span data-stu-id="091d0-130">This element is primarily available for use in client determination of event frequency.</span></span> <span data-ttu-id="091d0-131">Isso não está presente no [StatusEvent](statusevent.md).</span><span class="sxs-lookup"><span data-stu-id="091d0-131">This is not present in [StatusEvent](statusevent.md).</span></span>
  
<span data-ttu-id="091d0-132">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="091d0-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="091d0-133">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="091d0-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="091d0-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="091d0-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="091d0-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="091d0-135">Schema name</span></span>  <br/> |<span data-ttu-id="091d0-136">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="091d0-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="091d0-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="091d0-137">Validation file</span></span>  <br/> |<span data-ttu-id="091d0-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="091d0-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="091d0-139">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="091d0-139">Can be empty</span></span>  <br/> |<span data-ttu-id="091d0-140">False</span><span class="sxs-lookup"><span data-stu-id="091d0-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="091d0-141">Ver também</span><span class="sxs-lookup"><span data-stu-id="091d0-141">See also</span></span>



[<span data-ttu-id="091d0-142">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="091d0-142">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="091d0-143">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="091d0-143">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="091d0-144">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="091d0-144">Unsubscribe operation</span></span>](unsubscribe-operation.md)

