---
title: FolderChanges
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderChanges
api_type:
- schema
ms.assetid: d3f611ed-56a4-43f8-aa65-cbd7844b827f
description: O elemento FolderChanges representa uma coleção das alterações de uma pasta.
ms.openlocfilehash: 7ab89e79f6babb5e93863974835685c6975d96dd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752321"
---
# <a name="folderchanges"></a><span data-ttu-id="a0820-103">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="a0820-103">FolderChanges</span></span>

<span data-ttu-id="a0820-104">O elemento **FolderChanges** representa uma coleção das alterações de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="a0820-104">The **FolderChanges** element represents a collection of changes for a folder.</span></span> 
  
[<span data-ttu-id="a0820-105">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="a0820-105">UpdateFolder</span></span>](updatefolder.md)
  
[<span data-ttu-id="a0820-106">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="a0820-106">FolderChanges</span></span>](folderchanges.md)
  
```xml
<FolderChanges>
   <FolderChange/>
</FolderChanges>
```

 <span data-ttu-id="a0820-107">**NonEmptyArrayOfFolderChangesType**</span><span class="sxs-lookup"><span data-stu-id="a0820-107">**NonEmptyArrayOfFolderChangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a0820-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a0820-108">Attributes and elements</span></span>

<span data-ttu-id="a0820-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a0820-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a0820-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="a0820-110">Attributes</span></span>

<span data-ttu-id="a0820-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a0820-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a0820-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a0820-112">Child elements</span></span>

|<span data-ttu-id="a0820-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a0820-113">**Element**</span></span>|<span data-ttu-id="a0820-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a0820-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a0820-115">FolderChange</span><span class="sxs-lookup"><span data-stu-id="a0820-115">FolderChange</span></span>](folderchange.md) <br/> |<span data-ttu-id="a0820-116">Representa uma única alteração a ser executada em uma única pasta.</span><span class="sxs-lookup"><span data-stu-id="a0820-116">Represents a single change to be performed on a single folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a0820-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a0820-117">Parent elements</span></span>

|<span data-ttu-id="a0820-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a0820-118">**Element**</span></span>|<span data-ttu-id="a0820-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a0820-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a0820-120">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="a0820-120">UpdateFolder</span></span>](updatefolder.md) <br/> |<span data-ttu-id="a0820-121">Representa a operação que é usada para atualizar as propriedades de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="a0820-121">Represents the operation that is used to update properties for a folder.</span></span>  <br/> <span data-ttu-id="a0820-122">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="a0820-122">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateFolder` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a0820-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="a0820-123">Remarks</span></span>

<span data-ttu-id="a0820-124">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="a0820-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a0820-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a0820-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a0820-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="a0820-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a0820-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a0820-127">Schema Name</span></span>  <br/> |<span data-ttu-id="a0820-128">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="a0820-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a0820-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a0820-129">Validation File</span></span>  <br/> |<span data-ttu-id="a0820-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a0820-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a0820-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a0820-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="a0820-132">False</span><span class="sxs-lookup"><span data-stu-id="a0820-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a0820-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="a0820-133">See also</span></span>



[<span data-ttu-id="a0820-134">Operação UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="a0820-134">UpdateFolder operation</span></span>](updatefolder-operation.md)

