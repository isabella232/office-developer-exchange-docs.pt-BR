---
title: FolderName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderName
api_type:
- schema
ms.assetid: c5a2cd55-ac47-43bf-94b5-3ab3a4c28a62
description: O elemento FolderName identifica uma única pasta personalizada gerenciada para adicionar a uma caixa de correio.
ms.openlocfilehash: 1bb63e50c06e81337d1142a6624213fb2db12457
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461349"
---
# <a name="foldername"></a><span data-ttu-id="afabb-103">FolderName</span><span class="sxs-lookup"><span data-stu-id="afabb-103">FolderName</span></span>

<span data-ttu-id="afabb-104">O elemento **foldername** identifica uma única pasta personalizada gerenciada para adicionar a uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="afabb-104">The **FolderName** element identifies a single managed custom folder to add to a mailbox.</span></span> 
  
[<span data-ttu-id="afabb-105">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="afabb-105">CreateManagedFolder</span></span>](createmanagedfolder.md)
  
[<span data-ttu-id="afabb-106">FolderNames</span><span class="sxs-lookup"><span data-stu-id="afabb-106">FolderNames</span></span>](foldernames.md)
  
[<span data-ttu-id="afabb-107">FolderName</span><span class="sxs-lookup"><span data-stu-id="afabb-107">FolderName</span></span>](foldername.md)
  
```xml
<FolderName>...</FolderName>
```

 <span data-ttu-id="afabb-108">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="afabb-108">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="afabb-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="afabb-109">Attributes and elements</span></span>

<span data-ttu-id="afabb-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="afabb-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="afabb-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="afabb-111">Attributes</span></span>

<span data-ttu-id="afabb-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="afabb-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="afabb-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="afabb-113">Child elements</span></span>

<span data-ttu-id="afabb-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="afabb-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="afabb-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="afabb-115">Parent elements</span></span>

|<span data-ttu-id="afabb-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="afabb-116">**Element**</span></span>|<span data-ttu-id="afabb-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="afabb-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="afabb-118">FolderNames</span><span class="sxs-lookup"><span data-stu-id="afabb-118">FolderNames</span></span>](foldernames.md) <br/> |<span data-ttu-id="afabb-119">Contém uma matriz de pastas personalizadas gerenciadas e nomeadas para adicionar a uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="afabb-119">Contains an array of named managed custom folders to add to a mailbox.</span></span>  <br/> <span data-ttu-id="afabb-120">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="afabb-120">The following is the XPath expression to this element:</span></span>  <br/>  `/CreateManagedFolder/FolderNames` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="afabb-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="afabb-121">Text value</span></span>

<span data-ttu-id="afabb-122">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="afabb-122">A text value is required.</span></span> <span data-ttu-id="afabb-123">O valor de texto representa um nome de pasta.</span><span class="sxs-lookup"><span data-stu-id="afabb-123">The text value represents a folder name.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="afabb-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="afabb-124">Remarks</span></span>

<span data-ttu-id="afabb-125">Embora você possa usar os serviços Web do Exchange para adicionar pastas personalizadas gerenciadas a uma caixa de correio, não é possível usar a mesma tecnologia para acessar a lista de pastas personalizadas gerenciadas disponíveis.</span><span class="sxs-lookup"><span data-stu-id="afabb-125">Although you can use Exchange Web Services to add managed custom folders to a mailbox, you cannot use the same technology to access the list of available managed custom folders.</span></span> <span data-ttu-id="afabb-126">Você pode obter uma lista de pastas personalizadas gerenciadas usando um comando do Shell de gerenciamento do Exchange ou usando uma API que faz interface com o serviço de diretório do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="afabb-126">You can obtain a list of managed custom folders by using an Exchange Management Shell command or by using an API that interfaces with the Active Directory directory service.</span></span> <span data-ttu-id="afabb-127">O nome da pasta é o nome do objeto do Active Directory correspondente.</span><span class="sxs-lookup"><span data-stu-id="afabb-127">The folder name is the name of the corresponding Active Directory object.</span></span>
  
<span data-ttu-id="afabb-128">Você pode usar a [operação FindFolder](findfolder-operation.md) para localizar pastas personalizadas gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="afabb-128">You can use the [FindFolder operation](findfolder-operation.md) to find managed custom folders.</span></span> <span data-ttu-id="afabb-129">Use a [operação DeleteFolder](deletefolder-operation.md) para excluir pastas personalizadas gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="afabb-129">Use the [DeleteFolder operation](deletefolder-operation.md) to delete managed custom folders.</span></span> 
  
<span data-ttu-id="afabb-130">É importante observar que **foldername** é o nome de uma pasta personalizada gerenciada existente na organização.</span><span class="sxs-lookup"><span data-stu-id="afabb-130">It is important to note that **FolderName** is the name of an existing managed custom folder in the organization.</span></span> <span data-ttu-id="afabb-131">Uma tentativa de adicionar uma pasta que não esteja na organização resultará em uma resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="afabb-131">An attempt to add a folder that is not in the organization will result in an error response.</span></span> 
  
<span data-ttu-id="afabb-132">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="afabb-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="afabb-133">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="afabb-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="afabb-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="afabb-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="afabb-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="afabb-135">Schema Name</span></span>  <br/> |<span data-ttu-id="afabb-136">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="afabb-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="afabb-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="afabb-137">Validation File</span></span>  <br/> |<span data-ttu-id="afabb-138">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="afabb-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="afabb-139">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="afabb-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="afabb-140">False</span><span class="sxs-lookup"><span data-stu-id="afabb-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="afabb-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="afabb-141">See also</span></span>



[<span data-ttu-id="afabb-142">Operação FindFolder</span><span class="sxs-lookup"><span data-stu-id="afabb-142">FindFolder operation</span></span>](findfolder-operation.md)


[<span data-ttu-id="afabb-143">Localizando pastas</span><span class="sxs-lookup"><span data-stu-id="afabb-143">Finding Folders</span></span>](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[<span data-ttu-id="afabb-144">Adicionando pastas gerenciadas</span><span class="sxs-lookup"><span data-stu-id="afabb-144">Adding Managed Folders</span></span>](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

