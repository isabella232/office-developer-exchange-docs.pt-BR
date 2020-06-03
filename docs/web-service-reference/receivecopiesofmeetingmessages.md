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
description: O elemento ReceiveCopiesOfMeetingMessages indica se um representante recebe cópias de mensagens relacionadas à reunião endereçadas à entidade de segurança. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: af6e220304f88c4db00ab675077dcd9bf581ea9e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468261"
---
# <a name="receivecopiesofmeetingmessages"></a><span data-ttu-id="60eca-104">ReceiveCopiesOfMeetingMessages</span><span class="sxs-lookup"><span data-stu-id="60eca-104">ReceiveCopiesOfMeetingMessages</span></span>

<span data-ttu-id="60eca-105">O elemento **ReceiveCopiesOfMeetingMessages** indica se um representante recebe cópias de mensagens relacionadas à reunião endereçadas à entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="60eca-105">The **ReceiveCopiesOfMeetingMessages** element indicates whether a delegate receives copies of meeting-related messages that are addressed to the principal.</span></span> <span data-ttu-id="60eca-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="60eca-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ReceiveCopiesOfMeetingMessages>true or false</ReceiveCopiesOfMeetingMessages>
```

 <span data-ttu-id="60eca-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="60eca-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="60eca-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="60eca-108">Attributes and elements</span></span>

<span data-ttu-id="60eca-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="60eca-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="60eca-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="60eca-110">Attributes</span></span>

<span data-ttu-id="60eca-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="60eca-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="60eca-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="60eca-112">Child elements</span></span>

<span data-ttu-id="60eca-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="60eca-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="60eca-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="60eca-114">Parent elements</span></span>

|<span data-ttu-id="60eca-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="60eca-115">**Element**</span></span>|<span data-ttu-id="60eca-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="60eca-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="60eca-117">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="60eca-117">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="60eca-118">Identifica um único representante para adicionar ou atualizar em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="60eca-118">Identifies a single delegate to add or update in a mailbox.</span></span> <span data-ttu-id="60eca-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="60eca-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="60eca-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="60eca-120">Text value</span></span>

<span data-ttu-id="60eca-121">Um valor **true** indica que um representante recebe uma cópia das mensagens de reunião.</span><span class="sxs-lookup"><span data-stu-id="60eca-121">A text value of **true** indicates that a delegate receives a copy of meeting messages.</span></span> <span data-ttu-id="60eca-122">Um valor de texto **false** indica que um representante não recebe uma cópia das mensagens de reunião.</span><span class="sxs-lookup"><span data-stu-id="60eca-122">A text value of **false** indicates that a delegate does not receive a copy of meeting messages.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="60eca-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="60eca-123">Remarks</span></span>

<span data-ttu-id="60eca-124">Quando **ReceiveCopiesOfMeetingMessages** estiver definido como **false**, o representante ainda poderá enviar mensagens em nome da entidade de segurança, mas não receberá nenhuma mensagem relacionada à reunião.</span><span class="sxs-lookup"><span data-stu-id="60eca-124">When **ReceiveCopiesOfMeetingMessages** is set to **false**, the delegate can still send message on behalf of the principal, but will not receive any meeting-related messages.</span></span>
  
<span data-ttu-id="60eca-125">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="60eca-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="60eca-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="60eca-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="60eca-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="60eca-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="60eca-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="60eca-128">Schema Name</span></span>  <br/> |<span data-ttu-id="60eca-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="60eca-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="60eca-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="60eca-130">Validation File</span></span>  <br/> |<span data-ttu-id="60eca-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="60eca-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="60eca-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="60eca-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="60eca-133">False</span><span class="sxs-lookup"><span data-stu-id="60eca-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="60eca-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="60eca-134">See also</span></span>



[<span data-ttu-id="60eca-135">Operação AddDelegate</span><span class="sxs-lookup"><span data-stu-id="60eca-135">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="60eca-136">Operação UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="60eca-136">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="60eca-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="60eca-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="60eca-138">Adicionar representantes</span><span class="sxs-lookup"><span data-stu-id="60eca-138">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

