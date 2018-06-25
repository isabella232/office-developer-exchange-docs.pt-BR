---
title: DelegateUser
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DelegateUser
api_type:
- schema
ms.assetid: aac4e74e-f69b-4c41-a0c9-489610330fbf
description: O elemento DelegateUser identifica um único representante para adicionar ou atualizar em uma caixa de correio ou um representante retornados em uma resposta de gerenciamento do representante. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 72ddc313a5a76cd0345918cad63b7775ff85026b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751722"
---
# <a name="delegateuser"></a><span data-ttu-id="49619-104">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="49619-104">DelegateUser</span></span>

<span data-ttu-id="49619-105">O elemento **DelegateUser** identifica um único representante para adicionar ou atualizar em uma caixa de correio ou um representante retornados em uma resposta de gerenciamento do representante.</span><span class="sxs-lookup"><span data-stu-id="49619-105">The **DelegateUser** element identifies a single delegate to add or update in a mailbox or a delegate returned in a delegate management response.</span></span> <span data-ttu-id="49619-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="49619-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DelegateUser>
   <UserId/>
   <DelegatePermissions/>
   <ReceiveCopiesOfMeetingMessages/>
   <ViewPrivateItems/>
</DelegateUser>
```

<span data-ttu-id="49619-107">**DelegateUserType**</span><span class="sxs-lookup"><span data-stu-id="49619-107">**DelegateUserType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="49619-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="49619-108">Attributes and elements</span></span>

<span data-ttu-id="49619-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="49619-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="49619-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="49619-110">Attributes</span></span>

<span data-ttu-id="49619-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="49619-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="49619-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="49619-112">Child elements</span></span>

|<span data-ttu-id="49619-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="49619-113">**Element**</span></span>|<span data-ttu-id="49619-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="49619-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="49619-115">UserId</span><span class="sxs-lookup"><span data-stu-id="49619-115">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="49619-116">Identifica o delegado.</span><span class="sxs-lookup"><span data-stu-id="49619-116">Identifies the delegate.</span></span> <span data-ttu-id="49619-117">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="49619-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="49619-118">DelegatePermissions</span><span class="sxs-lookup"><span data-stu-id="49619-118">DelegatePermissions</span></span>](delegatepermissions.md) <br/> |<span data-ttu-id="49619-119">Contém as configurações de nível de permissão de representante.</span><span class="sxs-lookup"><span data-stu-id="49619-119">Contains the delegate permission level settings.</span></span> <span data-ttu-id="49619-120">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="49619-120">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="49619-121">ReceiveCopiesOfMeetingMessages</span><span class="sxs-lookup"><span data-stu-id="49619-121">ReceiveCopiesOfMeetingMessages</span></span>](receivecopiesofmeetingmessages.md) <br/> |<span data-ttu-id="49619-122">Indica se um delegado receba cópias de mensagens relacionadas a reuniões que são abordadas à entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="49619-122">Indicates whether a delegate receives copies of meeting-related messages that are addressed to the principal.</span></span> <span data-ttu-id="49619-123">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="49619-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="49619-124">ViewPrivateItems</span><span class="sxs-lookup"><span data-stu-id="49619-124">ViewPrivateItems</span></span>](viewprivateitems.md) <br/> |<span data-ttu-id="49619-125">Indica se um delegado tem permissão para exibir itens de calendário particular na caixa de correio do principal.</span><span class="sxs-lookup"><span data-stu-id="49619-125">Indicates whether a delegate has permission to view private calendar items in the principal's mailbox.</span></span> <span data-ttu-id="49619-126">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="49619-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="49619-127">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="49619-127">Parent elements</span></span>

|<span data-ttu-id="49619-128">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="49619-128">**Element**</span></span>|<span data-ttu-id="49619-129">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="49619-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="49619-130">DelegateUsers</span><span class="sxs-lookup"><span data-stu-id="49619-130">DelegateUsers</span></span>](delegateusers.md) <br/> |<span data-ttu-id="49619-131">Contém as identidades dos representantes para adicionar ou atualizar em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="49619-131">Contains the identities of delegates to add or update in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="49619-132">DelegateUserResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="49619-132">DelegateUserResponseMessageType</span></span>](delegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="49619-133">Contém mensagens de resposta para operações de gerenciamento de representante.</span><span class="sxs-lookup"><span data-stu-id="49619-133">Contains response messages for delegate management operations.</span></span> <span data-ttu-id="49619-134">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="49619-134">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="49619-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="49619-135">Remarks</span></span>

<span data-ttu-id="49619-136">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="49619-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="49619-137">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="49619-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="49619-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="49619-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="49619-139">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="49619-139">Schema Name</span></span>  <br/> |<span data-ttu-id="49619-140">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="49619-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="49619-141">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="49619-141">Validation File</span></span>  <br/> |<span data-ttu-id="49619-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="49619-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="49619-143">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="49619-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="49619-144">False</span><span class="sxs-lookup"><span data-stu-id="49619-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="49619-145">Ver também</span><span class="sxs-lookup"><span data-stu-id="49619-145">See also</span></span>

- [<span data-ttu-id="49619-146">Operação AddDelegate</span><span class="sxs-lookup"><span data-stu-id="49619-146">AddDelegate operation</span></span>](adddelegate-operation.md) 
- [<span data-ttu-id="49619-147">Operação UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="49619-147">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="49619-148">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="49619-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="49619-149">Adicionando representantes</span><span class="sxs-lookup"><span data-stu-id="49619-149">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

