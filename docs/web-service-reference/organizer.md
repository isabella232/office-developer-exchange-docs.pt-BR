---
title: Organizador
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Organizer
api_type:
- schema
ms.assetid: 63892b57-3805-4d60-b9f7-20552a69c241
description: O elemento organizador representa o organizador de uma reunião.
ms.openlocfilehash: b723578a1b52cd5f6e9bd869a15430453adfa291
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824662"
---
# <a name="organizer"></a><span data-ttu-id="26648-103">Organizador</span><span class="sxs-lookup"><span data-stu-id="26648-103">Organizer</span></span>

<span data-ttu-id="26648-104">O elemento **Organizador** representa o organizador de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="26648-104">The **Organizer** element represents the organizer of a meeting.</span></span> 
  
```xml
<Organizer>
   <Mailbox/>
</Organizer>
```

<span data-ttu-id="26648-105">**SingleRecipientType**</span><span class="sxs-lookup"><span data-stu-id="26648-105">**SingleRecipientType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="26648-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="26648-106">Attributes and elements</span></span>

<span data-ttu-id="26648-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="26648-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="26648-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="26648-108">Attributes</span></span>

<span data-ttu-id="26648-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="26648-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="26648-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="26648-110">Child elements</span></span>

|<span data-ttu-id="26648-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="26648-111">**Element**</span></span>|<span data-ttu-id="26648-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="26648-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="26648-113">Caixa de correio</span><span class="sxs-lookup"><span data-stu-id="26648-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="26648-114">Identifica um objeto de serviço de diretório do Active Directory habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="26648-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="26648-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="26648-115">Parent elements</span></span>

|<span data-ttu-id="26648-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="26648-116">**Element**</span></span>|<span data-ttu-id="26648-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="26648-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="26648-118">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="26648-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="26648-119">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="26648-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="26648-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="26648-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="26648-121">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="26648-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="26648-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="26648-122">Remarks</span></span>

<span data-ttu-id="26648-123">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="26648-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="26648-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="26648-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="26648-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="26648-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="26648-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="26648-126">Schema name</span></span>  <br/> |<span data-ttu-id="26648-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="26648-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="26648-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="26648-128">Validation file</span></span>  <br/> |<span data-ttu-id="26648-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="26648-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="26648-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="26648-130">Can be empty</span></span>  <br/> |<span data-ttu-id="26648-131">False</span><span class="sxs-lookup"><span data-stu-id="26648-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="26648-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="26648-132">See also</span></span>

- [<span data-ttu-id="26648-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="26648-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

