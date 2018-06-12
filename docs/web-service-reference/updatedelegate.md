---
title: UpdateDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateDelegate
api_type:
- schema
ms.assetid: c6ae99c4-18b0-4136-90ab-12cf15e15f91
description: O elemento de UpdateDelegate define uma solicitação de atualização de representantes em uma caixa de correio. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 32322e48acfa5f1058786162565a185a3e565d6e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837878"
---
# <a name="updatedelegate"></a><span data-ttu-id="b58f6-104">UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="b58f6-104">UpdateDelegate</span></span>

<span data-ttu-id="b58f6-105">O elemento de **UpdateDelegate** define uma solicitação de atualização de representantes em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b58f6-105">The **UpdateDelegate** element defines a request to update delegates in a mailbox.</span></span> <span data-ttu-id="b58f6-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="b58f6-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<UpdateDelegate>
      <DelegateUsers/>
   <DeliverMeetingRequests/>
      <Mailbox/>
</UpdateDelegate>
```

 <span data-ttu-id="b58f6-107">**UpdateDelegateType**</span><span class="sxs-lookup"><span data-stu-id="b58f6-107">**UpdateDelegateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b58f6-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b58f6-108">Attributes and elements</span></span>

<span data-ttu-id="b58f6-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b58f6-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b58f6-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="b58f6-110">Attributes</span></span>

<span data-ttu-id="b58f6-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b58f6-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b58f6-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b58f6-112">Child elements</span></span>

|<span data-ttu-id="b58f6-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b58f6-113">**Element**</span></span>|<span data-ttu-id="b58f6-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b58f6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b58f6-115">DelegateUsers</span><span class="sxs-lookup"><span data-stu-id="b58f6-115">DelegateUsers</span></span>](delegateusers.md) <br/> |<span data-ttu-id="b58f6-116">Contém uma matriz de elementos [DelegateUser](delegateuser.md) que identificam os representantes e as atualizações para aplicar aos delegados.</span><span class="sxs-lookup"><span data-stu-id="b58f6-116">Contains an array of [DelegateUser](delegateuser.md) elements that identify the delegates and the updates to apply to the delegates.</span></span> <span data-ttu-id="b58f6-117">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="b58f6-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="b58f6-118">DeliverMeetingRequests</span><span class="sxs-lookup"><span data-stu-id="b58f6-118">DeliverMeetingRequests</span></span>](delivermeetingrequests.md) <br/> |<span data-ttu-id="b58f6-119">Define como as solicitações de reunião são manipuladas entre o delegado e a entidade.</span><span class="sxs-lookup"><span data-stu-id="b58f6-119">Defines how meeting requests are handled between the delegate and the principal.</span></span> <span data-ttu-id="b58f6-120">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="b58f6-120">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="b58f6-121">Caixa de correio</span><span class="sxs-lookup"><span data-stu-id="b58f6-121">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="b58f6-122">Identifica um objeto de serviço de diretório do Active Directory habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="b58f6-122">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b58f6-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b58f6-123">Parent elements</span></span>

<span data-ttu-id="b58f6-124">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b58f6-124">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b58f6-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="b58f6-125">Remarks</span></span>

<span data-ttu-id="b58f6-126">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="b58f6-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b58f6-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b58f6-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b58f6-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="b58f6-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b58f6-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b58f6-129">Schema Name</span></span>  <br/> |<span data-ttu-id="b58f6-130">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="b58f6-130">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b58f6-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b58f6-131">Validation File</span></span>  <br/> |<span data-ttu-id="b58f6-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b58f6-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b58f6-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b58f6-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="b58f6-134">False</span><span class="sxs-lookup"><span data-stu-id="b58f6-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b58f6-135">Ver também</span><span class="sxs-lookup"><span data-stu-id="b58f6-135">See also</span></span>



[<span data-ttu-id="b58f6-136">Operação UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="b58f6-136">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="b58f6-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b58f6-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

