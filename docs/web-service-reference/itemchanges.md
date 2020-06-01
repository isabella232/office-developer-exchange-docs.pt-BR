---
title: Alterações
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemChanges
api_type:
- schema
ms.assetid: cd307892-2f69-4494-8325-219bdb5c3ad5
description: O elemento items contém uma matriz de elementos ItemChange que identificam itens e as atualizações a serem aplicadas aos itens.
ms.openlocfilehash: ea6fb2023b88360f9558057e80c7fe0d855173b5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459907"
---
# <a name="itemchanges"></a><span data-ttu-id="7e0f2-103">Alterações</span><span class="sxs-lookup"><span data-stu-id="7e0f2-103">ItemChanges</span></span>

<span data-ttu-id="7e0f2-104">O **elemento** Items contém uma matriz de elementos [ItemChange](itemchange.md) que identificam itens e as atualizações a serem aplicadas aos itens.</span><span class="sxs-lookup"><span data-stu-id="7e0f2-104">The **ItemChanges** element contains an array of [ItemChange](itemchange.md) elements that identify items and the updates to apply to the items.</span></span> 
  
[<span data-ttu-id="7e0f2-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="7e0f2-105">UpdateItem</span></span>](updateitem.md)
  
[<span data-ttu-id="7e0f2-106">Alterações</span><span class="sxs-lookup"><span data-stu-id="7e0f2-106">ItemChanges</span></span>](itemchanges.md)
  
```xml
<ItemChanges>
   <ItemChange/>
</ItemChanges>
```

 <span data-ttu-id="7e0f2-107">**NonEmptyArrayOfItemChangesType**</span><span class="sxs-lookup"><span data-stu-id="7e0f2-107">**NonEmptyArrayOfItemChangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7e0f2-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="7e0f2-108">Attributes and elements</span></span>

<span data-ttu-id="7e0f2-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7e0f2-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e0f2-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="7e0f2-110">Attributes</span></span>

<span data-ttu-id="7e0f2-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7e0f2-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7e0f2-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7e0f2-112">Child elements</span></span>

|<span data-ttu-id="7e0f2-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7e0f2-113">**Element**</span></span>|<span data-ttu-id="7e0f2-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7e0f2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e0f2-115">ItemChange</span><span class="sxs-lookup"><span data-stu-id="7e0f2-115">ItemChange</span></span>](itemchange.md) <br/> |<span data-ttu-id="7e0f2-116">Contém um identificador de item e as atualizações a serem aplicadas ao item.</span><span class="sxs-lookup"><span data-stu-id="7e0f2-116">Contains an item identifier and the updates to apply to the item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7e0f2-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7e0f2-117">Parent elements</span></span>

|<span data-ttu-id="7e0f2-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7e0f2-118">**Element**</span></span>|<span data-ttu-id="7e0f2-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7e0f2-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e0f2-120">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="7e0f2-120">UpdateItem</span></span>](updateitem.md) <br/> |<span data-ttu-id="7e0f2-121">Define uma solicitação para atualizar itens em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7e0f2-121">Defines a request to update items in a mailbox.</span></span>  <br/> <span data-ttu-id="7e0f2-122">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="7e0f2-122">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7e0f2-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="7e0f2-123">Remarks</span></span>

<span data-ttu-id="7e0f2-124">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="7e0f2-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7e0f2-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="7e0f2-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e0f2-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="7e0f2-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7e0f2-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7e0f2-127">Schema Name</span></span>  <br/> |<span data-ttu-id="7e0f2-128">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="7e0f2-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7e0f2-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7e0f2-129">Validation File</span></span>  <br/> |<span data-ttu-id="7e0f2-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7e0f2-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7e0f2-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="7e0f2-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="7e0f2-132">False</span><span class="sxs-lookup"><span data-stu-id="7e0f2-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7e0f2-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="7e0f2-133">See also</span></span>



[<span data-ttu-id="7e0f2-134">Operação UpdateItem</span><span class="sxs-lookup"><span data-stu-id="7e0f2-134">UpdateItem operation</span></span>](updateitem-operation.md)

