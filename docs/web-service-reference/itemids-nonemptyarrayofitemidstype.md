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
description: O elemento ItemIds contém uma matriz de identificadores de item que identificam os itens a serem exportados de uma caixa de correio.
ms.openlocfilehash: 16c2633528e2ecbc863cfdde645e0f431b4c4297
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468590"
---
# <a name="itemids-nonemptyarrayofitemidstype"></a><span data-ttu-id="a49f1-103">ItemIds (NonEmptyArrayOfItemIdsType)</span><span class="sxs-lookup"><span data-stu-id="a49f1-103">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>

<span data-ttu-id="a49f1-104">O elemento **ItemIds** contém uma matriz de identificadores de item que identificam os itens a serem exportados de uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="a49f1-104">The **ItemIds** element contains an array of item identifiers that identify the items to export from a mailbox.</span></span> 
  
[<span data-ttu-id="a49f1-105">ExportItems</span><span class="sxs-lookup"><span data-stu-id="a49f1-105">ExportItems</span></span>](exportitems.md)
  
[<span data-ttu-id="a49f1-106">ItemIds (NonEmptyArrayOfItemIdsType)</span><span class="sxs-lookup"><span data-stu-id="a49f1-106">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>](itemids-nonemptyarrayofitemidstype.md)
  
```XML
<ItemIds>
   <ItemId/>
</ItemIds>
```

 <span data-ttu-id="a49f1-107">**NonEmptyArrayOfItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="a49f1-107">**NonEmptyArrayOfItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a49f1-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a49f1-108">Attributes and elements</span></span>

<span data-ttu-id="a49f1-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a49f1-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a49f1-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="a49f1-110">Attributes</span></span>

<span data-ttu-id="a49f1-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a49f1-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a49f1-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a49f1-112">Child elements</span></span>

|<span data-ttu-id="a49f1-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a49f1-113">**Element**</span></span>|<span data-ttu-id="a49f1-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a49f1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a49f1-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="a49f1-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="a49f1-116">Contém o identificador exclusivo e a chave de alteração de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a49f1-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a49f1-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a49f1-117">Parent elements</span></span>

|<span data-ttu-id="a49f1-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a49f1-118">**Element**</span></span>|<span data-ttu-id="a49f1-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a49f1-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a49f1-120">ExportItems</span><span class="sxs-lookup"><span data-stu-id="a49f1-120">ExportItems</span></span>](exportitems.md) <br/> |<span data-ttu-id="a49f1-121">Representa uma solicitação para exportar itens de uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="a49f1-121">Represents a request to export items from a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a49f1-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="a49f1-122">Text value</span></span>

<span data-ttu-id="a49f1-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a49f1-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a49f1-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="a49f1-124">Remarks</span></span>

<span data-ttu-id="a49f1-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a49f1-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a49f1-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="a49f1-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a49f1-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="a49f1-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a49f1-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a49f1-128">Schema Name</span></span>  <br/> |<span data-ttu-id="a49f1-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="a49f1-129">Message schema</span></span>  <br/> |
|<span data-ttu-id="a49f1-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a49f1-130">Validation File</span></span>  <br/> |<span data-ttu-id="a49f1-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a49f1-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a49f1-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a49f1-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="a49f1-133">False</span><span class="sxs-lookup"><span data-stu-id="a49f1-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a49f1-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="a49f1-134">See also</span></span>



[<span data-ttu-id="a49f1-135">Operação ExportItems</span><span class="sxs-lookup"><span data-stu-id="a49f1-135">ExportItems operation</span></span>](exportitems-operation.md)
  
[<span data-ttu-id="a49f1-136">Operação UploadItems</span><span class="sxs-lookup"><span data-stu-id="a49f1-136">UploadItems operation</span></span>](uploaditems-operation.md)

