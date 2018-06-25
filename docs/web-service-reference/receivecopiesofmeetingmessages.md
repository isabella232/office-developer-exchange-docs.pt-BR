---
title: ReceiveCopiesOfMeetingMessages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReceiveCopiesOfMeetingMessages
api_type:
- schema
ms.assetid: 65217ca8-6aea-47eb-a989-e6cce25f5f09
description: O elemento ReceiveCopiesOfMeetingMessages indica se um delegado receba cópias de mensagens relacionadas a reuniões que são abordadas à entidade de segurança. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: e39a5d3255268b418fa956959da5ae0ea062d831
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824967"
---
# <a name="receivecopiesofmeetingmessages"></a><span data-ttu-id="ef735-104">ReceiveCopiesOfMeetingMessages</span><span class="sxs-lookup"><span data-stu-id="ef735-104">ReceiveCopiesOfMeetingMessages</span></span>

<span data-ttu-id="ef735-105">O elemento **ReceiveCopiesOfMeetingMessages** indica se um delegado receba cópias de mensagens relacionadas a reuniões que são abordadas à entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="ef735-105">The **ReceiveCopiesOfMeetingMessages** element indicates whether a delegate receives copies of meeting-related messages that are addressed to the principal.</span></span> <span data-ttu-id="ef735-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ef735-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ReceiveCopiesOfMeetingMessages>true or false</ReceiveCopiesOfMeetingMessages>
```

 <span data-ttu-id="ef735-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="ef735-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ef735-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ef735-108">Attributes and elements</span></span>

<span data-ttu-id="ef735-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ef735-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ef735-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="ef735-110">Attributes</span></span>

<span data-ttu-id="ef735-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ef735-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ef735-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ef735-112">Child elements</span></span>

<span data-ttu-id="ef735-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ef735-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ef735-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ef735-114">Parent elements</span></span>

|<span data-ttu-id="ef735-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ef735-115">**Element**</span></span>|<span data-ttu-id="ef735-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ef735-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ef735-117">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="ef735-117">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="ef735-118">Identifica um único representante para adicionar ou atualizar em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="ef735-118">Identifies a single delegate to add or update in a mailbox.</span></span> <span data-ttu-id="ef735-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="ef735-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ef735-120">Text value</span><span class="sxs-lookup"><span data-stu-id="ef735-120">Text value</span></span>

<span data-ttu-id="ef735-121">Um valor de texto de **true** indica que um delegado receba uma cópia das mensagens de reunião.</span><span class="sxs-lookup"><span data-stu-id="ef735-121">A text value of **true** indicates that a delegate receives a copy of meeting messages.</span></span> <span data-ttu-id="ef735-122">Um valor de texto de **false** indica que um representante não recebe uma cópia das mensagens de reunião.</span><span class="sxs-lookup"><span data-stu-id="ef735-122">A text value of **false** indicates that a delegate does not receive a copy of meeting messages.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ef735-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="ef735-123">Remarks</span></span>

<span data-ttu-id="ef735-124">Quando **ReceiveCopiesOfMeetingMessages** é definida como **false**, o representante ainda pode enviar mensagens em nome de entidade de segurança, mas não receberão todas as mensagens relacionadas a reuniões.</span><span class="sxs-lookup"><span data-stu-id="ef735-124">When **ReceiveCopiesOfMeetingMessages** is set to **false**, the delegate can still send message on behalf of the principal, but will not receive any meeting-related messages.</span></span>
  
<span data-ttu-id="ef735-125">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="ef735-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ef735-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ef735-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ef735-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="ef735-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ef735-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ef735-128">Schema Name</span></span>  <br/> |<span data-ttu-id="ef735-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ef735-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="ef735-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ef735-130">Validation File</span></span>  <br/> |<span data-ttu-id="ef735-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ef735-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ef735-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ef735-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="ef735-133">False</span><span class="sxs-lookup"><span data-stu-id="ef735-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ef735-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="ef735-134">See also</span></span>



[<span data-ttu-id="ef735-135">Operação AddDelegate</span><span class="sxs-lookup"><span data-stu-id="ef735-135">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="ef735-136">Operação UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="ef735-136">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="ef735-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ef735-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="ef735-138">Adicionando representantes</span><span class="sxs-lookup"><span data-stu-id="ef735-138">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

