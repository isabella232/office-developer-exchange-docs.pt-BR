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
description: O elemento MoveToFolder Especifica o identificador da pasta para o qual os itens de email podem ser movidos.
ms.openlocfilehash: 058f008b348d49c932bf334dd3379f02d06154e9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824494"
---
# <a name="movetofolder"></a><span data-ttu-id="ec180-103">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="ec180-103">MoveToFolder</span></span>

<span data-ttu-id="ec180-104">O elemento **MoveToFolder** Especifica o identificador da pasta para o qual os itens de email podem ser movidos.</span><span class="sxs-lookup"><span data-stu-id="ec180-104">The **MoveToFolder** element specifies the identifier of the folder to which email items can be moved.</span></span> 
  
```XML
<MoveToFolder>
    <FolderId></FolderId>
    <DistinguishedFolderId></DistinguisedFolderId>
</MoveToFolder>
```

 <span data-ttu-id="ec180-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="ec180-105">**TargetFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ec180-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ec180-106">Attributes and elements</span></span>

<span data-ttu-id="ec180-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ec180-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ec180-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ec180-108">Attributes</span></span>

<span data-ttu-id="ec180-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ec180-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ec180-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ec180-110">Child elements</span></span>

|<span data-ttu-id="ec180-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ec180-111">**Element**</span></span>|<span data-ttu-id="ec180-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ec180-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ec180-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="ec180-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="ec180-114">Contém o identificador de uma pasta de destino para um item movido ou copiada ou uma pasta.</span><span class="sxs-lookup"><span data-stu-id="ec180-114">Contains the identifier of a destination folder for a copied or moved item or folder.</span></span>  <br/> |
|[<span data-ttu-id="ec180-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="ec180-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="ec180-116">Identifica uma pasta de destino nomeado para um item movido ou copiada ou uma pasta.</span><span class="sxs-lookup"><span data-stu-id="ec180-116">Identifies a named destination folder for a copied or moved item or folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ec180-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ec180-117">Parent elements</span></span>

|<span data-ttu-id="ec180-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ec180-118">**Element**</span></span>|<span data-ttu-id="ec180-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ec180-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ec180-120">Ações</span><span class="sxs-lookup"><span data-stu-id="ec180-120">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="ec180-121">Representa o conjunto de ações que estão disponíveis a ser executada em uma mensagem quando as condições são atendidas..</span><span class="sxs-lookup"><span data-stu-id="ec180-121">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled..</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ec180-122">Text value</span><span class="sxs-lookup"><span data-stu-id="ec180-122">Text value</span></span>

<span data-ttu-id="ec180-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ec180-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ec180-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="ec180-124">Remarks</span></span>

<span data-ttu-id="ec180-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec180-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ec180-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ec180-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ec180-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="ec180-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ec180-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ec180-128">Schema Name</span></span>  <br/> |<span data-ttu-id="ec180-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="ec180-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ec180-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ec180-130">Validation File</span></span>  <br/> |<span data-ttu-id="ec180-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ec180-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ec180-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ec180-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="ec180-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="ec180-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ec180-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="ec180-134">See also</span></span>



[<span data-ttu-id="ec180-135">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="ec180-135">CopyToFolder</span></span>](copytofolder.md)


- [<span data-ttu-id="ec180-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ec180-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

