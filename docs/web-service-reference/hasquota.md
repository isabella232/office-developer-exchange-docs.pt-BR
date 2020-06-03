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
ms.openlocfilehash: 6e32aa4c69943774be928339936cca5016c58d85
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462749"
---
# <a name="hasquota"></a><span data-ttu-id="c6e6e-103">HasQuota</span><span class="sxs-lookup"><span data-stu-id="c6e6e-103">HasQuota</span></span>

<span data-ttu-id="c6e6e-104">O elemento **HasQuota** indica se a pasta gerenciada tem uma cota.</span><span class="sxs-lookup"><span data-stu-id="c6e6e-104">The **HasQuota** element indicates whether the managed folder has a quota.</span></span> 
  
```xml
<HasQuota/>
```

 <span data-ttu-id="c6e6e-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="c6e6e-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c6e6e-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c6e6e-106">Attributes and elements</span></span>

<span data-ttu-id="c6e6e-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c6e6e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c6e6e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c6e6e-108">Attributes</span></span>

<span data-ttu-id="c6e6e-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c6e6e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c6e6e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c6e6e-110">Child elements</span></span>

<span data-ttu-id="c6e6e-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c6e6e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c6e6e-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c6e6e-112">Parent elements</span></span>

|<span data-ttu-id="c6e6e-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c6e6e-113">**Element**</span></span>|<span data-ttu-id="c6e6e-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c6e6e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c6e6e-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="c6e6e-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="c6e6e-116">Contém informações sobre uma pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="c6e6e-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c6e6e-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="c6e6e-117">Text value</span></span>

<span data-ttu-id="c6e6e-118">O valor de texto representa um valor booliano.</span><span class="sxs-lookup"><span data-stu-id="c6e6e-118">The text value represents a Boolean value.</span></span> <span data-ttu-id="c6e6e-119">Um valor **true** indica que a pasta tem uma cota; um valor **false** indica que a pasta não tem uma cota.</span><span class="sxs-lookup"><span data-stu-id="c6e6e-119">A value of **true** indicates that the folder has a quota; a value of **false** indicates that the folder does not have a quota.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c6e6e-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="c6e6e-120">Remarks</span></span>

<span data-ttu-id="c6e6e-121">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="c6e6e-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c6e6e-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c6e6e-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c6e6e-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="c6e6e-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c6e6e-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c6e6e-124">Schema name</span></span>  <br/> |<span data-ttu-id="c6e6e-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c6e6e-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="c6e6e-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c6e6e-126">Validation file</span></span>  <br/> |<span data-ttu-id="c6e6e-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c6e6e-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c6e6e-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="c6e6e-128">Can be empty</span></span>  <br/> |<span data-ttu-id="c6e6e-129">False</span><span class="sxs-lookup"><span data-stu-id="c6e6e-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c6e6e-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="c6e6e-130">See also</span></span>



- [<span data-ttu-id="c6e6e-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c6e6e-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

