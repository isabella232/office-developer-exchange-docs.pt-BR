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
description: O elemento CopyFolder define uma solicitação para copiar pastas em uma caixa de correio no repositório do Exchange.
ms.openlocfilehash: fa75272540169a96d5567181d27b8a8f056cce42
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44452507"
---
# <a name="copyfolder"></a><span data-ttu-id="9453d-103">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="9453d-103">CopyFolder</span></span>

<span data-ttu-id="9453d-104">O elemento **CopyFolder** define uma solicitação para copiar pastas em uma caixa de correio no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9453d-104">The **CopyFolder** element defines a request to copy folders in a mailbox in the Exchange store.</span></span> 
  
```xml
<CopyFolder>
   <ToFolderId/>
   <FolderIds/>
</CopyFolder>
```

 <span data-ttu-id="9453d-105">**CopyFolderType**</span><span class="sxs-lookup"><span data-stu-id="9453d-105">**CopyFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9453d-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="9453d-106">Attributes and elements</span></span>

<span data-ttu-id="9453d-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9453d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9453d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9453d-108">Attributes</span></span>

<span data-ttu-id="9453d-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9453d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9453d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9453d-110">Child elements</span></span>

|<span data-ttu-id="9453d-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9453d-111">**Element**</span></span>|<span data-ttu-id="9453d-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9453d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9453d-113">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="9453d-113">ToFolderId</span></span>](tofolderid.md) <br/> |<span data-ttu-id="9453d-114">Representa a pasta de destino de uma pasta copiada.</span><span class="sxs-lookup"><span data-stu-id="9453d-114">Represents the destination folder for a copied folder.</span></span>  <br/> |
|[<span data-ttu-id="9453d-115">FolderIds</span><span class="sxs-lookup"><span data-stu-id="9453d-115">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="9453d-116">Contém uma matriz de pastas a serem copiadas para a pasta identificada pelo elemento [ToFolderId](tofolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="9453d-116">Contains an array of folders to copy to the folder identified by the [ToFolderId](tofolderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9453d-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9453d-117">Parent elements</span></span>

<span data-ttu-id="9453d-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9453d-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9453d-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="9453d-119">Remarks</span></span>

<span data-ttu-id="9453d-120">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="9453d-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9453d-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="9453d-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9453d-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="9453d-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9453d-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9453d-123">Schema Name</span></span>  <br/> |<span data-ttu-id="9453d-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="9453d-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9453d-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9453d-125">Validation File</span></span>  <br/> |<span data-ttu-id="9453d-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9453d-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9453d-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9453d-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="9453d-128">False</span><span class="sxs-lookup"><span data-stu-id="9453d-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9453d-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="9453d-129">See also</span></span>



[<span data-ttu-id="9453d-130">Operação CopyFolder</span><span class="sxs-lookup"><span data-stu-id="9453d-130">CopyFolder operation</span></span>](copyfolder-operation.md)

