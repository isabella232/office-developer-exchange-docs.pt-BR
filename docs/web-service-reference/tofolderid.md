---
title: ToFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ToFolderId
api_type:
- schema
ms.assetid: bd6a4265-ad40-43f6-bcc4-0bf5df4e984c
description: O elemento ToFolderId representa a pasta de destino para um item movido ou copiada ou uma pasta.
ms.openlocfilehash: 9d2fd6c177711cfe3a5d3415320440259e2f5289
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353655"
---
# <a name="tofolderid"></a><span data-ttu-id="18520-103">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="18520-103">ToFolderId</span></span>

<span data-ttu-id="18520-104">O elemento **ToFolderId** representa a pasta de destino para um item movido ou copiada ou uma pasta.</span><span class="sxs-lookup"><span data-stu-id="18520-104">The **ToFolderId** element represents the destination folder for a copied or moved item or folder.</span></span> 
  
```xml
<ToFolderId>
   <FolderId/>
</ToFolderId>
```

```xml
<ToFolderId>
   <DistinguishedFolderId/>
</ToFolderId>
```

<span data-ttu-id="18520-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="18520-105">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="18520-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="18520-106">Attributes and elements</span></span>

<span data-ttu-id="18520-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="18520-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="18520-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="18520-108">Attributes</span></span>

<span data-ttu-id="18520-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="18520-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="18520-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="18520-110">Child elements</span></span>

|<span data-ttu-id="18520-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="18520-111">**Element**</span></span>|<span data-ttu-id="18520-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="18520-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18520-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="18520-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="18520-114">Contém o identificador de uma pasta de destino para um item movido ou copiada ou uma pasta.</span><span class="sxs-lookup"><span data-stu-id="18520-114">Contains the identifier of a destination folder for a copied or moved item or folder.</span></span>  <br/> |
|[<span data-ttu-id="18520-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="18520-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="18520-116">Identifica uma pasta de destino nomeado para um item movido ou copiada ou uma pasta.</span><span class="sxs-lookup"><span data-stu-id="18520-116">Identifies a named destination folder for a copied or moved item or folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="18520-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="18520-117">Parent elements</span></span>

|<span data-ttu-id="18520-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="18520-118">**Element**</span></span>|<span data-ttu-id="18520-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="18520-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="18520-120">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="18520-120">MoveFolder</span></span>](movefolder.md) <br/> |<span data-ttu-id="18520-121">Define uma solicitação para mover uma pasta no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="18520-121">Defines a request to move a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="18520-122">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="18520-122">The following is the XPath expression to this element:</span></span>  <br/>  `/MoveFolder` <br/> |
|[<span data-ttu-id="18520-123">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="18520-123">CopyFolder</span></span>](copyfolder.md) <br/> |<span data-ttu-id="18520-124">Define uma solicitação para copiar uma pasta no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="18520-124">Defines a request to copy a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="18520-125">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="18520-125">The following is the XPath expression to this element:</span></span>  <br/>  `/CopyFolder` <br/> |
|[<span data-ttu-id="18520-126">MoveItem</span><span class="sxs-lookup"><span data-stu-id="18520-126">MoveItem</span></span>](moveitem.md) <br/> |<span data-ttu-id="18520-127">Define uma solicitação para mover um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="18520-127">Defines a request to move an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="18520-128">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="18520-128">The following is the XPath expression to this element:</span></span>  <br/>  `/MoveItem` <br/> |
|[<span data-ttu-id="18520-129">CopyItem</span><span class="sxs-lookup"><span data-stu-id="18520-129">CopyItem</span></span>](copyitem.md) <br/> |<span data-ttu-id="18520-130">Define uma solicitação para copiar um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="18520-130">Defines a request to copy an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="18520-131">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="18520-131">The following is the XPath expression to this element:</span></span>  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="18520-132">Comentários</span><span class="sxs-lookup"><span data-stu-id="18520-132">Remarks</span></span>

<span data-ttu-id="18520-133">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="18520-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="18520-134">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="18520-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="18520-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="18520-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="18520-136">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="18520-136">Schema Name</span></span>  <br/> |<span data-ttu-id="18520-137">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="18520-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="18520-138">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="18520-138">Validation File</span></span>  <br/> |<span data-ttu-id="18520-139">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="18520-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="18520-140">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="18520-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="18520-141">False</span><span class="sxs-lookup"><span data-stu-id="18520-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="18520-142">Ver também</span><span class="sxs-lookup"><span data-stu-id="18520-142">See also</span></span>

- [<span data-ttu-id="18520-143">Operação MoveFolder</span><span class="sxs-lookup"><span data-stu-id="18520-143">MoveFolder operation</span></span>](movefolder-operation.md)  
- [<span data-ttu-id="18520-144">Operação CopyFolder</span><span class="sxs-lookup"><span data-stu-id="18520-144">CopyFolder operation</span></span>](copyfolder-operation.md) 
- [<span data-ttu-id="18520-145">Operação MoveItem</span><span class="sxs-lookup"><span data-stu-id="18520-145">MoveItem operation</span></span>](moveitem-operation.md) 
- [<span data-ttu-id="18520-146">Operação CopyItem</span><span class="sxs-lookup"><span data-stu-id="18520-146">CopyItem operation</span></span>](copyitem-operation.md)

