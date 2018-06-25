---
title: Dados (base64Binary)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Data
api_type:
- schema
ms.assetid: 26d8c2d0-bed2-4aed-b381-20e2ace6892f
description: O elemento de dados contém os dados de um item para carregar em uma caixa de correio ou de um único item exportado.
ms.openlocfilehash: 9560273e31a64edb2254489961733dfe7360ad01
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751670"
---
# <a name="data-base64binary"></a><span data-ttu-id="902f5-103">Dados (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="902f5-103">Data (base64Binary)</span></span>

<span data-ttu-id="902f5-104">O elemento de **dados** contém os dados de um item para carregar em uma caixa de correio ou de um único item exportado.</span><span class="sxs-lookup"><span data-stu-id="902f5-104">The **Data** element contains the data of a single exported item or an item to upload into a mailbox.</span></span> 
  
```XML
<Data/>
```

<span data-ttu-id="902f5-105">**base64Binary**</span><span class="sxs-lookup"><span data-stu-id="902f5-105">**xs:base64Binary**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="902f5-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="902f5-106">Attributes and elements</span></span>

<span data-ttu-id="902f5-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="902f5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="902f5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="902f5-108">Attributes</span></span>

<span data-ttu-id="902f5-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="902f5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="902f5-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="902f5-110">Child elements</span></span>

<span data-ttu-id="902f5-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="902f5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="902f5-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="902f5-112">Parent elements</span></span>

|<span data-ttu-id="902f5-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="902f5-113">**Element**</span></span>|<span data-ttu-id="902f5-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="902f5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="902f5-115">ExportItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="902f5-115">ExportItemsResponseMessage</span></span>](exportitemsresponsemessage.md) <br/> |<span data-ttu-id="902f5-116">Contém o status e os resultados de uma solicitação para exportar um item de caixa de correio única.</span><span class="sxs-lookup"><span data-stu-id="902f5-116">Contains the status and results of a request to export a single mailbox item.</span></span>  <br/> |
|[<span data-ttu-id="902f5-117">Item (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="902f5-117">Item (UploadItemType)</span></span>](item-uploaditemtype.md) <br/> |<span data-ttu-id="902f5-118">Representa um único item para carregar em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="902f5-118">Represents a single item to upload into a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="902f5-119">Text value</span><span class="sxs-lookup"><span data-stu-id="902f5-119">Text value</span></span>

<span data-ttu-id="902f5-120">O elemento de **dados** contém os nomes de propriedade e valores para um item que será carregado em uma caixa de correio ou de um item exportado.</span><span class="sxs-lookup"><span data-stu-id="902f5-120">The **Data** element contains the property names and values for an exported item or an item that will be uploaded into a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="902f5-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="902f5-121">Remarks</span></span>

<span data-ttu-id="902f5-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="902f5-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="902f5-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="902f5-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="902f5-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="902f5-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="902f5-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="902f5-125">Schema Name</span></span>  <br/> |<span data-ttu-id="902f5-126">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="902f5-126">Message schema</span></span>  <br/> |
|<span data-ttu-id="902f5-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="902f5-127">Validation File</span></span>  <br/> |<span data-ttu-id="902f5-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="902f5-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="902f5-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="902f5-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="902f5-130">False</span><span class="sxs-lookup"><span data-stu-id="902f5-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="902f5-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="902f5-131">See also</span></span>

- [<span data-ttu-id="902f5-132">Operação ExportItems</span><span class="sxs-lookup"><span data-stu-id="902f5-132">ExportItems operation</span></span>](exportitems-operation.md)
- [<span data-ttu-id="902f5-133">Operação UploadItems</span><span class="sxs-lookup"><span data-stu-id="902f5-133">UploadItems operation</span></span>](uploaditems-operation.md)

