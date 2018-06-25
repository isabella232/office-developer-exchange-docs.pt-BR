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
description: Os UserIds elemento contém uma matriz de delegar usuários para obter ou remova a caixa de correio da entidade de segurança. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 277ae96fdbc30f1b39ef20553e10ff1de3ff7a8b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837984"
---
# <a name="userids"></a><span data-ttu-id="f8fc9-104">UserIds</span><span class="sxs-lookup"><span data-stu-id="f8fc9-104">UserIds</span></span>

<span data-ttu-id="f8fc9-105">O elemento **UserIds** contém uma matriz de usuários do representante para obter ou remova a caixa de correio da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="f8fc9-105">The **UserIds** element contains an array of delegate users to get or remove from a principal's mailbox.</span></span> <span data-ttu-id="f8fc9-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="f8fc9-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<UserIds>
   <UserId/>
</UserIds>
```

 <span data-ttu-id="f8fc9-107">**ArrayOfUserIdType**</span><span class="sxs-lookup"><span data-stu-id="f8fc9-107">**ArrayOfUserIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f8fc9-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f8fc9-108">Attributes and elements</span></span>

<span data-ttu-id="f8fc9-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f8fc9-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f8fc9-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="f8fc9-110">Attributes</span></span>

<span data-ttu-id="f8fc9-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f8fc9-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f8fc9-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f8fc9-112">Child elements</span></span>

|<span data-ttu-id="f8fc9-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f8fc9-113">**Element**</span></span>|<span data-ttu-id="f8fc9-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f8fc9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f8fc9-115">UserId</span><span class="sxs-lookup"><span data-stu-id="f8fc9-115">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="f8fc9-116">Identifica um representante para obter ou remova a caixa de correio da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="f8fc9-116">Identifies a delegate to get or remove from a principal's mailbox.</span></span> <span data-ttu-id="f8fc9-117">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="f8fc9-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f8fc9-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f8fc9-118">Parent elements</span></span>

|<span data-ttu-id="f8fc9-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f8fc9-119">**Element**</span></span>|<span data-ttu-id="f8fc9-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f8fc9-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f8fc9-121">GetDelegate</span><span class="sxs-lookup"><span data-stu-id="f8fc9-121">GetDelegate</span></span>](getdelegate.md) <br/> |<span data-ttu-id="f8fc9-122">Define uma solicitação para obter mais informações sobre os representantes para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="f8fc9-122">Defines a request to get information about delegates to a mailbox.</span></span> <span data-ttu-id="f8fc9-123">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="f8fc9-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="f8fc9-124">RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="f8fc9-124">RemoveDelegate</span></span>](removedelegate.md) <br/> |<span data-ttu-id="f8fc9-125">Define uma solicitação para remover representantes de uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="f8fc9-125">Defines a request to remove delegates from a mailbox.</span></span> <span data-ttu-id="f8fc9-126">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="f8fc9-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f8fc9-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="f8fc9-127">Remarks</span></span>

<span data-ttu-id="f8fc9-128">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="f8fc9-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f8fc9-129">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f8fc9-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f8fc9-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="f8fc9-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f8fc9-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f8fc9-131">Schema Name</span></span>  <br/> |<span data-ttu-id="f8fc9-132">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="f8fc9-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f8fc9-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f8fc9-133">Validation File</span></span>  <br/> |<span data-ttu-id="f8fc9-134">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f8fc9-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f8fc9-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f8fc9-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="f8fc9-136">False</span><span class="sxs-lookup"><span data-stu-id="f8fc9-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f8fc9-137">Ver também</span><span class="sxs-lookup"><span data-stu-id="f8fc9-137">See also</span></span>



[<span data-ttu-id="f8fc9-138">Operação GetDelegate</span><span class="sxs-lookup"><span data-stu-id="f8fc9-138">GetDelegate operation</span></span>](getdelegate-operation.md)
  
[<span data-ttu-id="f8fc9-139">Operação RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="f8fc9-139">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="f8fc9-140">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f8fc9-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

