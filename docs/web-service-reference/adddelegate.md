---
title: AddDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AddDelegate
api_type:
- schema
ms.assetid: 646fb994-229e-4d90-8b95-6541191cb3ae
description: O elemento de AddDelegate define uma solicitação para adicionar representantes para uma caixa de correio. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: d1cb0ff3ea68904bf88e346f68afe7c349ae4394
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751052"
---
# <a name="adddelegate"></a><span data-ttu-id="ec249-104">AddDelegate</span><span class="sxs-lookup"><span data-stu-id="ec249-104">AddDelegate</span></span>

<span data-ttu-id="ec249-105">O elemento de **AddDelegate** define uma solicitação para adicionar representantes para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="ec249-105">The **AddDelegate** element defines a request to add delegates to a mailbox.</span></span> <span data-ttu-id="ec249-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ec249-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<AddDelegate>
   <DelegateUsers/>
   <DeliverMeetingRequests/>
   <Mailbox/>
</AddDelegate>
```

 <span data-ttu-id="ec249-107">**AddDelegateType**</span><span class="sxs-lookup"><span data-stu-id="ec249-107">**AddDelegateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ec249-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ec249-108">Attributes and elements</span></span>

<span data-ttu-id="ec249-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ec249-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ec249-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="ec249-110">Attributes</span></span>

<span data-ttu-id="ec249-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ec249-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ec249-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ec249-112">Child elements</span></span>

|<span data-ttu-id="ec249-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ec249-113">**Element**</span></span>|<span data-ttu-id="ec249-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ec249-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ec249-115">DelegateUsers</span><span class="sxs-lookup"><span data-stu-id="ec249-115">DelegateUsers</span></span>](delegateusers.md) <br/> |<span data-ttu-id="ec249-116">Contém as identidades dos representantes para adicionar ou atualizar em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="ec249-116">Contains the identities of delegates to add to or update in a mailbox.</span></span> <span data-ttu-id="ec249-117">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ec249-117">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="ec249-118">DeliverMeetingRequests</span><span class="sxs-lookup"><span data-stu-id="ec249-118">DeliverMeetingRequests</span></span>](delivermeetingrequests.md) <br/> |<span data-ttu-id="ec249-119">Define como as solicitações de reunião são manipuladas entre o delegado e a entidade.</span><span class="sxs-lookup"><span data-stu-id="ec249-119">Defines how meeting requests are handled between the delegate and the principal.</span></span> <span data-ttu-id="ec249-120">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ec249-120">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="ec249-121">Caixa de correio</span><span class="sxs-lookup"><span data-stu-id="ec249-121">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="ec249-122">Identifica um objeto de serviço de diretório do Active Directory habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="ec249-122">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ec249-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ec249-123">Parent elements</span></span>

<span data-ttu-id="ec249-124">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ec249-124">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ec249-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="ec249-125">Remarks</span></span>

<span data-ttu-id="ec249-126">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="ec249-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ec249-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ec249-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ec249-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="ec249-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ec249-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ec249-129">Schema Name</span></span>  <br/> |<span data-ttu-id="ec249-130">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="ec249-130">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ec249-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ec249-131">Validation File</span></span>  <br/> |<span data-ttu-id="ec249-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ec249-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ec249-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ec249-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="ec249-134">False</span><span class="sxs-lookup"><span data-stu-id="ec249-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ec249-135">Ver também</span><span class="sxs-lookup"><span data-stu-id="ec249-135">See also</span></span>

- [<span data-ttu-id="ec249-136">Operação AddDelegate</span><span class="sxs-lookup"><span data-stu-id="ec249-136">AddDelegate operation</span></span>](adddelegate-operation.md)
- [<span data-ttu-id="ec249-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ec249-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="ec249-138">Adicionando representantes</span><span class="sxs-lookup"><span data-stu-id="ec249-138">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

