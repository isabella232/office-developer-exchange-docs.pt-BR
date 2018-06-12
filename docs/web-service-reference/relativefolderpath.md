---
title: RelativeFolderPath
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 54e3ba52-08a6-4d48-8a44-6fd5fdbffb25
description: O elemento RelativeFolderPath contém uma matriz das pastas que indicam o caminho da pasta relativa do caminho da pasta a ser criado.
ms.openlocfilehash: f568d282e47a41c0aaf6d70ef383e5ef3e2b54bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825051"
---
# <a name="relativefolderpath"></a><span data-ttu-id="68f11-103">RelativeFolderPath</span><span class="sxs-lookup"><span data-stu-id="68f11-103">RelativeFolderPath</span></span>

<span data-ttu-id="68f11-104">O elemento **RelativeFolderPath** contém uma matriz das pastas que indicam o caminho da pasta relativa do caminho da pasta a ser criado.</span><span class="sxs-lookup"><span data-stu-id="68f11-104">The **RelativeFolderPath** element contains an array of folders that indicate the relative folder path of the folder path to be created.</span></span> 
  
```XML
<RelativeFolderPath>
   <Folder/>
   <CalendarFolder/>
   <ContactsFolder/>
   <SearchFolder/>
   <TasksFolder/>
</RelativeFolderPath>
```

 <span data-ttu-id="68f11-105">**NonEmptyArrayOfFoldersType**</span><span class="sxs-lookup"><span data-stu-id="68f11-105">**NonEmptyArrayOfFoldersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="68f11-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="68f11-106">Attributes and elements</span></span>

<span data-ttu-id="68f11-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="68f11-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="68f11-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="68f11-108">Attributes</span></span>

<span data-ttu-id="68f11-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="68f11-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="68f11-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="68f11-110">Child elements</span></span>

<span data-ttu-id="68f11-111">[Pasta](folder.md) | [CalendarFolder](calendarfolder.md) | [ContactsFolder](contactsfolder.md) | [SearchFolder](searchfolder.md) | [TasksFolder](tasksfolder.md)</span><span class="sxs-lookup"><span data-stu-id="68f11-111">[Folder](folder.md) | [CalendarFolder](calendarfolder.md) | [ContactsFolder](contactsfolder.md) | [SearchFolder](searchfolder.md) | [TasksFolder](tasksfolder.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="68f11-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="68f11-112">Parent elements</span></span>

[<span data-ttu-id="68f11-113">CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="68f11-113">CreateFolderPath</span></span>](createfolderpath.md)
  
## <a name="remarks"></a><span data-ttu-id="68f11-114">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="68f11-114">Remarks</span></span>

<span data-ttu-id="68f11-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="68f11-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="68f11-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="68f11-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="68f11-117">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="68f11-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="68f11-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="68f11-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="68f11-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="68f11-119">Schema name</span></span>  <br/> |<span data-ttu-id="68f11-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="68f11-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="68f11-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="68f11-121">Validation file</span></span>  <br/> |<span data-ttu-id="68f11-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="68f11-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="68f11-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="68f11-123">Can be empty</span></span>  <br/> ||
   

