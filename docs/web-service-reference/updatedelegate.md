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
description: O elemento UpdateDelegate define uma solicitação para atualizar representantes em uma caixa de correio. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 17d69eb8c539217d39e1dd0c2616261d02ad304d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468870"
---
# <a name="updatedelegate"></a><span data-ttu-id="d2c1c-104">UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="d2c1c-104">UpdateDelegate</span></span>

<span data-ttu-id="d2c1c-105">O elemento **UpdateDelegate** define uma solicitação para atualizar representantes em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d2c1c-105">The **UpdateDelegate** element defines a request to update delegates in a mailbox.</span></span> <span data-ttu-id="d2c1c-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="d2c1c-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<UpdateDelegate>
      <DelegateUsers/>
   <DeliverMeetingRequests/>
      <Mailbox/>
</UpdateDelegate>
```

 <span data-ttu-id="d2c1c-107">**UpdateDelegateType**</span><span class="sxs-lookup"><span data-stu-id="d2c1c-107">**UpdateDelegateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d2c1c-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d2c1c-108">Attributes and elements</span></span>

<span data-ttu-id="d2c1c-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d2c1c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d2c1c-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="d2c1c-110">Attributes</span></span>

<span data-ttu-id="d2c1c-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d2c1c-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d2c1c-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d2c1c-112">Child elements</span></span>

|<span data-ttu-id="d2c1c-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d2c1c-113">**Element**</span></span>|<span data-ttu-id="d2c1c-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d2c1c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2c1c-115">DelegateUsers</span><span class="sxs-lookup"><span data-stu-id="d2c1c-115">DelegateUsers</span></span>](delegateusers.md) <br/> |<span data-ttu-id="d2c1c-116">Contém uma matriz de elementos [DelegateUser](delegateuser.md) que identificam os representantes e as atualizações a serem aplicadas aos representantes.</span><span class="sxs-lookup"><span data-stu-id="d2c1c-116">Contains an array of [DelegateUser](delegateuser.md) elements that identify the delegates and the updates to apply to the delegates.</span></span> <span data-ttu-id="d2c1c-117">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="d2c1c-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="d2c1c-118">DeliverMeetingRequests</span><span class="sxs-lookup"><span data-stu-id="d2c1c-118">DeliverMeetingRequests</span></span>](delivermeetingrequests.md) <br/> |<span data-ttu-id="d2c1c-119">Define como as solicitações de reunião são tratadas entre o representante e a entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="d2c1c-119">Defines how meeting requests are handled between the delegate and the principal.</span></span> <span data-ttu-id="d2c1c-120">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="d2c1c-120">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="d2c1c-121">Caixa de Correio</span><span class="sxs-lookup"><span data-stu-id="d2c1c-121">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="d2c1c-122">Identifica um objeto de serviço de diretório do Active Directory habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="d2c1c-122">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d2c1c-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d2c1c-123">Parent elements</span></span>

<span data-ttu-id="d2c1c-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d2c1c-124">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d2c1c-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="d2c1c-125">Remarks</span></span>

<span data-ttu-id="d2c1c-126">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="d2c1c-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d2c1c-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d2c1c-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d2c1c-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="d2c1c-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d2c1c-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d2c1c-129">Schema Name</span></span>  <br/> |<span data-ttu-id="d2c1c-130">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="d2c1c-130">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d2c1c-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d2c1c-131">Validation File</span></span>  <br/> |<span data-ttu-id="d2c1c-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d2c1c-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d2c1c-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d2c1c-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="d2c1c-134">False</span><span class="sxs-lookup"><span data-stu-id="d2c1c-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d2c1c-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="d2c1c-135">See also</span></span>



[<span data-ttu-id="d2c1c-136">Operação UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="d2c1c-136">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="d2c1c-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d2c1c-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

