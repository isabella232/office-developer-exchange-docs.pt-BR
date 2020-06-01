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
description: O elemento CopyToFolder especifica o identificador da pasta para a qual os itens de email podem ser copiados.
ms.openlocfilehash: 7cdda0f9769f909255c9b76f78ac7094a8dfc8f8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463171"
---
# <a name="copytofolder"></a><span data-ttu-id="0b882-103">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="0b882-103">CopyToFolder</span></span>

<span data-ttu-id="0b882-104">O elemento **CopyToFolder** especifica o identificador da pasta para a qual os itens de email podem ser copiados.</span><span class="sxs-lookup"><span data-stu-id="0b882-104">The **CopyToFolder** element specifies the identifier of the folder that email items can be copied to.</span></span> 
  
```XML
<CopyToFolder>
    <FolderId></FolderId>
    <DistinguishedFolderId></DistinguisedFolderId>
</CopyToFolder>
```

 <span data-ttu-id="0b882-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="0b882-105">**TargetFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0b882-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="0b882-106">Attributes and elements</span></span>

<span data-ttu-id="0b882-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0b882-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0b882-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0b882-108">Attributes</span></span>

<span data-ttu-id="0b882-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0b882-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0b882-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0b882-110">Child elements</span></span>

|<span data-ttu-id="0b882-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0b882-111">**Element**</span></span>|<span data-ttu-id="0b882-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0b882-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b882-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="0b882-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="0b882-114">Contém o identificador de uma pasta de destino para uma pasta ou item copiado ou movido.</span><span class="sxs-lookup"><span data-stu-id="0b882-114">Contains the identifier of a destination folder for a copied or moved item or folder.</span></span>  <br/> |
|[<span data-ttu-id="0b882-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="0b882-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="0b882-116">Identifica uma pasta de destino nomeada para uma pasta ou item copiado ou movido.</span><span class="sxs-lookup"><span data-stu-id="0b882-116">Identifies a named destination folder for a copied or moved item or folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0b882-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0b882-117">Parent elements</span></span>

|<span data-ttu-id="0b882-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0b882-118">**Element**</span></span>|<span data-ttu-id="0b882-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0b882-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b882-120">Actions</span><span class="sxs-lookup"><span data-stu-id="0b882-120">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="0b882-121">Representa o conjunto de ações que estão disponíveis para serem realizadas em uma mensagem quando as condições forem atendidas.</span><span class="sxs-lookup"><span data-stu-id="0b882-121">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0b882-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="0b882-122">Text value</span></span>

<span data-ttu-id="0b882-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0b882-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0b882-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="0b882-124">Remarks</span></span>

<span data-ttu-id="0b882-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0b882-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0b882-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="0b882-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0b882-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="0b882-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0b882-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0b882-128">Schema Name</span></span>  <br/> |<span data-ttu-id="0b882-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="0b882-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0b882-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0b882-130">Validation File</span></span>  <br/> |<span data-ttu-id="0b882-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0b882-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0b882-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0b882-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="0b882-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="0b882-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0b882-134">Também consulte</span><span class="sxs-lookup"><span data-stu-id="0b882-134">See also</span></span>



[<span data-ttu-id="0b882-135">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="0b882-135">MoveToFolder</span></span>](movetofolder.md)


- [<span data-ttu-id="0b882-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0b882-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

