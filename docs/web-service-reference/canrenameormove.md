---
title: CanRenameOrMove
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CanRenameOrMove
api_type:
- schema
ms.assetid: fe0cdb04-5f2b-4f1d-9d12-7ace0883cd86
description: O elemento CanRenameOrMove indica se uma pasta gerenciada pode ser renomeada ou movida pelo cliente.
ms.openlocfilehash: 0303499f5cd54d4a52222e43c2c5f0b389fbcf53
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751381"
---
# <a name="canrenameormove"></a><span data-ttu-id="e08fc-103">CanRenameOrMove</span><span class="sxs-lookup"><span data-stu-id="e08fc-103">CanRenameOrMove</span></span>

<span data-ttu-id="e08fc-104">O elemento **CanRenameOrMove** indica se uma pasta gerenciada pode ser renomeada ou movida pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e08fc-104">The **CanRenameOrMove** element indicates whether a managed folder can be renamed or moved by the customer.</span></span> 
  
```xml
<CanRenameOrMove/>
```

 <span data-ttu-id="e08fc-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="e08fc-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e08fc-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e08fc-106">Attributes and elements</span></span>

<span data-ttu-id="e08fc-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e08fc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e08fc-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e08fc-108">Attributes</span></span>

<span data-ttu-id="e08fc-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e08fc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e08fc-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e08fc-110">Child elements</span></span>

<span data-ttu-id="e08fc-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e08fc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e08fc-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e08fc-112">Parent elements</span></span>

|<span data-ttu-id="e08fc-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e08fc-113">**Element**</span></span>|<span data-ttu-id="e08fc-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e08fc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e08fc-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="e08fc-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="e08fc-116">Contém informações sobre uma pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="e08fc-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e08fc-117">Text value</span><span class="sxs-lookup"><span data-stu-id="e08fc-117">Text value</span></span>

<span data-ttu-id="e08fc-118">O valor de texto representa um valor booleano.</span><span class="sxs-lookup"><span data-stu-id="e08fc-118">The text value represents a Boolean value.</span></span> <span data-ttu-id="e08fc-119">Um valor **true** indica que a pasta pode ser renomeada ou movida; um valor **false** indica que a pasta não pode ser renomeada ou movida.</span><span class="sxs-lookup"><span data-stu-id="e08fc-119">A value of **true** indicates that the folder can be renamed or moved; a value of **false** indicates that the folder cannot be renamed or moved.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e08fc-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="e08fc-120">Remarks</span></span>

<span data-ttu-id="e08fc-121">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="e08fc-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e08fc-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e08fc-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e08fc-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="e08fc-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e08fc-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e08fc-124">Schema name</span></span>  <br/> |<span data-ttu-id="e08fc-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e08fc-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="e08fc-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e08fc-126">Validation file</span></span>  <br/> |<span data-ttu-id="e08fc-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e08fc-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e08fc-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="e08fc-128">Can be empty</span></span>  <br/> |<span data-ttu-id="e08fc-129">False</span><span class="sxs-lookup"><span data-stu-id="e08fc-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e08fc-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="e08fc-130">See also</span></span>



- [<span data-ttu-id="e08fc-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e08fc-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

