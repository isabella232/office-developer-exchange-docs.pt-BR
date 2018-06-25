---
title: ItemIds (NonEmptyArrayOfItemIdsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemIds
api_type:
- schema
ms.assetid: e895782a-74fe-4216-8ac2-c3c88c4b232d
description: O elemento ItemIds contém uma matriz de identificadores de item que identificam os itens para exportar de uma caixa de correio.
ms.openlocfilehash: c6d48832c5435080c7cec8e43093ea60825b604a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824151"
---
# <a name="itemids-nonemptyarrayofitemidstype"></a><span data-ttu-id="2718a-103">ItemIds (NonEmptyArrayOfItemIdsType)</span><span class="sxs-lookup"><span data-stu-id="2718a-103">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>

<span data-ttu-id="2718a-104">O elemento **ItemIds** contém uma matriz de identificadores de item que identificam os itens para exportar de uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2718a-104">The **ItemIds** element contains an array of item identifiers that identify the items to export from a mailbox.</span></span> 
  
[<span data-ttu-id="2718a-105">ExportItems</span><span class="sxs-lookup"><span data-stu-id="2718a-105">ExportItems</span></span>](exportitems.md)
  
[<span data-ttu-id="2718a-106">ItemIds (NonEmptyArrayOfItemIdsType)</span><span class="sxs-lookup"><span data-stu-id="2718a-106">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>](itemids-nonemptyarrayofitemidstype.md)
  
```XML
<ItemIds>
   <ItemId/>
</ItemIds>
```

 <span data-ttu-id="2718a-107">**NonEmptyArrayOfItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="2718a-107">**NonEmptyArrayOfItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2718a-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="2718a-108">Attributes and elements</span></span>

<span data-ttu-id="2718a-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2718a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2718a-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="2718a-110">Attributes</span></span>

<span data-ttu-id="2718a-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2718a-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2718a-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2718a-112">Child elements</span></span>

|<span data-ttu-id="2718a-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2718a-113">**Element**</span></span>|<span data-ttu-id="2718a-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2718a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2718a-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="2718a-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="2718a-116">Contém o identificador e alterar a chave exclusiva de um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2718a-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2718a-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2718a-117">Parent elements</span></span>

|<span data-ttu-id="2718a-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2718a-118">**Element**</span></span>|<span data-ttu-id="2718a-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2718a-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2718a-120">ExportItems</span><span class="sxs-lookup"><span data-stu-id="2718a-120">ExportItems</span></span>](exportitems.md) <br/> |<span data-ttu-id="2718a-121">Representa uma solicitação para exportar itens de uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2718a-121">Represents a request to export items from a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2718a-122">Text value</span><span class="sxs-lookup"><span data-stu-id="2718a-122">Text value</span></span>

<span data-ttu-id="2718a-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2718a-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2718a-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="2718a-124">Remarks</span></span>

<span data-ttu-id="2718a-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="2718a-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2718a-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="2718a-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2718a-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="2718a-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2718a-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2718a-128">Schema Name</span></span>  <br/> |<span data-ttu-id="2718a-129">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="2718a-129">Message schema</span></span>  <br/> |
|<span data-ttu-id="2718a-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2718a-130">Validation File</span></span>  <br/> |<span data-ttu-id="2718a-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2718a-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2718a-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="2718a-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="2718a-133">False</span><span class="sxs-lookup"><span data-stu-id="2718a-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2718a-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="2718a-134">See also</span></span>



[<span data-ttu-id="2718a-135">Operação ExportItems</span><span class="sxs-lookup"><span data-stu-id="2718a-135">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="2718a-136">Operação UploadItems</span><span class="sxs-lookup"><span data-stu-id="2718a-136">UploadItems operation</span></span>](uploaditems-operation.md)

