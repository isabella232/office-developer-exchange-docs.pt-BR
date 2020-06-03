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
description: O elemento DistinguishedUser identifica contas de usuário anônimas e padrão para acesso de representante. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 922c36251290d7090cdafbed9e570144593ca97e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530730"
---
# <a name="distinguisheduser"></a><span data-ttu-id="40d1b-104">DistinguishedUser</span><span class="sxs-lookup"><span data-stu-id="40d1b-104">DistinguishedUser</span></span>

<span data-ttu-id="40d1b-105">O elemento **DistinguishedUser** identifica contas de usuário anônimas e padrão para acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="40d1b-105">The **DistinguishedUser** element identifies Anonymous and Default user accounts for delegate access.</span></span> <span data-ttu-id="40d1b-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="40d1b-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DistinguishedUser>Default or Anonymous</DistinguishedUser>
```

 <span data-ttu-id="40d1b-107">**DistinguishedUserType**</span><span class="sxs-lookup"><span data-stu-id="40d1b-107">**DistinguishedUserType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="40d1b-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="40d1b-108">Attributes and elements</span></span>

<span data-ttu-id="40d1b-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="40d1b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="40d1b-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="40d1b-110">Attributes</span></span>

<span data-ttu-id="40d1b-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="40d1b-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="40d1b-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="40d1b-112">Child elements</span></span>

<span data-ttu-id="40d1b-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="40d1b-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="40d1b-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="40d1b-114">Parent elements</span></span>

|<span data-ttu-id="40d1b-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="40d1b-115">**Element**</span></span>|<span data-ttu-id="40d1b-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="40d1b-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="40d1b-117">UserId</span><span class="sxs-lookup"><span data-stu-id="40d1b-117">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="40d1b-118">Identifica um usuário delegado ou um usuário com permissões de acesso à pasta.</span><span class="sxs-lookup"><span data-stu-id="40d1b-118">Identifies a delegate user or a user who has folder access permissions.</span></span> <span data-ttu-id="40d1b-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="40d1b-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="40d1b-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="40d1b-120">Text value</span></span>

<span data-ttu-id="40d1b-121">Um valor **padrão** de texto descreve a configuração padrão para usuários delegados que são adicionados à caixa de correio da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="40d1b-121">A text value of **Default** describes the default setting for delegate users who are added to the principal's mailbox.</span></span> <span data-ttu-id="40d1b-122">Um valor de texto **anônimo** descreve as configurações de acesso de representante que os usuários anônimos têm na caixa de correio da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="40d1b-122">A text value of **Anonymous** describes the delegate access settings that anonymous users have on the principal's mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="40d1b-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="40d1b-123">Remarks</span></span>

<span data-ttu-id="40d1b-124">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="40d1b-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="40d1b-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="40d1b-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="40d1b-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="40d1b-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="40d1b-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="40d1b-127">Schema Name</span></span>  <br/> |<span data-ttu-id="40d1b-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="40d1b-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="40d1b-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="40d1b-129">Validation File</span></span>  <br/> |<span data-ttu-id="40d1b-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="40d1b-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="40d1b-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="40d1b-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="40d1b-132">False</span><span class="sxs-lookup"><span data-stu-id="40d1b-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="40d1b-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="40d1b-133">See also</span></span>

- [<span data-ttu-id="40d1b-134">Operação AddDelegate</span><span class="sxs-lookup"><span data-stu-id="40d1b-134">AddDelegate operation</span></span>](adddelegate-operation.md)  
- [<span data-ttu-id="40d1b-135">Operação UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="40d1b-135">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="40d1b-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="40d1b-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="40d1b-137">Adicionar representantes</span><span class="sxs-lookup"><span data-stu-id="40d1b-137">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

