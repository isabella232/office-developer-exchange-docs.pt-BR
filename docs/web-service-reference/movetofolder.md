---
title: MoveToFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveToFolder
api_type:
- schema
ms.assetid: 991673b9-b627-4848-bfba-59a187b8575f
description: O elemento MoveToFolder especifica o identificador da pasta para a qual os itens de email podem ser movidos.
ms.openlocfilehash: e323b2ac5390855b3db0b5495af667cdf2da5596
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529999"
---
# <a name="movetofolder"></a><span data-ttu-id="ae6a1-103">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="ae6a1-103">MoveToFolder</span></span>

<span data-ttu-id="ae6a1-104">O elemento **MoveToFolder** especifica o identificador da pasta para a qual os itens de email podem ser movidos.</span><span class="sxs-lookup"><span data-stu-id="ae6a1-104">The **MoveToFolder** element specifies the identifier of the folder to which email items can be moved.</span></span> 
  
```XML
<MoveToFolder>
    <FolderId></FolderId>
    <DistinguishedFolderId></DistinguisedFolderId>
</MoveToFolder>
```

 <span data-ttu-id="ae6a1-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="ae6a1-105">**TargetFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ae6a1-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ae6a1-106">Attributes and elements</span></span>

<span data-ttu-id="ae6a1-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ae6a1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ae6a1-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ae6a1-108">Attributes</span></span>

<span data-ttu-id="ae6a1-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ae6a1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ae6a1-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ae6a1-110">Child elements</span></span>

|<span data-ttu-id="ae6a1-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ae6a1-111">**Element**</span></span>|<span data-ttu-id="ae6a1-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ae6a1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ae6a1-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="ae6a1-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="ae6a1-114">Contém o identificador de uma pasta de destino para uma pasta ou item copiado ou movido.</span><span class="sxs-lookup"><span data-stu-id="ae6a1-114">Contains the identifier of a destination folder for a copied or moved item or folder.</span></span>  <br/> |
|[<span data-ttu-id="ae6a1-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="ae6a1-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="ae6a1-116">Identifica uma pasta de destino nomeada para uma pasta ou item copiado ou movido.</span><span class="sxs-lookup"><span data-stu-id="ae6a1-116">Identifies a named destination folder for a copied or moved item or folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ae6a1-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ae6a1-117">Parent elements</span></span>

|<span data-ttu-id="ae6a1-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ae6a1-118">**Element**</span></span>|<span data-ttu-id="ae6a1-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ae6a1-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ae6a1-120">Actions</span><span class="sxs-lookup"><span data-stu-id="ae6a1-120">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="ae6a1-121">Representa o conjunto de ações que estão disponíveis para serem realizadas em uma mensagem quando as condições forem atendidas..</span><span class="sxs-lookup"><span data-stu-id="ae6a1-121">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled..</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ae6a1-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="ae6a1-122">Text value</span></span>

<span data-ttu-id="ae6a1-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ae6a1-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ae6a1-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="ae6a1-124">Remarks</span></span>

<span data-ttu-id="ae6a1-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ae6a1-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ae6a1-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ae6a1-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ae6a1-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="ae6a1-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ae6a1-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ae6a1-128">Schema Name</span></span>  <br/> |<span data-ttu-id="ae6a1-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="ae6a1-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ae6a1-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ae6a1-130">Validation File</span></span>  <br/> |<span data-ttu-id="ae6a1-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ae6a1-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ae6a1-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ae6a1-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="ae6a1-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="ae6a1-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ae6a1-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="ae6a1-134">See also</span></span>



[<span data-ttu-id="ae6a1-135">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="ae6a1-135">CopyToFolder</span></span>](copytofolder.md)


- [<span data-ttu-id="ae6a1-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ae6a1-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

