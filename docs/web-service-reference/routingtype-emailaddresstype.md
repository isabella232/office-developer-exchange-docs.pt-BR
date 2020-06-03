---
title: RoutingType (EmailAddresstype)
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
description: O elemento RoutingType define o tipo de endereço da caixa de correio.
ms.openlocfilehash: d4229f2857a5c99cc9bb7ff9b9b103de099a0055
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465083"
---
# <a name="routingtype-emailaddresstype"></a><span data-ttu-id="32831-103">RoutingType (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="32831-103">RoutingType (EmailAddressType)</span></span>

<span data-ttu-id="32831-104">O elemento **RoutingType** define o tipo de endereço da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="32831-104">The **RoutingType** element defines the address type for the mailbox.</span></span> 
  
```XML
<RoutingType/>
```

 <span data-ttu-id="32831-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="32831-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="32831-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="32831-106">Attributes and elements</span></span>

<span data-ttu-id="32831-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="32831-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="32831-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="32831-108">Attributes</span></span>

<span data-ttu-id="32831-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="32831-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="32831-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="32831-110">Child elements</span></span>

<span data-ttu-id="32831-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="32831-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="32831-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="32831-112">Parent elements</span></span>

|<span data-ttu-id="32831-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="32831-113">**Element**</span></span>|<span data-ttu-id="32831-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="32831-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="32831-115">Agindo</span><span class="sxs-lookup"><span data-stu-id="32831-115">ActingAs</span></span>](actingas.md) <br/> |<span data-ttu-id="32831-116">Identifica quem o chamador está enviando como.</span><span class="sxs-lookup"><span data-stu-id="32831-116">Identifies who the caller is sending as.</span></span>  <br/> |
|[<span data-ttu-id="32831-117">Caixa de Correio</span><span class="sxs-lookup"><span data-stu-id="32831-117">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="32831-118">Identifica um endereço de email totalmente resolvido.</span><span class="sxs-lookup"><span data-stu-id="32831-118">Identifies a fully resolved e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="32831-119">RoomList</span><span class="sxs-lookup"><span data-stu-id="32831-119">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="32831-120">Identifica uma lista de salas de reunião.</span><span class="sxs-lookup"><span data-stu-id="32831-120">Identifies a list of meeting rooms.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="32831-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="32831-121">Text value</span></span>

<span data-ttu-id="32831-122">O valor de texto representa um tipo de roteamento.</span><span class="sxs-lookup"><span data-stu-id="32831-122">The text value represents a routing type.</span></span> <span data-ttu-id="32831-123">SMTP é o valor de texto típico para este elemento.</span><span class="sxs-lookup"><span data-stu-id="32831-123">SMTP is the typical text value for this element.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="32831-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="32831-124">Remarks</span></span>

<span data-ttu-id="32831-125">Este elemento é opcional no elemento [Mailbox](mailbox.md) .</span><span class="sxs-lookup"><span data-stu-id="32831-125">This element is optional in the [Mailbox](mailbox.md) element.</span></span> <span data-ttu-id="32831-126">Outro elemento [RoutingType (EmailAddress)](routingtype-emailaddress.md) é usado para operações de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="32831-126">Another [RoutingType (EmailAddress)](routingtype-emailaddress.md) element is used for Availability operations.</span></span> 
  
<span data-ttu-id="32831-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="32831-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="32831-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="32831-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="32831-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="32831-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="32831-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="32831-130">Schema Name</span></span>  <br/> |<span data-ttu-id="32831-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="32831-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="32831-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="32831-132">Validation File</span></span>  <br/> |<span data-ttu-id="32831-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="32831-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="32831-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="32831-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="32831-135">False</span><span class="sxs-lookup"><span data-stu-id="32831-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="32831-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="32831-136">See also</span></span>



- [<span data-ttu-id="32831-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="32831-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

