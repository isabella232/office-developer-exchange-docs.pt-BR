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
description: O elemento IsManagedFoldersRoot indica se a pasta gerenciada é a raiz para todas as pastas gerenciadas.
ms.openlocfilehash: 3484a3fef56545a9a8d56af65f56f75205918ec7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824044"
---
# <a name="ismanagedfoldersroot"></a><span data-ttu-id="4152c-103">IsManagedFoldersRoot</span><span class="sxs-lookup"><span data-stu-id="4152c-103">IsManagedFoldersRoot</span></span>

<span data-ttu-id="4152c-104">O elemento **IsManagedFoldersRoot** indica se a pasta gerenciada é a raiz para todas as pastas gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="4152c-104">The **IsManagedFoldersRoot** element indicates whether the managed folder is the root for all managed folders.</span></span> 
  
```xml
<IsManagedFoldersRoot/>
```

 <span data-ttu-id="4152c-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="4152c-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4152c-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="4152c-106">Attributes and elements</span></span>

<span data-ttu-id="4152c-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4152c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4152c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4152c-108">Attributes</span></span>

<span data-ttu-id="4152c-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4152c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4152c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4152c-110">Child elements</span></span>

<span data-ttu-id="4152c-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4152c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4152c-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4152c-112">Parent elements</span></span>

|<span data-ttu-id="4152c-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4152c-113">**Element**</span></span>|<span data-ttu-id="4152c-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4152c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4152c-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="4152c-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="4152c-116">Contém informações sobre uma pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="4152c-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4152c-117">Text value</span><span class="sxs-lookup"><span data-stu-id="4152c-117">Text value</span></span>

<span data-ttu-id="4152c-118">Um valor de texto que representa um valor booleano é necessário se este elemento está presente.</span><span class="sxs-lookup"><span data-stu-id="4152c-118">A text value that represents a Boolean value is required if this element is present.</span></span> <span data-ttu-id="4152c-119">Um valor **true** indica que a pasta é a pasta raiz da pasta gerenciada; um valor **false** indica que a pasta não é a pasta raiz da pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="4152c-119">A value of **true** indicates that the folder is the root folder of the managed folder; a value of **false** indicates that the folder is not the root folder of the managed folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="4152c-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="4152c-120">Remarks</span></span>

<span data-ttu-id="4152c-121">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="4152c-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4152c-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="4152c-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4152c-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="4152c-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4152c-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4152c-124">Schema name</span></span>  <br/> |<span data-ttu-id="4152c-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="4152c-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="4152c-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4152c-126">Validation file</span></span>  <br/> |<span data-ttu-id="4152c-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4152c-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4152c-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="4152c-128">Can be empty</span></span>  <br/> |<span data-ttu-id="4152c-129">False</span><span class="sxs-lookup"><span data-stu-id="4152c-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4152c-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="4152c-130">See also</span></span>



- [<span data-ttu-id="4152c-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4152c-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

