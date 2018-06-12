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
description: O elemento ViewPrivateItems indica se um aplicativo de cliente ou de usuário delegado tem permissão para exibir itens particulares na caixa de correio do principal.
ms.openlocfilehash: c35f24ae79e907424cb5cfb0efeec2307334ca12
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838042"
---
# <a name="viewprivateitems"></a><span data-ttu-id="9ed4d-103">ViewPrivateItems</span><span class="sxs-lookup"><span data-stu-id="9ed4d-103">ViewPrivateItems</span></span>

<span data-ttu-id="9ed4d-104">O elemento **ViewPrivateItems** indica se um aplicativo de cliente ou de usuário delegado tem permissão para exibir itens particulares na caixa de correio do principal.</span><span class="sxs-lookup"><span data-stu-id="9ed4d-104">The **ViewPrivateItems** element indicates whether a delegate user or client application has permission to view private items in the principal's mailbox.</span></span> 
  
```XML
<ViewPrivateItems>true | false</ViewPrivateItems>
```

 <span data-ttu-id="9ed4d-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="9ed4d-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9ed4d-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="9ed4d-106">Attributes and elements</span></span>

<span data-ttu-id="9ed4d-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9ed4d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9ed4d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9ed4d-108">Attributes</span></span>

<span data-ttu-id="9ed4d-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9ed4d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9ed4d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9ed4d-110">Child elements</span></span>

<span data-ttu-id="9ed4d-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9ed4d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9ed4d-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9ed4d-112">Parent elements</span></span>

|<span data-ttu-id="9ed4d-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9ed4d-113">**Element**</span></span>|<span data-ttu-id="9ed4d-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9ed4d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ed4d-115">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="9ed4d-115">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="9ed4d-116">Identifica um único representante para adicionar ou atualizar em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="9ed4d-116">Identifies a single delegate to add or update in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="9ed4d-117">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="9ed4d-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="9ed4d-118">Contém os direitos do cliente com base nas configurações de permissão para o item ou a pasta.</span><span class="sxs-lookup"><span data-stu-id="9ed4d-118">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="9ed4d-119">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9ed4d-119">This element is read-only.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9ed4d-120">Text value</span><span class="sxs-lookup"><span data-stu-id="9ed4d-120">Text value</span></span>

<span data-ttu-id="9ed4d-121">Um valor **true** indica que o (s) representante (cliente possa exibir itens particulares na caixa de correio do principal.</span><span class="sxs-lookup"><span data-stu-id="9ed4d-121">A value of **true** indicates that the delegate or client can view private items in the principal's mailbox.</span></span> <span data-ttu-id="9ed4d-122">Um valor **false** indica que não são visíveis para um cliente ou representante itens particulares.</span><span class="sxs-lookup"><span data-stu-id="9ed4d-122">A value of **false** indicates that private items are not visible to a delegate or client.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="9ed4d-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="9ed4d-123">Remarks</span></span>

<span data-ttu-id="9ed4d-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9ed4d-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9ed4d-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="9ed4d-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9ed4d-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="9ed4d-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9ed4d-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9ed4d-127">Schema Name</span></span>  <br/> |<span data-ttu-id="9ed4d-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="9ed4d-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="9ed4d-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9ed4d-129">Validation File</span></span>  <br/> |<span data-ttu-id="9ed4d-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9ed4d-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9ed4d-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9ed4d-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="9ed4d-132">False</span><span class="sxs-lookup"><span data-stu-id="9ed4d-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9ed4d-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="9ed4d-133">See also</span></span>



[<span data-ttu-id="9ed4d-134">Operação AddDelegate</span><span class="sxs-lookup"><span data-stu-id="9ed4d-134">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="9ed4d-135">Operação UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="9ed4d-135">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="9ed4d-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9ed4d-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="9ed4d-137">Adicionando representantes</span><span class="sxs-lookup"><span data-stu-id="9ed4d-137">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

