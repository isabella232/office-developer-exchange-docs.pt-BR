---
title: CreateFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateFolder
api_type:
- schema
ms.assetid: 110bada1-517b-4bd6-870d-7086dc879e5d
description: O elemento de CreateFolder define uma solicitação para criar uma pasta no repositório do Exchange.
ms.openlocfilehash: e30af23b8ed8669053b94be460d62fbf7abf24c9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751579"
---
# <a name="createfolder"></a><span data-ttu-id="b9425-103">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="b9425-103">CreateFolder</span></span>

<span data-ttu-id="b9425-104">O elemento de **CreateFolder** define uma solicitação para criar uma pasta no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b9425-104">The **CreateFolder** element defines a request to create a folder in the Exchange store.</span></span> 
  
```xml
<CreateFolder>
   <ParentFolderId/>
   <Folders/>
</CreateFolder>
```

 <span data-ttu-id="b9425-105">**CreateFolderType**</span><span class="sxs-lookup"><span data-stu-id="b9425-105">**CreateFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b9425-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b9425-106">Attributes and elements</span></span>

<span data-ttu-id="b9425-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b9425-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b9425-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b9425-108">Attributes</span></span>

<span data-ttu-id="b9425-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b9425-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b9425-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b9425-110">Child elements</span></span>

|<span data-ttu-id="b9425-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b9425-111">**Element**</span></span>|<span data-ttu-id="b9425-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b9425-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b9425-113">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="b9425-113">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> |<span data-ttu-id="b9425-114">O elemento que identifica o local onde a nova pasta é criada.</span><span class="sxs-lookup"><span data-stu-id="b9425-114">The element that identifies the location where the new folder is created.</span></span>  <br/> |
|[<span data-ttu-id="b9425-115">Pastas</span><span class="sxs-lookup"><span data-stu-id="b9425-115">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="b9425-116">O elemento que contém todas as pastas para criar.</span><span class="sxs-lookup"><span data-stu-id="b9425-116">The element that contains all the folders to create.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b9425-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b9425-117">Parent elements</span></span>

<span data-ttu-id="b9425-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b9425-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b9425-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="b9425-119">Remarks</span></span>

<span data-ttu-id="b9425-120">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="b9425-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b9425-121">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b9425-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b9425-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="b9425-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b9425-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b9425-123">Schema Name</span></span>  <br/> |<span data-ttu-id="b9425-124">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="b9425-124">Message schema</span></span>  <br/> |
|<span data-ttu-id="b9425-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b9425-125">Validation File</span></span>  <br/> |<span data-ttu-id="b9425-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b9425-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b9425-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b9425-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="b9425-128">False</span><span class="sxs-lookup"><span data-stu-id="b9425-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b9425-129">Ver também</span><span class="sxs-lookup"><span data-stu-id="b9425-129">See also</span></span>



[<span data-ttu-id="b9425-130">Operação CreateFolder</span><span class="sxs-lookup"><span data-stu-id="b9425-130">CreateFolder operation</span></span>](createfolder-operation.md)


[<span data-ttu-id="b9425-131">Criação de pastas (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="b9425-131">Creating Folders (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

