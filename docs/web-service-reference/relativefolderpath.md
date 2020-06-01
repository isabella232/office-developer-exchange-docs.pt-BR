---
title: RelativeFolderPath
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 54e3ba52-08a6-4d48-8a44-6fd5fdbffb25
description: O elemento RelativeFolderPath contém uma matriz de pastas que indica o caminho de pasta relativo do caminho da pasta a ser criado.
ms.openlocfilehash: 8a0fc0020943afdbe6cd4c79d51d61337f8dd329
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457155"
---
# <a name="relativefolderpath"></a><span data-ttu-id="d7867-103">RelativeFolderPath</span><span class="sxs-lookup"><span data-stu-id="d7867-103">RelativeFolderPath</span></span>

<span data-ttu-id="d7867-104">O elemento **RelativeFolderPath** contém uma matriz de pastas que indica o caminho de pasta relativo do caminho da pasta a ser criado.</span><span class="sxs-lookup"><span data-stu-id="d7867-104">The **RelativeFolderPath** element contains an array of folders that indicate the relative folder path of the folder path to be created.</span></span> 
  
```XML
<RelativeFolderPath>
   <Folder/>
   <CalendarFolder/>
   <ContactsFolder/>
   <SearchFolder/>
   <TasksFolder/>
</RelativeFolderPath>
```

 <span data-ttu-id="d7867-105">**NonEmptyArrayOfFoldersType**</span><span class="sxs-lookup"><span data-stu-id="d7867-105">**NonEmptyArrayOfFoldersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d7867-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d7867-106">Attributes and elements</span></span>

<span data-ttu-id="d7867-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d7867-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d7867-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d7867-108">Attributes</span></span>

<span data-ttu-id="d7867-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d7867-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d7867-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d7867-110">Child elements</span></span>

<span data-ttu-id="d7867-111">[Pasta](folder.md)  |  [CalendarFolder](calendarfolder.md)  |  [ContactsFolder](contactsfolder.md)  |  [SearchFolder](searchfolder.md)  |  [TasksFolder](tasksfolder.md)</span><span class="sxs-lookup"><span data-stu-id="d7867-111">[Folder](folder.md) | [CalendarFolder](calendarfolder.md) | [ContactsFolder](contactsfolder.md) | [SearchFolder](searchfolder.md) | [TasksFolder](tasksfolder.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d7867-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d7867-112">Parent elements</span></span>

[<span data-ttu-id="d7867-113">Createfolderpath</span><span class="sxs-lookup"><span data-stu-id="d7867-113">CreateFolderPath</span></span>](createfolderpath.md)
  
## <a name="remarks"></a><span data-ttu-id="d7867-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="d7867-114">Remarks</span></span>

<span data-ttu-id="d7867-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d7867-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d7867-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d7867-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d7867-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d7867-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d7867-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="d7867-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d7867-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d7867-119">Schema name</span></span>  <br/> |<span data-ttu-id="d7867-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="d7867-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d7867-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d7867-121">Validation file</span></span>  <br/> |<span data-ttu-id="d7867-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d7867-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d7867-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="d7867-123">Can be empty</span></span>  <br/> ||
   

