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
ms.openlocfilehash: c1188c9b3a894e86a08b8869045c3647e394f506
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462413"
---
# <a name="organizer"></a><span data-ttu-id="a165b-103">Organizador</span><span class="sxs-lookup"><span data-stu-id="a165b-103">Organizer</span></span>

<span data-ttu-id="a165b-104">O elemento **organizador** representa o organizador de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="a165b-104">The **Organizer** element represents the organizer of a meeting.</span></span> 
  
```xml
<Organizer>
   <Mailbox/>
</Organizer>
```

<span data-ttu-id="a165b-105">**SingleRecipientType**</span><span class="sxs-lookup"><span data-stu-id="a165b-105">**SingleRecipientType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a165b-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a165b-106">Attributes and elements</span></span>

<span data-ttu-id="a165b-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a165b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a165b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a165b-108">Attributes</span></span>

<span data-ttu-id="a165b-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a165b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a165b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a165b-110">Child elements</span></span>

|<span data-ttu-id="a165b-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a165b-111">**Element**</span></span>|<span data-ttu-id="a165b-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a165b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a165b-113">Caixa de Correio</span><span class="sxs-lookup"><span data-stu-id="a165b-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="a165b-114">Identifica um objeto de serviço de diretório do Active Directory habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="a165b-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a165b-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a165b-115">Parent elements</span></span>

|<span data-ttu-id="a165b-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a165b-116">**Element**</span></span>|<span data-ttu-id="a165b-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a165b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a165b-118">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="a165b-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="a165b-119">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a165b-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="a165b-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="a165b-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="a165b-121">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a165b-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a165b-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="a165b-122">Remarks</span></span>

<span data-ttu-id="a165b-123">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="a165b-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a165b-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="a165b-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a165b-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="a165b-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a165b-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a165b-126">Schema name</span></span>  <br/> |<span data-ttu-id="a165b-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a165b-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="a165b-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a165b-128">Validation file</span></span>  <br/> |<span data-ttu-id="a165b-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a165b-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a165b-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="a165b-130">Can be empty</span></span>  <br/> |<span data-ttu-id="a165b-131">False</span><span class="sxs-lookup"><span data-stu-id="a165b-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a165b-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="a165b-132">See also</span></span>

- [<span data-ttu-id="a165b-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a165b-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

