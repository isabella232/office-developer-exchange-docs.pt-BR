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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459774"
---
# <a name="userids"></a><span data-ttu-id="47f69-104">UserIds</span><span class="sxs-lookup"><span data-stu-id="47f69-104">UserIds</span></span>

<span data-ttu-id="47f69-105">O elemento **userids** contém uma matriz de usuários delegados a serem obtidos ou removidos da caixa de correio de uma entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="47f69-105">The **UserIds** element contains an array of delegate users to get or remove from a principal's mailbox.</span></span> <span data-ttu-id="47f69-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="47f69-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<UserIds>
   <UserId/>
</UserIds>
```

 <span data-ttu-id="47f69-107">**ArrayOfUserIdType**</span><span class="sxs-lookup"><span data-stu-id="47f69-107">**ArrayOfUserIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="47f69-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="47f69-108">Attributes and elements</span></span>

<span data-ttu-id="47f69-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="47f69-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="47f69-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="47f69-110">Attributes</span></span>

<span data-ttu-id="47f69-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="47f69-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="47f69-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="47f69-112">Child elements</span></span>

|<span data-ttu-id="47f69-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="47f69-113">**Element**</span></span>|<span data-ttu-id="47f69-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="47f69-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="47f69-115">UserId</span><span class="sxs-lookup"><span data-stu-id="47f69-115">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="47f69-116">Identifica um representante para obter ou remover da caixa de correio de uma entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="47f69-116">Identifies a delegate to get or remove from a principal's mailbox.</span></span> <span data-ttu-id="47f69-117">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="47f69-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="47f69-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="47f69-118">Parent elements</span></span>

|<span data-ttu-id="47f69-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="47f69-119">**Element**</span></span>|<span data-ttu-id="47f69-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="47f69-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="47f69-121">Getdelegate</span><span class="sxs-lookup"><span data-stu-id="47f69-121">GetDelegate</span></span>](getdelegate.md) <br/> |<span data-ttu-id="47f69-122">Define uma solicitação para obter informações sobre representantes para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="47f69-122">Defines a request to get information about delegates to a mailbox.</span></span> <span data-ttu-id="47f69-123">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="47f69-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="47f69-124">RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="47f69-124">RemoveDelegate</span></span>](removedelegate.md) <br/> |<span data-ttu-id="47f69-125">Define uma solicitação para remover representantes de uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="47f69-125">Defines a request to remove delegates from a mailbox.</span></span> <span data-ttu-id="47f69-126">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="47f69-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="47f69-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="47f69-127">Remarks</span></span>

<span data-ttu-id="47f69-128">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="47f69-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="47f69-129">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="47f69-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="47f69-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="47f69-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="47f69-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="47f69-131">Schema Name</span></span>  <br/> |<span data-ttu-id="47f69-132">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="47f69-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="47f69-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="47f69-133">Validation File</span></span>  <br/> |<span data-ttu-id="47f69-134">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="47f69-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="47f69-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="47f69-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="47f69-136">False</span><span class="sxs-lookup"><span data-stu-id="47f69-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="47f69-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="47f69-137">See also</span></span>



[<span data-ttu-id="47f69-138">Operação getdelegate</span><span class="sxs-lookup"><span data-stu-id="47f69-138">GetDelegate operation</span></span>](getdelegate-operation.md)
  
[<span data-ttu-id="47f69-139">Operação RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="47f69-139">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="47f69-140">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="47f69-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

