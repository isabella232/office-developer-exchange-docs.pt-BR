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
description: O elemento CreateFolder define uma solicitação para criar uma pasta no repositório do Exchange.
ms.openlocfilehash: c2a971a6b827553a1632c2a86e4d36e3b83a2de3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457540"
---
# <a name="createfolder"></a><span data-ttu-id="6b46a-103">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="6b46a-103">CreateFolder</span></span>

<span data-ttu-id="6b46a-104">O elemento **CreateFolder** define uma solicitação para criar uma pasta no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6b46a-104">The **CreateFolder** element defines a request to create a folder in the Exchange store.</span></span> 
  
```xml
<CreateFolder>
   <ParentFolderId/>
   <Folders/>
</CreateFolder>
```

 <span data-ttu-id="6b46a-105">**CreateFolderType**</span><span class="sxs-lookup"><span data-stu-id="6b46a-105">**CreateFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6b46a-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="6b46a-106">Attributes and elements</span></span>

<span data-ttu-id="6b46a-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6b46a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6b46a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="6b46a-108">Attributes</span></span>

<span data-ttu-id="6b46a-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6b46a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6b46a-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6b46a-110">Child elements</span></span>

|<span data-ttu-id="6b46a-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6b46a-111">**Element**</span></span>|<span data-ttu-id="6b46a-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6b46a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6b46a-113">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="6b46a-113">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> |<span data-ttu-id="6b46a-114">O elemento que identifica o local onde a nova pasta é criada.</span><span class="sxs-lookup"><span data-stu-id="6b46a-114">The element that identifies the location where the new folder is created.</span></span>  <br/> |
|[<span data-ttu-id="6b46a-115">Pastas</span><span class="sxs-lookup"><span data-stu-id="6b46a-115">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="6b46a-116">O elemento que contém todas as pastas a serem criadas.</span><span class="sxs-lookup"><span data-stu-id="6b46a-116">The element that contains all the folders to create.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6b46a-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6b46a-117">Parent elements</span></span>

<span data-ttu-id="6b46a-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6b46a-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6b46a-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="6b46a-119">Remarks</span></span>

<span data-ttu-id="6b46a-120">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="6b46a-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6b46a-121">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="6b46a-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6b46a-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="6b46a-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6b46a-123">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6b46a-123">Schema Name</span></span>  <br/> |<span data-ttu-id="6b46a-124">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="6b46a-124">Message schema</span></span>  <br/> |
|<span data-ttu-id="6b46a-125">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6b46a-125">Validation File</span></span>  <br/> |<span data-ttu-id="6b46a-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6b46a-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6b46a-127">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6b46a-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="6b46a-128">False</span><span class="sxs-lookup"><span data-stu-id="6b46a-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6b46a-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="6b46a-129">See also</span></span>



[<span data-ttu-id="6b46a-130">Operação CreateFolder</span><span class="sxs-lookup"><span data-stu-id="6b46a-130">CreateFolder operation</span></span>](createfolder-operation.md)


[<span data-ttu-id="6b46a-131">Criando pastas (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="6b46a-131">Creating Folders (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

