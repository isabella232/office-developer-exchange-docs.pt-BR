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
description: O elemento de dados contém os dados de um único item exportado ou um item a ser carregado em uma caixa de correio.
ms.openlocfilehash: 43ee16ca7caf634756ca00a88715d9834adad92b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526967"
---
# <a name="data-base64binary"></a><span data-ttu-id="76d80-103">Dados (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="76d80-103">Data (base64Binary)</span></span>

<span data-ttu-id="76d80-104">O elemento de **dados** contém os dados de um único item exportado ou um item a ser carregado em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="76d80-104">The **Data** element contains the data of a single exported item or an item to upload into a mailbox.</span></span> 
  
```XML
<Data/>
```

<span data-ttu-id="76d80-105">**xs: base64Binary**</span><span class="sxs-lookup"><span data-stu-id="76d80-105">**xs:base64Binary**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="76d80-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="76d80-106">Attributes and elements</span></span>

<span data-ttu-id="76d80-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="76d80-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="76d80-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="76d80-108">Attributes</span></span>

<span data-ttu-id="76d80-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="76d80-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="76d80-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="76d80-110">Child elements</span></span>

<span data-ttu-id="76d80-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="76d80-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="76d80-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="76d80-112">Parent elements</span></span>

|<span data-ttu-id="76d80-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="76d80-113">**Element**</span></span>|<span data-ttu-id="76d80-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="76d80-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="76d80-115">ExportItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76d80-115">ExportItemsResponseMessage</span></span>](exportitemsresponsemessage.md) <br/> |<span data-ttu-id="76d80-116">Contém o status e os resultados de uma solicitação para exportar um único item de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="76d80-116">Contains the status and results of a request to export a single mailbox item.</span></span>  <br/> |
|[<span data-ttu-id="76d80-117">Item (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="76d80-117">Item (UploadItemType)</span></span>](item-uploaditemtype.md) <br/> |<span data-ttu-id="76d80-118">Representa um único item a ser carregado em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="76d80-118">Represents a single item to upload into a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="76d80-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="76d80-119">Text value</span></span>

<span data-ttu-id="76d80-120">O elemento de **dados** contém os nomes e valores de propriedade de um item exportado ou um item que será carregado em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="76d80-120">The **Data** element contains the property names and values for an exported item or an item that will be uploaded into a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="76d80-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="76d80-121">Remarks</span></span>

<span data-ttu-id="76d80-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="76d80-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="76d80-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="76d80-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="76d80-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="76d80-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="76d80-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="76d80-125">Schema Name</span></span>  <br/> |<span data-ttu-id="76d80-126">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="76d80-126">Message schema</span></span>  <br/> |
|<span data-ttu-id="76d80-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="76d80-127">Validation File</span></span>  <br/> |<span data-ttu-id="76d80-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="76d80-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="76d80-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="76d80-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="76d80-130">False</span><span class="sxs-lookup"><span data-stu-id="76d80-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="76d80-131">Confira também</span><span class="sxs-lookup"><span data-stu-id="76d80-131">See also</span></span>

- [<span data-ttu-id="76d80-132">Operação ExportItems</span><span class="sxs-lookup"><span data-stu-id="76d80-132">ExportItems operation</span></span>](exportitems-operation.md)
- [<span data-ttu-id="76d80-133">Operação UploadItems</span><span class="sxs-lookup"><span data-stu-id="76d80-133">UploadItems operation</span></span>](uploaditems-operation.md)

