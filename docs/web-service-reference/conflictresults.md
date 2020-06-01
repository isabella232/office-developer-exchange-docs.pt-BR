---
title: ConflictResults
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConflictResults
api_type:
- schema
ms.assetid: 08cdd547-4de7-4c7a-b60f-e618dc217d20
description: O elemento ConflictResults contém o número de conflitos em uma resposta de operação UpdateItem.
ms.openlocfilehash: 923c7950e21039adf28e232486f4df5fc04889d1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460166"
---
# <a name="conflictresults"></a><span data-ttu-id="06832-103">ConflictResults</span><span class="sxs-lookup"><span data-stu-id="06832-103">ConflictResults</span></span>

<span data-ttu-id="06832-104">O elemento [ConflictResults](conflictresults.md) contém o número de conflitos em uma resposta de [operação UpdateItem](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="06832-104">The [ConflictResults](conflictresults.md) element contains the number of conflicts in an [UpdateItem operation](updateitem-operation.md) response.</span></span> 
  
[<span data-ttu-id="06832-105">UpdateItemResponse</span><span class="sxs-lookup"><span data-stu-id="06832-105">UpdateItemResponse</span></span>](updateitemresponse.md)
  
[<span data-ttu-id="06832-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="06832-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="06832-107">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="06832-107">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
  
[<span data-ttu-id="06832-108">ConflictResults</span><span class="sxs-lookup"><span data-stu-id="06832-108">ConflictResults</span></span>](conflictresults.md)
  
```xml
<ConflictResults>
   <Count/>
</ConflictResults>
```

 <span data-ttu-id="06832-109">**ConflictResultsType**</span><span class="sxs-lookup"><span data-stu-id="06832-109">**ConflictResultsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="06832-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="06832-110">Attributes and elements</span></span>

<span data-ttu-id="06832-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="06832-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="06832-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="06832-112">Attributes</span></span>

<span data-ttu-id="06832-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="06832-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="06832-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="06832-114">Child elements</span></span>

|<span data-ttu-id="06832-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="06832-115">**Element**</span></span>|<span data-ttu-id="06832-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="06832-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="06832-117">Count</span><span class="sxs-lookup"><span data-stu-id="06832-117">Count</span></span>](count.md) <br/> |<span data-ttu-id="06832-118">Contém o número de conflitos em uma resposta de [operação UpdateItem](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="06832-118">Contains the number of conflicts in an [UpdateItem operation](updateitem-operation.md) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="06832-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="06832-119">Parent elements</span></span>

|<span data-ttu-id="06832-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="06832-120">**Element**</span></span>|<span data-ttu-id="06832-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="06832-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="06832-122">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="06832-122">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md) <br/> |<span data-ttu-id="06832-123">Contém o status e o resultado de uma única solicitação de [operação UpdateItem](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="06832-123">Contains the status and result of a single [UpdateItem operation](updateitem-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="06832-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="06832-124">Remarks</span></span>

<span data-ttu-id="06832-125">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Exchange Server com a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="06832-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="06832-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="06832-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="06832-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="06832-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="06832-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="06832-128">Schema Name</span></span>  <br/> |<span data-ttu-id="06832-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="06832-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="06832-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="06832-130">Validation File</span></span>  <br/> |<span data-ttu-id="06832-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="06832-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="06832-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="06832-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="06832-133">False</span><span class="sxs-lookup"><span data-stu-id="06832-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="06832-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="06832-134">See also</span></span>



[<span data-ttu-id="06832-135">Operação UpdateItem</span><span class="sxs-lookup"><span data-stu-id="06832-135">UpdateItem operation</span></span>](updateitem-operation.md)
  
 <span data-ttu-id="06832-136">**ConflictResultsType**</span><span class="sxs-lookup"><span data-stu-id="06832-136">**ConflictResultsType**</span></span>

