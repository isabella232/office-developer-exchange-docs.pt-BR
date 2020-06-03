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
description: O elemento ToFolderId representa a pasta de destino para uma pasta ou item copiado ou movido.
ms.openlocfilehash: c9cceb17fd55b7357d54b37bf4c8da1137d39b6a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44468772"
---
# <a name="tofolderid"></a><span data-ttu-id="468fc-103">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="468fc-103">ToFolderId</span></span>

<span data-ttu-id="468fc-104">O elemento **ToFolderId** representa a pasta de destino para uma pasta ou item copiado ou movido.</span><span class="sxs-lookup"><span data-stu-id="468fc-104">The **ToFolderId** element represents the destination folder for a copied or moved item or folder.</span></span> 
  
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

<span data-ttu-id="468fc-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="468fc-105">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="468fc-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="468fc-106">Attributes and elements</span></span>

<span data-ttu-id="468fc-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="468fc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="468fc-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="468fc-108">Attributes</span></span>

<span data-ttu-id="468fc-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="468fc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="468fc-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="468fc-110">Child elements</span></span>

|<span data-ttu-id="468fc-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="468fc-111">**Element**</span></span>|<span data-ttu-id="468fc-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="468fc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="468fc-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="468fc-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="468fc-114">Contém o identificador de uma pasta de destino para uma pasta ou item copiado ou movido.</span><span class="sxs-lookup"><span data-stu-id="468fc-114">Contains the identifier of a destination folder for a copied or moved item or folder.</span></span>  <br/> |
|[<span data-ttu-id="468fc-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="468fc-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="468fc-116">Identifica uma pasta de destino nomeada para uma pasta ou item copiado ou movido.</span><span class="sxs-lookup"><span data-stu-id="468fc-116">Identifies a named destination folder for a copied or moved item or folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="468fc-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="468fc-117">Parent elements</span></span>

|<span data-ttu-id="468fc-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="468fc-118">**Element**</span></span>|<span data-ttu-id="468fc-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="468fc-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="468fc-120">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="468fc-120">MoveFolder</span></span>](movefolder.md) <br/> |<span data-ttu-id="468fc-121">Define uma solicitação para mover uma pasta no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="468fc-121">Defines a request to move a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="468fc-122">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="468fc-122">The following is the XPath expression to this element:</span></span>  <br/>  `/MoveFolder` <br/> |
|[<span data-ttu-id="468fc-123">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="468fc-123">CopyFolder</span></span>](copyfolder.md) <br/> |<span data-ttu-id="468fc-124">Define uma solicitação para copiar uma pasta no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="468fc-124">Defines a request to copy a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="468fc-125">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="468fc-125">The following is the XPath expression to this element:</span></span>  <br/>  `/CopyFolder` <br/> |
|[<span data-ttu-id="468fc-126">MoveItem</span><span class="sxs-lookup"><span data-stu-id="468fc-126">MoveItem</span></span>](moveitem.md) <br/> |<span data-ttu-id="468fc-127">Define uma solicitação para mover um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="468fc-127">Defines a request to move an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="468fc-128">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="468fc-128">The following is the XPath expression to this element:</span></span>  <br/>  `/MoveItem` <br/> |
|[<span data-ttu-id="468fc-129">CopyItem</span><span class="sxs-lookup"><span data-stu-id="468fc-129">CopyItem</span></span>](copyitem.md) <br/> |<span data-ttu-id="468fc-130">Define uma solicitação para copiar um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="468fc-130">Defines a request to copy an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="468fc-131">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="468fc-131">The following is the XPath expression to this element:</span></span>  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="468fc-132">Comentários</span><span class="sxs-lookup"><span data-stu-id="468fc-132">Remarks</span></span>

<span data-ttu-id="468fc-133">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="468fc-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="468fc-134">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="468fc-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="468fc-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="468fc-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="468fc-136">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="468fc-136">Schema Name</span></span>  <br/> |<span data-ttu-id="468fc-137">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="468fc-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="468fc-138">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="468fc-138">Validation File</span></span>  <br/> |<span data-ttu-id="468fc-139">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="468fc-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="468fc-140">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="468fc-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="468fc-141">False</span><span class="sxs-lookup"><span data-stu-id="468fc-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="468fc-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="468fc-142">See also</span></span>

- [<span data-ttu-id="468fc-143">Operação MoveFolder</span><span class="sxs-lookup"><span data-stu-id="468fc-143">MoveFolder operation</span></span>](movefolder-operation.md)  
- [<span data-ttu-id="468fc-144">Operação CopyFolder</span><span class="sxs-lookup"><span data-stu-id="468fc-144">CopyFolder operation</span></span>](copyfolder-operation.md) 
- [<span data-ttu-id="468fc-145">Operação MoveItem</span><span class="sxs-lookup"><span data-stu-id="468fc-145">MoveItem operation</span></span>](moveitem-operation.md) 
- [<span data-ttu-id="468fc-146">Operação CopyItem</span><span class="sxs-lookup"><span data-stu-id="468fc-146">CopyItem operation</span></span>](copyitem-operation.md)

