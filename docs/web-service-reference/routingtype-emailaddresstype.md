---
title: RoutingType (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RoutingType
api_type:
- schema
ms.assetid: 683216be-9972-4f48-a148-c34bfe7f53e5
description: O elemento de RoutingType define o tipo de endereço da caixa de correio.
ms.openlocfilehash: a02c3b5711a657311428d67cccabd9c8c231db67
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825256"
---
# <a name="routingtype-emailaddresstype"></a><span data-ttu-id="83431-103">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="83431-103">RoutingType (EmailAddressType)</span></span>

<span data-ttu-id="83431-104">O elemento de **RoutingType** define o tipo de endereço da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="83431-104">The **RoutingType** element defines the address type for the mailbox.</span></span> 
  
```XML
<RoutingType/>
```

 <span data-ttu-id="83431-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="83431-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="83431-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="83431-106">Attributes and elements</span></span>

<span data-ttu-id="83431-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="83431-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="83431-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="83431-108">Attributes</span></span>

<span data-ttu-id="83431-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="83431-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="83431-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="83431-110">Child elements</span></span>

<span data-ttu-id="83431-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="83431-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="83431-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="83431-112">Parent elements</span></span>

|<span data-ttu-id="83431-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="83431-113">**Element**</span></span>|<span data-ttu-id="83431-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="83431-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="83431-115">ActingAs</span><span class="sxs-lookup"><span data-stu-id="83431-115">ActingAs</span></span>](actingas.md) <br/> |<span data-ttu-id="83431-116">Identifica que o chamador está enviando como.</span><span class="sxs-lookup"><span data-stu-id="83431-116">Identifies who the caller is sending as.</span></span>  <br/> |
|[<span data-ttu-id="83431-117">Caixa de correio</span><span class="sxs-lookup"><span data-stu-id="83431-117">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="83431-118">Identifica um endereço de email totalmente resolvido.</span><span class="sxs-lookup"><span data-stu-id="83431-118">Identifies a fully resolved e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="83431-119">RoomList</span><span class="sxs-lookup"><span data-stu-id="83431-119">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="83431-120">Identifica uma lista de salas de reunião.</span><span class="sxs-lookup"><span data-stu-id="83431-120">Identifies a list of meeting rooms.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="83431-121">Text value</span><span class="sxs-lookup"><span data-stu-id="83431-121">Text value</span></span>

<span data-ttu-id="83431-122">O valor de texto representa um tipo de roteamento.</span><span class="sxs-lookup"><span data-stu-id="83431-122">The text value represents a routing type.</span></span> <span data-ttu-id="83431-123">SMTP é o valor de texto típica para esse elemento.</span><span class="sxs-lookup"><span data-stu-id="83431-123">SMTP is the typical text value for this element.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="83431-124">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="83431-124">Remarks</span></span>

<span data-ttu-id="83431-125">Esse elemento é opcional no elemento de [caixa de correio](mailbox.md) .</span><span class="sxs-lookup"><span data-stu-id="83431-125">This element is optional in the [Mailbox](mailbox.md) element.</span></span> <span data-ttu-id="83431-126">Outro elemento [RoutingType (EmailAddress)](routingtype-emailaddress.md) é usado para operações de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="83431-126">Another [RoutingType (EmailAddress)](routingtype-emailaddress.md) element is used for Availability operations.</span></span> 
  
<span data-ttu-id="83431-127">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="83431-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="83431-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="83431-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="83431-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="83431-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="83431-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="83431-130">Schema Name</span></span>  <br/> |<span data-ttu-id="83431-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="83431-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="83431-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="83431-132">Validation File</span></span>  <br/> |<span data-ttu-id="83431-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="83431-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="83431-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="83431-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="83431-135">False</span><span class="sxs-lookup"><span data-stu-id="83431-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="83431-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="83431-136">See also</span></span>



- [<span data-ttu-id="83431-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="83431-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

