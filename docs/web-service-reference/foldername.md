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
description: O elemento FolderName identifica uma única pasta personalizada gerenciada para adicionar uma caixa de correio.
ms.openlocfilehash: 56a7a7d256624c5103c88a333222807519d21501
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752339"
---
# <a name="foldername"></a><span data-ttu-id="eb7ee-103">FolderName</span><span class="sxs-lookup"><span data-stu-id="eb7ee-103">FolderName</span></span>

<span data-ttu-id="eb7ee-104">O elemento **FolderName** identifica uma única pasta personalizada gerenciada para adicionar uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="eb7ee-104">The **FolderName** element identifies a single managed custom folder to add to a mailbox.</span></span> 
  
[<span data-ttu-id="eb7ee-105">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="eb7ee-105">CreateManagedFolder</span></span>](createmanagedfolder.md)
  
[<span data-ttu-id="eb7ee-106">Nomes de pastas</span><span class="sxs-lookup"><span data-stu-id="eb7ee-106">FolderNames</span></span>](foldernames.md)
  
[<span data-ttu-id="eb7ee-107">FolderName</span><span class="sxs-lookup"><span data-stu-id="eb7ee-107">FolderName</span></span>](foldername.md)
  
```xml
<FolderName>...</FolderName>
```

 <span data-ttu-id="eb7ee-108">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="eb7ee-108">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eb7ee-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="eb7ee-109">Attributes and elements</span></span>

<span data-ttu-id="eb7ee-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="eb7ee-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eb7ee-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="eb7ee-111">Attributes</span></span>

<span data-ttu-id="eb7ee-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="eb7ee-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eb7ee-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="eb7ee-113">Child elements</span></span>

<span data-ttu-id="eb7ee-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="eb7ee-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="eb7ee-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="eb7ee-115">Parent elements</span></span>

|<span data-ttu-id="eb7ee-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="eb7ee-116">**Element**</span></span>|<span data-ttu-id="eb7ee-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="eb7ee-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eb7ee-118">Nomes de pastas</span><span class="sxs-lookup"><span data-stu-id="eb7ee-118">FolderNames</span></span>](foldernames.md) <br/> |<span data-ttu-id="eb7ee-119">Contém uma matriz de nomeada pastas personalizadas gerenciadas para adicionar uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="eb7ee-119">Contains an array of named managed custom folders to add to a mailbox.</span></span>  <br/> <span data-ttu-id="eb7ee-120">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="eb7ee-120">The following is the XPath expression to this element:</span></span>  <br/>  `/CreateManagedFolder/FolderNames` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="eb7ee-121">Text value</span><span class="sxs-lookup"><span data-stu-id="eb7ee-121">Text value</span></span>

<span data-ttu-id="eb7ee-122">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="eb7ee-122">A text value is required.</span></span> <span data-ttu-id="eb7ee-123">O valor de texto representa um nome de pasta.</span><span class="sxs-lookup"><span data-stu-id="eb7ee-123">The text value represents a folder name.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="eb7ee-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="eb7ee-124">Remarks</span></span>

<span data-ttu-id="eb7ee-125">Embora você possa usar os serviços Web do Exchange para adicionar pastas personalizadas gerenciadas a uma caixa de correio, você não pode usar a mesma tecnologia para acessar a lista de disponíveis pastas personalizadas gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="eb7ee-125">Although you can use Exchange Web Services to add managed custom folders to a mailbox, you cannot use the same technology to access the list of available managed custom folders.</span></span> <span data-ttu-id="eb7ee-126">Você pode obter uma lista de pastas personalizadas gerenciadas usando um comando do Shell de gerenciamento do Exchange ou por meio de uma API que interage com o serviço de diretório do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="eb7ee-126">You can obtain a list of managed custom folders by using an Exchange Management Shell command or by using an API that interfaces with the Active Directory directory service.</span></span> <span data-ttu-id="eb7ee-127">O nome da pasta é o nome do objeto do Active Directory correspondente.</span><span class="sxs-lookup"><span data-stu-id="eb7ee-127">The folder name is the name of the corresponding Active Directory object.</span></span>
  
<span data-ttu-id="eb7ee-128">Você pode usar a [operação FindFolder](findfolder-operation.md) para localizar pastas personalizadas gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="eb7ee-128">You can use the [FindFolder operation](findfolder-operation.md) to find managed custom folders.</span></span> <span data-ttu-id="eb7ee-129">Use a [operação DeleteFolder](deletefolder-operation.md) para excluir o pastas personalizadas gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="eb7ee-129">Use the [DeleteFolder operation](deletefolder-operation.md) to delete managed custom folders.</span></span> 
  
<span data-ttu-id="eb7ee-130">É importante observar que o **nome da pasta** é o nome de uma pasta de personalizada gerenciada existente na organização.</span><span class="sxs-lookup"><span data-stu-id="eb7ee-130">It is important to note that **FolderName** is the name of an existing managed custom folder in the organization.</span></span> <span data-ttu-id="eb7ee-131">Uma tentativa de adicionar uma pasta que não esteja na organização resultará em uma resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="eb7ee-131">An attempt to add a folder that is not in the organization will result in an error response.</span></span> 
  
<span data-ttu-id="eb7ee-132">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="eb7ee-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eb7ee-133">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="eb7ee-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eb7ee-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="eb7ee-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="eb7ee-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="eb7ee-135">Schema Name</span></span>  <br/> |<span data-ttu-id="eb7ee-136">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="eb7ee-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="eb7ee-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="eb7ee-137">Validation File</span></span>  <br/> |<span data-ttu-id="eb7ee-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="eb7ee-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="eb7ee-139">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="eb7ee-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="eb7ee-140">False</span><span class="sxs-lookup"><span data-stu-id="eb7ee-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eb7ee-141">Ver também</span><span class="sxs-lookup"><span data-stu-id="eb7ee-141">See also</span></span>



[<span data-ttu-id="eb7ee-142">Operação FindFolder</span><span class="sxs-lookup"><span data-stu-id="eb7ee-142">FindFolder operation</span></span>](findfolder-operation.md)


[<span data-ttu-id="eb7ee-143">Localizando pastas</span><span class="sxs-lookup"><span data-stu-id="eb7ee-143">Finding Folders</span></span>](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[<span data-ttu-id="eb7ee-144">Adicionando pastas gerenciadas</span><span class="sxs-lookup"><span data-stu-id="eb7ee-144">Adding Managed Folders</span></span>](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

