---
title: ViewPrivateItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ViewPrivateItems
api_type:
- schema
ms.assetid: 80b949ac-440c-4a01-b428-ebafb5b1b802
description: O elemento ViewPrivateItems indica se um usuário delegado ou um aplicativo cliente tem permissão para exibir itens privados na caixa de correio da entidade de segurança.
ms.openlocfilehash: 4e1375f7c4a3c660cc5de885deff8d094250ca7b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44525966"
---
# <a name="viewprivateitems"></a><span data-ttu-id="afb30-103">ViewPrivateItems</span><span class="sxs-lookup"><span data-stu-id="afb30-103">ViewPrivateItems</span></span>

<span data-ttu-id="afb30-104">O elemento **ViewPrivateItems** indica se um usuário delegado ou um aplicativo cliente tem permissão para exibir itens privados na caixa de correio da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="afb30-104">The **ViewPrivateItems** element indicates whether a delegate user or client application has permission to view private items in the principal's mailbox.</span></span> 
  
```XML
<ViewPrivateItems>true | false</ViewPrivateItems>
```

 <span data-ttu-id="afb30-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="afb30-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="afb30-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="afb30-106">Attributes and elements</span></span>

<span data-ttu-id="afb30-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="afb30-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="afb30-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="afb30-108">Attributes</span></span>

<span data-ttu-id="afb30-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="afb30-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="afb30-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="afb30-110">Child elements</span></span>

<span data-ttu-id="afb30-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="afb30-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="afb30-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="afb30-112">Parent elements</span></span>

|<span data-ttu-id="afb30-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="afb30-113">**Element**</span></span>|<span data-ttu-id="afb30-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="afb30-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="afb30-115">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="afb30-115">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="afb30-116">Identifica um único representante para adicionar ou atualizar em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="afb30-116">Identifies a single delegate to add or update in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="afb30-117">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="afb30-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="afb30-118">Contém os direitos do cliente com base nas configurações de permissão para o item ou pasta.</span><span class="sxs-lookup"><span data-stu-id="afb30-118">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="afb30-119">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="afb30-119">This element is read-only.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="afb30-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="afb30-120">Text value</span></span>

<span data-ttu-id="afb30-121">Um valor **true** indica que o representante ou o cliente pode exibir itens privados na caixa de correio da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="afb30-121">A value of **true** indicates that the delegate or client can view private items in the principal's mailbox.</span></span> <span data-ttu-id="afb30-122">Um valor **false** indica que os itens privados não estão visíveis para um representante ou cliente.</span><span class="sxs-lookup"><span data-stu-id="afb30-122">A value of **false** indicates that private items are not visible to a delegate or client.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="afb30-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="afb30-123">Remarks</span></span>

<span data-ttu-id="afb30-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="afb30-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="afb30-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="afb30-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="afb30-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="afb30-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="afb30-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="afb30-127">Schema Name</span></span>  <br/> |<span data-ttu-id="afb30-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="afb30-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="afb30-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="afb30-129">Validation File</span></span>  <br/> |<span data-ttu-id="afb30-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="afb30-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="afb30-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="afb30-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="afb30-132">False</span><span class="sxs-lookup"><span data-stu-id="afb30-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="afb30-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="afb30-133">See also</span></span>



[<span data-ttu-id="afb30-134">Operação AddDelegate</span><span class="sxs-lookup"><span data-stu-id="afb30-134">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="afb30-135">Operação UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="afb30-135">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="afb30-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="afb30-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="afb30-137">Adicionar representantes</span><span class="sxs-lookup"><span data-stu-id="afb30-137">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

