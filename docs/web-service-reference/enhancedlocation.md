---
title: EnhancedLocation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4fdfb74f-f33c-46ae-a7c7-451a5b0c6a59
description: O elemento EnhancedLocation especifica informações de local como nome, endereço e observações opcionais sobre um local.
ms.openlocfilehash: 06ec800b763ef61af51da03ca8a340f6ac4d2a8e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462954"
---
# <a name="enhancedlocation"></a><span data-ttu-id="35c0b-103">EnhancedLocation</span><span class="sxs-lookup"><span data-stu-id="35c0b-103">EnhancedLocation</span></span>

<span data-ttu-id="35c0b-104">O elemento **EnhancedLocation** especifica informações de local como nome, endereço e observações opcionais sobre um local.</span><span class="sxs-lookup"><span data-stu-id="35c0b-104">The **EnhancedLocation** element specifies location information such as the name, address, and optional notes about a location.</span></span> 
  
```XML
<EnhancedLocation>
    <DisplayName/>
    <Annotation/>
    <PostalAddress/>
</EnhancedLocation>
```

 <span data-ttu-id="35c0b-105">**EnhancedLocationType**</span><span class="sxs-lookup"><span data-stu-id="35c0b-105">**EnhancedLocationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="35c0b-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="35c0b-106">Attributes and elements</span></span>

<span data-ttu-id="35c0b-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="35c0b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="35c0b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="35c0b-108">Attributes</span></span>

<span data-ttu-id="35c0b-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="35c0b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="35c0b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="35c0b-110">Child elements</span></span>

|<span data-ttu-id="35c0b-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="35c0b-111">**Element**</span></span>|<span data-ttu-id="35c0b-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="35c0b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="35c0b-113">DisplayName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="35c0b-113">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="35c0b-114">Define o nome de exibição de uma pasta, contato, lista de distribuição, usuário delegado, local ou regra.</span><span class="sxs-lookup"><span data-stu-id="35c0b-114">Defines the display name of a folder, contact, distribution list, delegate user, location, or rule.</span></span>  <br/> |
|[<span data-ttu-id="35c0b-115">Comentário</span><span class="sxs-lookup"><span data-stu-id="35c0b-115">Annotation</span></span>](annotation.md) <br/> |<span data-ttu-id="35c0b-116">Contém observações opcionais adicionadas por um usuário.</span><span class="sxs-lookup"><span data-stu-id="35c0b-116">Contains optional notes added by a user.</span></span>  <br/> |
|[<span data-ttu-id="35c0b-117">Address (PersonaPostalAddressType)</span><span class="sxs-lookup"><span data-stu-id="35c0b-117">PostalAddress (PersonaPostalAddressType)</span></span>](postaladdress-personapostaladdresstype.md) <br/> |<span data-ttu-id="35c0b-118">Especifica o endereço postal de um persona.</span><span class="sxs-lookup"><span data-stu-id="35c0b-118">Specifies the postal address for a persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="35c0b-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="35c0b-119">Parent elements</span></span>

|<span data-ttu-id="35c0b-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="35c0b-120">**Element**</span></span>|<span data-ttu-id="35c0b-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="35c0b-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="35c0b-122">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="35c0b-122">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="35c0b-123">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="35c0b-123">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="35c0b-124">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="35c0b-124">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="35c0b-125">Representa um cancelamento de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="35c0b-125">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="35c0b-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="35c0b-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="35c0b-127">Representa uma resposta de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="35c0b-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="35c0b-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="35c0b-128">Remarks</span></span>

<span data-ttu-id="35c0b-129">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="35c0b-129">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="35c0b-130">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="35c0b-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="35c0b-131">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="35c0b-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="35c0b-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="35c0b-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="35c0b-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="35c0b-133">Schema Name</span></span>  <br/> |<span data-ttu-id="35c0b-134">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="35c0b-134">Type schema</span></span>  <br/> |
|<span data-ttu-id="35c0b-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="35c0b-135">Validation File</span></span>  <br/> |<span data-ttu-id="35c0b-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="35c0b-136">types.xsd</span></span>  <br/> |
|<span data-ttu-id="35c0b-137">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="35c0b-137">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="35c0b-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="35c0b-138">See also</span></span>



- [<span data-ttu-id="35c0b-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="35c0b-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

