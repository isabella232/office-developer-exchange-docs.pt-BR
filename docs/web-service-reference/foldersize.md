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
description: O elemento Folderize descreve o tamanho total de todo o conteúdo de uma pasta gerenciada.
ms.openlocfilehash: 8ed493cfb0c2cabd02d28354c115a73662992473
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461335"
---
# <a name="foldersize"></a><span data-ttu-id="85ddc-103">FolderSize</span><span class="sxs-lookup"><span data-stu-id="85ddc-103">FolderSize</span></span>

<span data-ttu-id="85ddc-104">O elemento **folderize** descreve o tamanho total de todo o conteúdo de uma pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="85ddc-104">The **FolderSize** element describes the total size of all the contents of a managed folder.</span></span> 
  
```xml
<FolderSize/>
```

 <span data-ttu-id="85ddc-105">**int**</span><span class="sxs-lookup"><span data-stu-id="85ddc-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="85ddc-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="85ddc-106">Attributes and elements</span></span>

<span data-ttu-id="85ddc-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="85ddc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="85ddc-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="85ddc-108">Attributes</span></span>

<span data-ttu-id="85ddc-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="85ddc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="85ddc-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="85ddc-110">Child elements</span></span>

<span data-ttu-id="85ddc-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="85ddc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="85ddc-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="85ddc-112">Parent elements</span></span>

|<span data-ttu-id="85ddc-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="85ddc-113">**Element**</span></span>|<span data-ttu-id="85ddc-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="85ddc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="85ddc-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="85ddc-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="85ddc-116">Contém informações sobre uma pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="85ddc-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="85ddc-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="85ddc-117">Text value</span></span>

<span data-ttu-id="85ddc-118">O valor de texto representa o tamanho total da pasta em megabytes.</span><span class="sxs-lookup"><span data-stu-id="85ddc-118">The text value represents the total size of the folder in megabytes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="85ddc-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="85ddc-119">Remarks</span></span>

<span data-ttu-id="85ddc-120">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="85ddc-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="85ddc-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="85ddc-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="85ddc-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="85ddc-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="85ddc-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="85ddc-123">Schema name</span></span>  <br/> |<span data-ttu-id="85ddc-124">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="85ddc-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="85ddc-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="85ddc-125">Validation file</span></span>  <br/> |<span data-ttu-id="85ddc-126">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="85ddc-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="85ddc-127">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="85ddc-127">Can be empty</span></span>  <br/> |<span data-ttu-id="85ddc-128">False</span><span class="sxs-lookup"><span data-stu-id="85ddc-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="85ddc-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="85ddc-129">See also</span></span>



[<span data-ttu-id="85ddc-130">Operação CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="85ddc-130">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)


- [<span data-ttu-id="85ddc-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="85ddc-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

