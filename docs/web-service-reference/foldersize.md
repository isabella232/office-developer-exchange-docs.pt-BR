---
title: FolderSize
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderSize
api_type:
- schema
ms.assetid: 27e5f0cd-e23a-4ddd-943a-9f17bf0fd87b
description: O elemento FolderSize descreve o tamanho total de todo o conteúdo de uma pasta gerenciada.
ms.openlocfilehash: 314c75e6ab824caed4c6a1c6f5b62a43f86ba939
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752347"
---
# <a name="foldersize"></a><span data-ttu-id="5d810-103">FolderSize</span><span class="sxs-lookup"><span data-stu-id="5d810-103">FolderSize</span></span>

<span data-ttu-id="5d810-104">O elemento **FolderSize** descreve o tamanho total de todo o conteúdo de uma pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="5d810-104">The **FolderSize** element describes the total size of all the contents of a managed folder.</span></span> 
  
```xml
<FolderSize/>
```

 <span data-ttu-id="5d810-105">**int**</span><span class="sxs-lookup"><span data-stu-id="5d810-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5d810-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="5d810-106">Attributes and elements</span></span>

<span data-ttu-id="5d810-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5d810-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5d810-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5d810-108">Attributes</span></span>

<span data-ttu-id="5d810-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5d810-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5d810-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5d810-110">Child elements</span></span>

<span data-ttu-id="5d810-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5d810-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5d810-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5d810-112">Parent elements</span></span>

|<span data-ttu-id="5d810-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5d810-113">**Element**</span></span>|<span data-ttu-id="5d810-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5d810-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5d810-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="5d810-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="5d810-116">Contém informações sobre uma pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="5d810-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5d810-117">Text value</span><span class="sxs-lookup"><span data-stu-id="5d810-117">Text value</span></span>

<span data-ttu-id="5d810-118">O valor de texto representa o tamanho total da pasta em megabytes.</span><span class="sxs-lookup"><span data-stu-id="5d810-118">The text value represents the total size of the folder in megabytes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5d810-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="5d810-119">Remarks</span></span>

<span data-ttu-id="5d810-120">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="5d810-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5d810-121">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="5d810-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5d810-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="5d810-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5d810-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5d810-123">Schema name</span></span>  <br/> |<span data-ttu-id="5d810-124">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="5d810-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="5d810-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5d810-125">Validation file</span></span>  <br/> |<span data-ttu-id="5d810-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5d810-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5d810-127">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="5d810-127">Can be empty</span></span>  <br/> |<span data-ttu-id="5d810-128">False</span><span class="sxs-lookup"><span data-stu-id="5d810-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5d810-129">Ver também</span><span class="sxs-lookup"><span data-stu-id="5d810-129">See also</span></span>



[<span data-ttu-id="5d810-130">Operação CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="5d810-130">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)


- [<span data-ttu-id="5d810-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5d810-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

