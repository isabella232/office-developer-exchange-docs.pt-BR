---
title: UserIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserIds
api_type:
- schema
ms.assetid: 78a09c3a-1646-4c55-95a2-1109fb11e1c6
description: O elemento UserIds contém uma matriz de usuários delegados a serem obtidos ou removidos da caixa de correio de uma entidade de segurança. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: de4661226c154ef0d2d5ac55c57405e20c4d2aee
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459774"
---
# <a name="userids"></a><span data-ttu-id="94dc8-104">UserIds</span><span class="sxs-lookup"><span data-stu-id="94dc8-104">UserIds</span></span>

<span data-ttu-id="94dc8-105">O elemento **userids** contém uma matriz de usuários delegados a serem obtidos ou removidos da caixa de correio de uma entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="94dc8-105">The **UserIds** element contains an array of delegate users to get or remove from a principal's mailbox.</span></span> <span data-ttu-id="94dc8-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="94dc8-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<UserIds>
   <UserId/>
</UserIds>
```

 <span data-ttu-id="94dc8-107">**ArrayOfUserIdType**</span><span class="sxs-lookup"><span data-stu-id="94dc8-107">**ArrayOfUserIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="94dc8-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="94dc8-108">Attributes and elements</span></span>

<span data-ttu-id="94dc8-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="94dc8-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="94dc8-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="94dc8-110">Attributes</span></span>

<span data-ttu-id="94dc8-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="94dc8-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="94dc8-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="94dc8-112">Child elements</span></span>

|<span data-ttu-id="94dc8-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="94dc8-113">**Element**</span></span>|<span data-ttu-id="94dc8-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="94dc8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="94dc8-115">UserId</span><span class="sxs-lookup"><span data-stu-id="94dc8-115">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="94dc8-116">Identifica um representante para obter ou remover da caixa de correio de uma entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="94dc8-116">Identifies a delegate to get or remove from a principal's mailbox.</span></span> <span data-ttu-id="94dc8-117">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="94dc8-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="94dc8-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="94dc8-118">Parent elements</span></span>

|<span data-ttu-id="94dc8-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="94dc8-119">**Element**</span></span>|<span data-ttu-id="94dc8-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="94dc8-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="94dc8-121">Getdelegate</span><span class="sxs-lookup"><span data-stu-id="94dc8-121">GetDelegate</span></span>](getdelegate.md) <br/> |<span data-ttu-id="94dc8-122">Define uma solicitação para obter informações sobre representantes para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="94dc8-122">Defines a request to get information about delegates to a mailbox.</span></span> <span data-ttu-id="94dc8-123">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="94dc8-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="94dc8-124">RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="94dc8-124">RemoveDelegate</span></span>](removedelegate.md) <br/> |<span data-ttu-id="94dc8-125">Define uma solicitação para remover representantes de uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="94dc8-125">Defines a request to remove delegates from a mailbox.</span></span> <span data-ttu-id="94dc8-126">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="94dc8-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="94dc8-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="94dc8-127">Remarks</span></span>

<span data-ttu-id="94dc8-128">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="94dc8-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="94dc8-129">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="94dc8-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="94dc8-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="94dc8-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="94dc8-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="94dc8-131">Schema Name</span></span>  <br/> |<span data-ttu-id="94dc8-132">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="94dc8-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="94dc8-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="94dc8-133">Validation File</span></span>  <br/> |<span data-ttu-id="94dc8-134">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="94dc8-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="94dc8-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="94dc8-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="94dc8-136">False</span><span class="sxs-lookup"><span data-stu-id="94dc8-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="94dc8-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="94dc8-137">See also</span></span>



[<span data-ttu-id="94dc8-138">Operação getdelegate</span><span class="sxs-lookup"><span data-stu-id="94dc8-138">GetDelegate operation</span></span>](getdelegate-operation.md)
  
[<span data-ttu-id="94dc8-139">Operação RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="94dc8-139">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="94dc8-140">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="94dc8-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

