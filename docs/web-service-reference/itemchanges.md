---
title: ItemChanges
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
description: O elemento ItemChanges contém uma matriz de elementos ItemChange que identificam os itens e as atualizações para aplicar aos itens.
ms.openlocfilehash: 38fe112441a8773a2d6b494ed57c63341cab2b58
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824141"
---
# <a name="itemchanges"></a><span data-ttu-id="2bb81-103">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="2bb81-103">ItemChanges</span></span>

<span data-ttu-id="2bb81-104">O elemento **ItemChanges** contém uma matriz de elementos [ItemChange](itemchange.md) que identificam os itens e as atualizações para aplicar aos itens.</span><span class="sxs-lookup"><span data-stu-id="2bb81-104">The **ItemChanges** element contains an array of [ItemChange](itemchange.md) elements that identify items and the updates to apply to the items.</span></span> 
  
[<span data-ttu-id="2bb81-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="2bb81-105">UpdateItem</span></span>](updateitem.md)
  
[<span data-ttu-id="2bb81-106">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="2bb81-106">ItemChanges</span></span>](itemchanges.md)
  
```xml
<ItemChanges>
   <ItemChange/>
</ItemChanges>
```

 <span data-ttu-id="2bb81-107">**NonEmptyArrayOfItemChangesType**</span><span class="sxs-lookup"><span data-stu-id="2bb81-107">**NonEmptyArrayOfItemChangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2bb81-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="2bb81-108">Attributes and elements</span></span>

<span data-ttu-id="2bb81-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2bb81-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2bb81-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="2bb81-110">Attributes</span></span>

<span data-ttu-id="2bb81-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2bb81-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2bb81-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2bb81-112">Child elements</span></span>

|<span data-ttu-id="2bb81-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2bb81-113">**Element**</span></span>|<span data-ttu-id="2bb81-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2bb81-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2bb81-115">ItemChange</span><span class="sxs-lookup"><span data-stu-id="2bb81-115">ItemChange</span></span>](itemchange.md) <br/> |<span data-ttu-id="2bb81-116">Contém um identificador de item e as atualizações para aplicar ao item.</span><span class="sxs-lookup"><span data-stu-id="2bb81-116">Contains an item identifier and the updates to apply to the item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2bb81-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2bb81-117">Parent elements</span></span>

|<span data-ttu-id="2bb81-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2bb81-118">**Element**</span></span>|<span data-ttu-id="2bb81-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2bb81-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2bb81-120">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="2bb81-120">UpdateItem</span></span>](updateitem.md) <br/> |<span data-ttu-id="2bb81-121">Define uma solicitação de atualização de itens em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2bb81-121">Defines a request to update items in a mailbox.</span></span>  <br/> <span data-ttu-id="2bb81-122">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="2bb81-122">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2bb81-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="2bb81-123">Remarks</span></span>

<span data-ttu-id="2bb81-124">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="2bb81-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2bb81-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="2bb81-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2bb81-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="2bb81-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2bb81-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2bb81-127">Schema Name</span></span>  <br/> |<span data-ttu-id="2bb81-128">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="2bb81-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2bb81-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2bb81-129">Validation File</span></span>  <br/> |<span data-ttu-id="2bb81-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2bb81-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2bb81-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="2bb81-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="2bb81-132">False</span><span class="sxs-lookup"><span data-stu-id="2bb81-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2bb81-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="2bb81-133">See also</span></span>



[<span data-ttu-id="2bb81-134">Operação UpdateItem</span><span class="sxs-lookup"><span data-stu-id="2bb81-134">UpdateItem operation</span></span>](updateitem-operation.md)

