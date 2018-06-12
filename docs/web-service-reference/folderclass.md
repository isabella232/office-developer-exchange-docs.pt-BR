---
title: FolderClass
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderClass
api_type:
- schema
ms.assetid: 0041d135-2869-4612-89a5-d1aa86aa1093
description: O elemento FolderClass representa a classe de pasta para uma pasta.
ms.openlocfilehash: 87be00563d0375abebf32159ff38d62d03112b95
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752326"
---
# <a name="folderclass"></a><span data-ttu-id="12d75-103">FolderClass</span><span class="sxs-lookup"><span data-stu-id="12d75-103">FolderClass</span></span>

<span data-ttu-id="12d75-104">O elemento **FolderClass** representa a classe de pasta para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="12d75-104">The **FolderClass** element represents the folder class for a folder.</span></span> 
  
```xml
<FolderClass/>
```

 <span data-ttu-id="12d75-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="12d75-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="12d75-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="12d75-106">Attributes and elements</span></span>

<span data-ttu-id="12d75-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="12d75-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="12d75-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="12d75-108">Attributes</span></span>

<span data-ttu-id="12d75-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="12d75-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="12d75-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="12d75-110">Child elements</span></span>

<span data-ttu-id="12d75-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="12d75-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="12d75-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="12d75-112">Parent elements</span></span>

|<span data-ttu-id="12d75-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="12d75-113">**Element**</span></span>|<span data-ttu-id="12d75-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="12d75-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="12d75-115">Folder</span><span class="sxs-lookup"><span data-stu-id="12d75-115">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="12d75-116">Representa uma pasta em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="12d75-116">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="12d75-117">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="12d75-117">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="12d75-118">Representa uma pasta de calendário em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="12d75-118">Represents a calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="12d75-119">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="12d75-119">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="12d75-120">Representa uma pasta de contatos em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="12d75-120">Represents a contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="12d75-121">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="12d75-121">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="12d75-122">Representa uma pasta de pesquisa em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="12d75-122">Represents a search folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="12d75-123">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="12d75-123">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="12d75-124">Representa uma pasta de tarefa em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="12d75-124">Represents a task folder in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="12d75-125">Text value</span><span class="sxs-lookup"><span data-stu-id="12d75-125">Text value</span></span>

<span data-ttu-id="12d75-126">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="12d75-126">A text value is required.</span></span> <span data-ttu-id="12d75-127">Classes de pasta geralmente começar com "IPF."</span><span class="sxs-lookup"><span data-stu-id="12d75-127">Folder classes typically start with "IPF."</span></span>
  
## <a name="remarks"></a><span data-ttu-id="12d75-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="12d75-128">Remarks</span></span>

<span data-ttu-id="12d75-129">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="12d75-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="12d75-130">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="12d75-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="12d75-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="12d75-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="12d75-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="12d75-132">Schema Name</span></span>  <br/> |<span data-ttu-id="12d75-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="12d75-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="12d75-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="12d75-134">Validation File</span></span>  <br/> |<span data-ttu-id="12d75-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="12d75-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="12d75-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="12d75-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="12d75-137">False</span><span class="sxs-lookup"><span data-stu-id="12d75-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="12d75-138">Ver também</span><span class="sxs-lookup"><span data-stu-id="12d75-138">See also</span></span>



- [<span data-ttu-id="12d75-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="12d75-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

