---
title: CopyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyFolder
api_type:
- schema
ms.assetid: 7d5cd08a-fe81-4cb6-a5a0-6dec2d3c93d4
description: O elemento de CopyFolder define uma solicitação para copiar pastas em uma caixa de correio no armazenamento do Exchange.
ms.openlocfilehash: 7bcfcc7f4212b3a3bd339fa5863df2990eb20d6d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751548"
---
# <a name="copyfolder"></a><span data-ttu-id="12516-103">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="12516-103">CopyFolder</span></span>

<span data-ttu-id="12516-104">O elemento de **CopyFolder** define uma solicitação para copiar pastas em uma caixa de correio no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="12516-104">The **CopyFolder** element defines a request to copy folders in a mailbox in the Exchange store.</span></span> 
  
```xml
<CopyFolder>
   <ToFolderId/>
   <FolderIds/>
</CopyFolder>
```

 <span data-ttu-id="12516-105">**CopyFolderType**</span><span class="sxs-lookup"><span data-stu-id="12516-105">**CopyFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="12516-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="12516-106">Attributes and elements</span></span>

<span data-ttu-id="12516-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="12516-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="12516-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="12516-108">Attributes</span></span>

<span data-ttu-id="12516-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="12516-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="12516-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="12516-110">Child elements</span></span>

|<span data-ttu-id="12516-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="12516-111">**Element**</span></span>|<span data-ttu-id="12516-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="12516-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="12516-113">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="12516-113">ToFolderId</span></span>](tofolderid.md) <br/> |<span data-ttu-id="12516-114">Representa a pasta de destino para uma pasta copiada.</span><span class="sxs-lookup"><span data-stu-id="12516-114">Represents the destination folder for a copied folder.</span></span>  <br/> |
|[<span data-ttu-id="12516-115">FolderIds</span><span class="sxs-lookup"><span data-stu-id="12516-115">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="12516-116">Contém uma matriz de pastas a serem copiados para a pasta identificada pelo elemento [ToFolderId](tofolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="12516-116">Contains an array of folders to copy to the folder identified by the [ToFolderId](tofolderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="12516-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="12516-117">Parent elements</span></span>

<span data-ttu-id="12516-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="12516-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="12516-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="12516-119">Remarks</span></span>

<span data-ttu-id="12516-120">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="12516-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="12516-121">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="12516-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="12516-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="12516-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="12516-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="12516-123">Schema Name</span></span>  <br/> |<span data-ttu-id="12516-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="12516-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="12516-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="12516-125">Validation File</span></span>  <br/> |<span data-ttu-id="12516-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="12516-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="12516-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="12516-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="12516-128">False</span><span class="sxs-lookup"><span data-stu-id="12516-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="12516-129">Ver também</span><span class="sxs-lookup"><span data-stu-id="12516-129">See also</span></span>



[<span data-ttu-id="12516-130">Operação CopyFolder</span><span class="sxs-lookup"><span data-stu-id="12516-130">CopyFolder operation</span></span>](copyfolder-operation.md)

