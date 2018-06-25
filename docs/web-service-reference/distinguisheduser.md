---
title: DistinguishedUser
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DistinguishedUser
api_type:
- schema
ms.assetid: 9362699d-666a-4acf-8fa1-c6669f0a2ae5
description: O elemento DistinguishedUser identifica as contas de usuário anônimo e padrão para acesso de representante. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: b14be22bfe5316b9ab254e63cdfa0757596b8b92
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751899"
---
# <a name="distinguisheduser"></a><span data-ttu-id="95be2-104">DistinguishedUser</span><span class="sxs-lookup"><span data-stu-id="95be2-104">DistinguishedUser</span></span>

<span data-ttu-id="95be2-105">O elemento **DistinguishedUser** identifica as contas de usuário anônimo e padrão para acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="95be2-105">The **DistinguishedUser** element identifies Anonymous and Default user accounts for delegate access.</span></span> <span data-ttu-id="95be2-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="95be2-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DistinguishedUser>Default or Anonymous</DistinguishedUser>
```

 <span data-ttu-id="95be2-107">**DistinguishedUserType**</span><span class="sxs-lookup"><span data-stu-id="95be2-107">**DistinguishedUserType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="95be2-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="95be2-108">Attributes and elements</span></span>

<span data-ttu-id="95be2-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="95be2-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="95be2-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="95be2-110">Attributes</span></span>

<span data-ttu-id="95be2-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="95be2-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="95be2-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="95be2-112">Child elements</span></span>

<span data-ttu-id="95be2-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="95be2-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="95be2-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="95be2-114">Parent elements</span></span>

|<span data-ttu-id="95be2-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="95be2-115">**Element**</span></span>|<span data-ttu-id="95be2-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="95be2-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="95be2-117">UserId</span><span class="sxs-lookup"><span data-stu-id="95be2-117">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="95be2-118">Identifica um usuário delegado ou um usuário que tem permissões de acesso de pasta.</span><span class="sxs-lookup"><span data-stu-id="95be2-118">Identifies a delegate user or a user who has folder access permissions.</span></span> <span data-ttu-id="95be2-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="95be2-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="95be2-120">Text value</span><span class="sxs-lookup"><span data-stu-id="95be2-120">Text value</span></span>

<span data-ttu-id="95be2-121">Um valor de texto do **padrão** descreve a configuração padrão para os usuários de representante que são adicionados à caixa de correio do principal.</span><span class="sxs-lookup"><span data-stu-id="95be2-121">A text value of **Default** describes the default setting for delegate users who are added to the principal's mailbox.</span></span> <span data-ttu-id="95be2-122">Um valor de texto de **anônimo** descreve as configurações de acesso de representante que os usuários anônimos terão na caixa de correio do principal.</span><span class="sxs-lookup"><span data-stu-id="95be2-122">A text value of **Anonymous** describes the delegate access settings that anonymous users have on the principal's mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="95be2-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="95be2-123">Remarks</span></span>

<span data-ttu-id="95be2-124">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="95be2-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="95be2-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="95be2-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="95be2-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="95be2-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="95be2-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="95be2-127">Schema Name</span></span>  <br/> |<span data-ttu-id="95be2-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="95be2-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="95be2-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="95be2-129">Validation File</span></span>  <br/> |<span data-ttu-id="95be2-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="95be2-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="95be2-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="95be2-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="95be2-132">False</span><span class="sxs-lookup"><span data-stu-id="95be2-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="95be2-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="95be2-133">See also</span></span>

- [<span data-ttu-id="95be2-134">Operação AddDelegate</span><span class="sxs-lookup"><span data-stu-id="95be2-134">AddDelegate operation</span></span>](adddelegate-operation.md)  
- [<span data-ttu-id="95be2-135">Operação UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="95be2-135">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="95be2-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="95be2-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="95be2-137">Adicionando representantes</span><span class="sxs-lookup"><span data-stu-id="95be2-137">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

