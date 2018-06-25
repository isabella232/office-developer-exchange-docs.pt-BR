---
title: HasQuota
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- HasQuota
api_type:
- schema
ms.assetid: b6e4fef0-92a9-415f-81ae-0c5ecb7c12ad
description: O elemento HasQuota indica se a pasta gerenciada tem uma cota.
ms.openlocfilehash: 26f14ee7c9d4de267733bca11f7884d1d391b3dd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823807"
---
# <a name="hasquota"></a><span data-ttu-id="9a685-103">HasQuota</span><span class="sxs-lookup"><span data-stu-id="9a685-103">HasQuota</span></span>

<span data-ttu-id="9a685-104">O elemento **HasQuota** indica se a pasta gerenciada tem uma cota.</span><span class="sxs-lookup"><span data-stu-id="9a685-104">The **HasQuota** element indicates whether the managed folder has a quota.</span></span> 
  
```xml
<HasQuota/>
```

 <span data-ttu-id="9a685-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="9a685-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9a685-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="9a685-106">Attributes and elements</span></span>

<span data-ttu-id="9a685-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9a685-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9a685-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9a685-108">Attributes</span></span>

<span data-ttu-id="9a685-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9a685-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9a685-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9a685-110">Child elements</span></span>

<span data-ttu-id="9a685-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9a685-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9a685-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9a685-112">Parent elements</span></span>

|<span data-ttu-id="9a685-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9a685-113">**Element**</span></span>|<span data-ttu-id="9a685-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9a685-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9a685-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="9a685-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="9a685-116">Contém informações sobre uma pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="9a685-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9a685-117">Text value</span><span class="sxs-lookup"><span data-stu-id="9a685-117">Text value</span></span>

<span data-ttu-id="9a685-118">O valor de texto representa um valor booleano.</span><span class="sxs-lookup"><span data-stu-id="9a685-118">The text value represents a Boolean value.</span></span> <span data-ttu-id="9a685-119">Um valor **true** indica que a pasta tem uma cota; um valor **false** indica que a pasta não tem uma cota.</span><span class="sxs-lookup"><span data-stu-id="9a685-119">A value of **true** indicates that the folder has a quota; a value of **false** indicates that the folder does not have a quota.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="9a685-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="9a685-120">Remarks</span></span>

<span data-ttu-id="9a685-121">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="9a685-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9a685-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="9a685-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9a685-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="9a685-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9a685-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9a685-124">Schema name</span></span>  <br/> |<span data-ttu-id="9a685-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="9a685-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="9a685-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9a685-126">Validation file</span></span>  <br/> |<span data-ttu-id="9a685-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9a685-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9a685-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="9a685-128">Can be empty</span></span>  <br/> |<span data-ttu-id="9a685-129">False</span><span class="sxs-lookup"><span data-stu-id="9a685-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9a685-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="9a685-130">See also</span></span>



- [<span data-ttu-id="9a685-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9a685-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

