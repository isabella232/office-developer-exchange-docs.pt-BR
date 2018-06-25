---
title: EnhancedLocation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4fdfb74f-f33c-46ae-a7c7-451a5b0c6a59
description: O elemento EnhancedLocation Especifica as informações de local como o nome, endereço e observações opcionais sobre um local.
ms.openlocfilehash: 90397cfc622fed40c561d30c13d6617eb979a68a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752071"
---
# <a name="enhancedlocation"></a><span data-ttu-id="0d5c2-103">EnhancedLocation</span><span class="sxs-lookup"><span data-stu-id="0d5c2-103">EnhancedLocation</span></span>

<span data-ttu-id="0d5c2-104">O elemento **EnhancedLocation** Especifica as informações de local como o nome, endereço e observações opcionais sobre um local.</span><span class="sxs-lookup"><span data-stu-id="0d5c2-104">The **EnhancedLocation** element specifies location information such as the name, address, and optional notes about a location.</span></span> 
  
```XML
<EnhancedLocation>
    <DisplayName/>
    <Annotation/>
    <PostalAddress/>
</EnhancedLocation>
```

 <span data-ttu-id="0d5c2-105">**EnhancedLocationType**</span><span class="sxs-lookup"><span data-stu-id="0d5c2-105">**EnhancedLocationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0d5c2-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="0d5c2-106">Attributes and elements</span></span>

<span data-ttu-id="0d5c2-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0d5c2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0d5c2-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0d5c2-108">Attributes</span></span>

<span data-ttu-id="0d5c2-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0d5c2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0d5c2-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0d5c2-110">Child elements</span></span>

|<span data-ttu-id="0d5c2-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0d5c2-111">**Element**</span></span>|<span data-ttu-id="0d5c2-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0d5c2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0d5c2-113">DisplayName (string)</span><span class="sxs-lookup"><span data-stu-id="0d5c2-113">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="0d5c2-114">Define o nome de exibição de uma pasta, contatos, lista de distribuição, usuário delegado, local ou regra.</span><span class="sxs-lookup"><span data-stu-id="0d5c2-114">Defines the display name of a folder, contact, distribution list, delegate user, location, or rule.</span></span>  <br/> |
|[<span data-ttu-id="0d5c2-115">Anotação</span><span class="sxs-lookup"><span data-stu-id="0d5c2-115">Annotation</span></span>](annotation.md) <br/> |<span data-ttu-id="0d5c2-116">Contém observações opcionais adicionadas por um usuário.</span><span class="sxs-lookup"><span data-stu-id="0d5c2-116">Contains optional notes added by a user.</span></span>  <br/> |
|[<span data-ttu-id="0d5c2-117">Address (PersonaPostalAddressType)</span><span class="sxs-lookup"><span data-stu-id="0d5c2-117">PostalAddress (PersonaPostalAddressType)</span></span>](postaladdress-personapostaladdresstype.md) <br/> |<span data-ttu-id="0d5c2-118">Especifica o endereço postal para uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="0d5c2-118">Specifies the postal address for a persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0d5c2-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0d5c2-119">Parent elements</span></span>

|<span data-ttu-id="0d5c2-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0d5c2-120">**Element**</span></span>|<span data-ttu-id="0d5c2-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0d5c2-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0d5c2-122">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="0d5c2-122">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="0d5c2-123">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0d5c2-123">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="0d5c2-124">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="0d5c2-124">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="0d5c2-125">Representa o cancelamento da reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0d5c2-125">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0d5c2-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="0d5c2-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="0d5c2-127">Representa uma resposta de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0d5c2-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0d5c2-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="0d5c2-128">Remarks</span></span>

<span data-ttu-id="0d5c2-129">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0d5c2-129">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0d5c2-130">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0d5c2-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0d5c2-131">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="0d5c2-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0d5c2-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="0d5c2-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0d5c2-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0d5c2-133">Schema Name</span></span>  <br/> |<span data-ttu-id="0d5c2-134">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="0d5c2-134">Type schema</span></span>  <br/> |
|<span data-ttu-id="0d5c2-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0d5c2-135">Validation File</span></span>  <br/> |<span data-ttu-id="0d5c2-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0d5c2-136">types.xsd</span></span>  <br/> |
|<span data-ttu-id="0d5c2-137">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="0d5c2-137">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="0d5c2-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="0d5c2-138">See also</span></span>



- [<span data-ttu-id="0d5c2-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0d5c2-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

