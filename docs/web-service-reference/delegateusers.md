---
title: DelegateUsers
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DelegateUsers
api_type:
- schema
ms.assetid: f30f80d9-20c8-41cc-afc7-a5eec1e0c5ea
description: O elemento DelegateUsers contém as identidades de representantes a serem adicionadas ou atualizadas em uma caixa de correio. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 69f5aab65634f41ec0f820da05dee79a300fb32e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457372"
---
# <a name="delegateusers"></a><span data-ttu-id="c344b-104">DelegateUsers</span><span class="sxs-lookup"><span data-stu-id="c344b-104">DelegateUsers</span></span>

<span data-ttu-id="c344b-105">O elemento **DelegateUsers** contém as identidades de representantes a serem adicionadas ou atualizadas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c344b-105">The **DelegateUsers** element contains the identities of delegates to add to or update in a mailbox.</span></span> <span data-ttu-id="c344b-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="c344b-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DelegateUsers>
   <DelegateUser>
</DelegateUsers>
```

<span data-ttu-id="c344b-107">**ArrayOfDelegateUserType**</span><span class="sxs-lookup"><span data-stu-id="c344b-107">**ArrayOfDelegateUserType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="c344b-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c344b-108">Attributes and elements</span></span>

<span data-ttu-id="c344b-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c344b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c344b-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="c344b-110">Attributes</span></span>

<span data-ttu-id="c344b-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c344b-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c344b-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c344b-112">Child elements</span></span>

|<span data-ttu-id="c344b-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c344b-113">**Element**</span></span>|<span data-ttu-id="c344b-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c344b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c344b-115">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="c344b-115">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="c344b-116">Identifica um único representante para adicionar ou atualizar em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c344b-116">Identifies a single delegate to add to or update in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c344b-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c344b-117">Parent elements</span></span>

|<span data-ttu-id="c344b-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c344b-118">**Element**</span></span>|<span data-ttu-id="c344b-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c344b-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c344b-120">AddDelegate</span><span class="sxs-lookup"><span data-stu-id="c344b-120">AddDelegate</span></span>](adddelegate.md) <br/> |<span data-ttu-id="c344b-121">Define uma solicitação para adicionar representantes a uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c344b-121">Defines a request to add delegates to a mailbox.</span></span> <span data-ttu-id="c344b-122">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="c344b-122">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="c344b-123">UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="c344b-123">UpdateDelegate</span></span>](updatedelegate.md) <br/> |<span data-ttu-id="c344b-124">Define uma solicitação para atualizar representantes em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c344b-124">Defines a request to update delegates in a mailbox.</span></span> <span data-ttu-id="c344b-125">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="c344b-125">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c344b-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="c344b-126">Remarks</span></span>

<span data-ttu-id="c344b-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="c344b-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c344b-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c344b-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c344b-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="c344b-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c344b-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c344b-130">Schema Name</span></span>  <br/> |<span data-ttu-id="c344b-131">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="c344b-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c344b-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c344b-132">Validation File</span></span>  <br/> |<span data-ttu-id="c344b-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c344b-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c344b-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c344b-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="c344b-135">False</span><span class="sxs-lookup"><span data-stu-id="c344b-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c344b-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="c344b-136">See also</span></span>

- [<span data-ttu-id="c344b-137">Operação AddDelegate</span><span class="sxs-lookup"><span data-stu-id="c344b-137">AddDelegate operation</span></span>](adddelegate-operation.md) 
- [<span data-ttu-id="c344b-138">Operação UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="c344b-138">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="c344b-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c344b-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="c344b-140">Adicionar representantes</span><span class="sxs-lookup"><span data-stu-id="c344b-140">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

