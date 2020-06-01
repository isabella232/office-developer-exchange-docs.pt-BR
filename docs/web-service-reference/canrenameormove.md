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
ms.openlocfilehash: eb6aaeb8b0edcab5b67212c426a44daf32a0cf73
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463360"
---
# <a name="canrenameormove"></a><span data-ttu-id="fa707-103">CanRenameOrMove</span><span class="sxs-lookup"><span data-stu-id="fa707-103">CanRenameOrMove</span></span>

<span data-ttu-id="fa707-104">O elemento **CanRenameOrMove** indica se uma pasta gerenciada pode ser renomeada ou movida pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="fa707-104">The **CanRenameOrMove** element indicates whether a managed folder can be renamed or moved by the customer.</span></span> 
  
```xml
<CanRenameOrMove/>
```

 <span data-ttu-id="fa707-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="fa707-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fa707-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="fa707-106">Attributes and elements</span></span>

<span data-ttu-id="fa707-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="fa707-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fa707-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="fa707-108">Attributes</span></span>

<span data-ttu-id="fa707-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fa707-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fa707-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="fa707-110">Child elements</span></span>

<span data-ttu-id="fa707-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fa707-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fa707-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="fa707-112">Parent elements</span></span>

|<span data-ttu-id="fa707-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fa707-113">**Element**</span></span>|<span data-ttu-id="fa707-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fa707-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fa707-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="fa707-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="fa707-116">Contém informações sobre uma pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="fa707-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fa707-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="fa707-117">Text value</span></span>

<span data-ttu-id="fa707-118">O valor de texto representa um valor booliano.</span><span class="sxs-lookup"><span data-stu-id="fa707-118">The text value represents a Boolean value.</span></span> <span data-ttu-id="fa707-119">Um valor **true** indica que a pasta pode ser renomeada ou movida; um valor **false** indica que a pasta não pode ser renomeada ou movida.</span><span class="sxs-lookup"><span data-stu-id="fa707-119">A value of **true** indicates that the folder can be renamed or moved; a value of **false** indicates that the folder cannot be renamed or moved.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="fa707-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="fa707-120">Remarks</span></span>

<span data-ttu-id="fa707-121">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="fa707-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fa707-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="fa707-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fa707-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="fa707-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fa707-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="fa707-124">Schema name</span></span>  <br/> |<span data-ttu-id="fa707-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="fa707-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="fa707-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="fa707-126">Validation file</span></span>  <br/> |<span data-ttu-id="fa707-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="fa707-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fa707-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="fa707-128">Can be empty</span></span>  <br/> |<span data-ttu-id="fa707-129">False</span><span class="sxs-lookup"><span data-stu-id="fa707-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fa707-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="fa707-130">See also</span></span>



- [<span data-ttu-id="fa707-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="fa707-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

