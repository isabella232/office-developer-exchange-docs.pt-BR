---
title: MoveFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveFolder
api_type:
- schema
ms.assetid: f2bb0a73-94d7-4bc7-8902-bd9c69120221
description: O elemento de MoveFolder define uma solicitação para mover uma pasta no repositório do Exchange.
ms.openlocfilehash: 42a990ced18cc13c7694042df786d33c018f346c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824485"
---
# <a name="movefolder"></a><span data-ttu-id="0ca8c-103">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="0ca8c-103">MoveFolder</span></span>

<span data-ttu-id="0ca8c-104">O elemento de **MoveFolder** define uma solicitação para mover uma pasta no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ca8c-104">The **MoveFolder** element defines a request to move a folder in the Exchange store.</span></span> 
  
```xml
<MoveFolder>
   <ToFolderId/>
   <FolderIds/>
</MoveFolder>
```

 <span data-ttu-id="0ca8c-105">**MoveFolderType**</span><span class="sxs-lookup"><span data-stu-id="0ca8c-105">**MoveFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0ca8c-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="0ca8c-106">Attributes and elements</span></span>

<span data-ttu-id="0ca8c-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0ca8c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0ca8c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0ca8c-108">Attributes</span></span>

<span data-ttu-id="0ca8c-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0ca8c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0ca8c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0ca8c-110">Child elements</span></span>

|<span data-ttu-id="0ca8c-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0ca8c-111">**Element**</span></span>|<span data-ttu-id="0ca8c-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0ca8c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0ca8c-113">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="0ca8c-113">ToFolderId</span></span>](tofolderid.md) <br/> |<span data-ttu-id="0ca8c-114">Representa a pasta de destino para uma pasta movida.</span><span class="sxs-lookup"><span data-stu-id="0ca8c-114">Represents the destination folder for a moved folder.</span></span>  <br/> |
|[<span data-ttu-id="0ca8c-115">FolderIds</span><span class="sxs-lookup"><span data-stu-id="0ca8c-115">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="0ca8c-116">Contém uma matriz de pastas para mover para a pasta identificada pelo elemento [ToFolderId](tofolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="0ca8c-116">Contains an array of folders to move to the folder identified by the [ToFolderId](tofolderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0ca8c-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0ca8c-117">Parent elements</span></span>

<span data-ttu-id="0ca8c-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0ca8c-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0ca8c-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="0ca8c-119">Remarks</span></span>

<span data-ttu-id="0ca8c-120">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="0ca8c-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0ca8c-121">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="0ca8c-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0ca8c-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="0ca8c-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0ca8c-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0ca8c-123">Schema Name</span></span>  <br/> |<span data-ttu-id="0ca8c-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="0ca8c-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0ca8c-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0ca8c-125">Validation File</span></span>  <br/> |<span data-ttu-id="0ca8c-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0ca8c-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0ca8c-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0ca8c-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="0ca8c-128">False</span><span class="sxs-lookup"><span data-stu-id="0ca8c-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0ca8c-129">Ver também</span><span class="sxs-lookup"><span data-stu-id="0ca8c-129">See also</span></span>



[<span data-ttu-id="0ca8c-130">Operação MoveFolder</span><span class="sxs-lookup"><span data-stu-id="0ca8c-130">MoveFolder operation</span></span>](movefolder-operation.md)

