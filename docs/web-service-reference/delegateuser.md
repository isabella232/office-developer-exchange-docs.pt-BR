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
description: O elemento DelegateUser identifica um único representante para adicionar ou atualizar em uma caixa de correio ou um Representante retornado em uma resposta de gerenciamento de representante. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 40d9dacbd544436a3edf3213cf078cd33f961a74
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458800"
---
# <a name="delegateuser"></a><span data-ttu-id="cb708-104">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="cb708-104">DelegateUser</span></span>

<span data-ttu-id="cb708-105">O elemento **DelegateUser** identifica um único representante para adicionar ou atualizar em uma caixa de correio ou um Representante retornado em uma resposta de gerenciamento de representante.</span><span class="sxs-lookup"><span data-stu-id="cb708-105">The **DelegateUser** element identifies a single delegate to add or update in a mailbox or a delegate returned in a delegate management response.</span></span> <span data-ttu-id="cb708-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="cb708-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DelegateUser>
   <UserId/>
   <DelegatePermissions/>
   <ReceiveCopiesOfMeetingMessages/>
   <ViewPrivateItems/>
</DelegateUser>
```

<span data-ttu-id="cb708-107">**DelegateUserType**</span><span class="sxs-lookup"><span data-stu-id="cb708-107">**DelegateUserType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="cb708-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="cb708-108">Attributes and elements</span></span>

<span data-ttu-id="cb708-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="cb708-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cb708-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="cb708-110">Attributes</span></span>

<span data-ttu-id="cb708-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cb708-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cb708-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="cb708-112">Child elements</span></span>

|<span data-ttu-id="cb708-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cb708-113">**Element**</span></span>|<span data-ttu-id="cb708-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cb708-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cb708-115">UserId</span><span class="sxs-lookup"><span data-stu-id="cb708-115">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="cb708-116">Identifica o representante.</span><span class="sxs-lookup"><span data-stu-id="cb708-116">Identifies the delegate.</span></span> <span data-ttu-id="cb708-117">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="cb708-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="cb708-118">DelegatePermissions</span><span class="sxs-lookup"><span data-stu-id="cb708-118">DelegatePermissions</span></span>](delegatepermissions.md) <br/> |<span data-ttu-id="cb708-119">Contém as configurações de nível de permissão de representante.</span><span class="sxs-lookup"><span data-stu-id="cb708-119">Contains the delegate permission level settings.</span></span> <span data-ttu-id="cb708-120">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="cb708-120">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="cb708-121">ReceiveCopiesOfMeetingMessages</span><span class="sxs-lookup"><span data-stu-id="cb708-121">ReceiveCopiesOfMeetingMessages</span></span>](receivecopiesofmeetingmessages.md) <br/> |<span data-ttu-id="cb708-122">Indica se um representante recebe cópias de mensagens relacionadas à reunião endereçadas à entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="cb708-122">Indicates whether a delegate receives copies of meeting-related messages that are addressed to the principal.</span></span> <span data-ttu-id="cb708-123">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="cb708-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="cb708-124">ViewPrivateItems</span><span class="sxs-lookup"><span data-stu-id="cb708-124">ViewPrivateItems</span></span>](viewprivateitems.md) <br/> |<span data-ttu-id="cb708-125">Indica se um representante tem permissão para exibir itens de calendário privados na caixa de correio da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="cb708-125">Indicates whether a delegate has permission to view private calendar items in the principal's mailbox.</span></span> <span data-ttu-id="cb708-126">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="cb708-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cb708-127">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="cb708-127">Parent elements</span></span>

|<span data-ttu-id="cb708-128">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cb708-128">**Element**</span></span>|<span data-ttu-id="cb708-129">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cb708-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cb708-130">DelegateUsers</span><span class="sxs-lookup"><span data-stu-id="cb708-130">DelegateUsers</span></span>](delegateusers.md) <br/> |<span data-ttu-id="cb708-131">Contém as identidades dos representantes a serem adicionadas ou atualizadas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="cb708-131">Contains the identities of delegates to add or update in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="cb708-132">DelegateUserResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="cb708-132">DelegateUserResponseMessageType</span></span>](delegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="cb708-133">Contém mensagens de resposta para operações de gerenciamento de representante.</span><span class="sxs-lookup"><span data-stu-id="cb708-133">Contains response messages for delegate management operations.</span></span> <span data-ttu-id="cb708-134">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="cb708-134">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cb708-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="cb708-135">Remarks</span></span>

<span data-ttu-id="cb708-136">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="cb708-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cb708-137">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="cb708-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cb708-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="cb708-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cb708-139">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="cb708-139">Schema Name</span></span>  <br/> |<span data-ttu-id="cb708-140">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="cb708-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="cb708-141">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="cb708-141">Validation File</span></span>  <br/> |<span data-ttu-id="cb708-142">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="cb708-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cb708-143">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="cb708-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="cb708-144">False</span><span class="sxs-lookup"><span data-stu-id="cb708-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cb708-145">Confira também</span><span class="sxs-lookup"><span data-stu-id="cb708-145">See also</span></span>

- [<span data-ttu-id="cb708-146">Operação AddDelegate</span><span class="sxs-lookup"><span data-stu-id="cb708-146">AddDelegate operation</span></span>](adddelegate-operation.md) 
- [<span data-ttu-id="cb708-147">Operação UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="cb708-147">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="cb708-148">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="cb708-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="cb708-149">Adicionar representantes</span><span class="sxs-lookup"><span data-stu-id="cb708-149">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

