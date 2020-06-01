---
title: IsManagedFoldersRoot
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsManagedFoldersRoot
api_type:
- schema
ms.assetid: 00823fb9-bf8b-49bb-8e1b-d698c6d4063f
description: O elemento IsManagedFoldersRoot indica se a pasta gerenciada é a raiz de todas as pastas gerenciadas.
ms.openlocfilehash: 4373dba9dce92de8e175948d889f0806e100fa6c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466021"
---
# <a name="ismanagedfoldersroot"></a><span data-ttu-id="173f0-103">IsManagedFoldersRoot</span><span class="sxs-lookup"><span data-stu-id="173f0-103">IsManagedFoldersRoot</span></span>

<span data-ttu-id="173f0-104">O elemento **IsManagedFoldersRoot** indica se a pasta gerenciada é a raiz de todas as pastas gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="173f0-104">The **IsManagedFoldersRoot** element indicates whether the managed folder is the root for all managed folders.</span></span> 
  
```xml
<IsManagedFoldersRoot/>
```

 <span data-ttu-id="173f0-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="173f0-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="173f0-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="173f0-106">Attributes and elements</span></span>

<span data-ttu-id="173f0-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="173f0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="173f0-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="173f0-108">Attributes</span></span>

<span data-ttu-id="173f0-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="173f0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="173f0-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="173f0-110">Child elements</span></span>

<span data-ttu-id="173f0-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="173f0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="173f0-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="173f0-112">Parent elements</span></span>

|<span data-ttu-id="173f0-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="173f0-113">**Element**</span></span>|<span data-ttu-id="173f0-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="173f0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="173f0-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="173f0-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="173f0-116">Contém informações sobre uma pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="173f0-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="173f0-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="173f0-117">Text value</span></span>

<span data-ttu-id="173f0-118">Um valor de texto que representa um valor booliano é necessário se esse elemento estiver presente.</span><span class="sxs-lookup"><span data-stu-id="173f0-118">A text value that represents a Boolean value is required if this element is present.</span></span> <span data-ttu-id="173f0-119">Um valor **true** indica que a pasta é a pasta raiz da pasta gerenciada; um valor **false** indica que a pasta não é a pasta raiz da pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="173f0-119">A value of **true** indicates that the folder is the root folder of the managed folder; a value of **false** indicates that the folder is not the root folder of the managed folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="173f0-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="173f0-120">Remarks</span></span>

<span data-ttu-id="173f0-121">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="173f0-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="173f0-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="173f0-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="173f0-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="173f0-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="173f0-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="173f0-124">Schema name</span></span>  <br/> |<span data-ttu-id="173f0-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="173f0-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="173f0-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="173f0-126">Validation file</span></span>  <br/> |<span data-ttu-id="173f0-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="173f0-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="173f0-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="173f0-128">Can be empty</span></span>  <br/> |<span data-ttu-id="173f0-129">False</span><span class="sxs-lookup"><span data-stu-id="173f0-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="173f0-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="173f0-130">See also</span></span>



- [<span data-ttu-id="173f0-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="173f0-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

