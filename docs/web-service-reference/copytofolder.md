---
title: CopyToFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyToFolder
api_type:
- schema
ms.assetid: 6fd8a6b8-d813-43ff-991b-0e9e782fe00e
description: O elemento CopyToFolder Especifica o identificador da pasta esse email itens podem ser copiados para.
ms.openlocfilehash: b641c23b7aed11ae85157e2ed01cfa9d61d07e0a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751554"
---
# <a name="copytofolder"></a><span data-ttu-id="00cf8-103">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="00cf8-103">CopyToFolder</span></span>

<span data-ttu-id="00cf8-104">O elemento **CopyToFolder** Especifica o identificador da pasta esse email itens podem ser copiados para.</span><span class="sxs-lookup"><span data-stu-id="00cf8-104">The **CopyToFolder** element specifies the identifier of the folder that email items can be copied to.</span></span> 
  
```XML
<CopyToFolder>
    <FolderId></FolderId>
    <DistinguishedFolderId></DistinguisedFolderId>
</CopyToFolder>
```

 <span data-ttu-id="00cf8-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="00cf8-105">**TargetFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="00cf8-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="00cf8-106">Attributes and elements</span></span>

<span data-ttu-id="00cf8-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="00cf8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="00cf8-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="00cf8-108">Attributes</span></span>

<span data-ttu-id="00cf8-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="00cf8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="00cf8-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="00cf8-110">Child elements</span></span>

|<span data-ttu-id="00cf8-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="00cf8-111">**Element**</span></span>|<span data-ttu-id="00cf8-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="00cf8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00cf8-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="00cf8-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="00cf8-114">Contém o identificador de uma pasta de destino para um item movido ou copiada ou uma pasta.</span><span class="sxs-lookup"><span data-stu-id="00cf8-114">Contains the identifier of a destination folder for a copied or moved item or folder.</span></span>  <br/> |
|[<span data-ttu-id="00cf8-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="00cf8-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="00cf8-116">Identifica uma pasta de destino nomeado para um item movido ou copiada ou uma pasta.</span><span class="sxs-lookup"><span data-stu-id="00cf8-116">Identifies a named destination folder for a copied or moved item or folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="00cf8-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="00cf8-117">Parent elements</span></span>

|<span data-ttu-id="00cf8-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="00cf8-118">**Element**</span></span>|<span data-ttu-id="00cf8-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="00cf8-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00cf8-120">Ações</span><span class="sxs-lookup"><span data-stu-id="00cf8-120">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="00cf8-121">Representa o conjunto de ações que estão disponíveis a ser executada em uma mensagem quando as condições são atendidas.</span><span class="sxs-lookup"><span data-stu-id="00cf8-121">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="00cf8-122">Text value</span><span class="sxs-lookup"><span data-stu-id="00cf8-122">Text value</span></span>

<span data-ttu-id="00cf8-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="00cf8-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="00cf8-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="00cf8-124">Remarks</span></span>

<span data-ttu-id="00cf8-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="00cf8-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="00cf8-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="00cf8-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="00cf8-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="00cf8-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="00cf8-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="00cf8-128">Schema Name</span></span>  <br/> |<span data-ttu-id="00cf8-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="00cf8-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="00cf8-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="00cf8-130">Validation File</span></span>  <br/> |<span data-ttu-id="00cf8-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="00cf8-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="00cf8-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="00cf8-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="00cf8-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="00cf8-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="00cf8-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="00cf8-134">See also</span></span>



[<span data-ttu-id="00cf8-135">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="00cf8-135">MoveToFolder</span></span>](movetofolder.md)


- [<span data-ttu-id="00cf8-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="00cf8-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

