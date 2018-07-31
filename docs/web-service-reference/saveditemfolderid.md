---
title: SavedItemFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SavedItemFolderId
api_type:
- schema
ms.assetid: 4b8b475c-9ca5-48c9-acb0-8848b53be1ce
description: O elemento SavedItemFolderId identifica a pasta de destino para operações que atualizar, enviar e criar itens em uma caixa de correio.
ms.openlocfilehash: 3f46070a538f5e03007925565a8888efe06b62b7
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354159"
---
# <a name="saveditemfolderid"></a><span data-ttu-id="781d4-103">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="781d4-103">SavedItemFolderId</span></span>

<span data-ttu-id="781d4-104">O elemento **SavedItemFolderId** identifica a pasta de destino para operações que atualizar, enviar e criar itens em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="781d4-104">The **SavedItemFolderId** element identifies the target folder for operations that update, send, and create items in a mailbox.</span></span> 
  
```xml
<SavedItemFolderId>
   <FolderId/>
</SavedItemFolderId>
```

```xml
<SavedItemFolderId>
   <DistinguishedFolderId/>
</SavedItemFolderId>
```

<span data-ttu-id="781d4-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="781d4-105">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="781d4-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="781d4-106">Attributes and elements</span></span>

<span data-ttu-id="781d4-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="781d4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="781d4-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="781d4-108">Attributes</span></span>

<span data-ttu-id="781d4-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="781d4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="781d4-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="781d4-110">Child elements</span></span>

|<span data-ttu-id="781d4-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="781d4-111">**Element**</span></span>|<span data-ttu-id="781d4-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="781d4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="781d4-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="781d4-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="781d4-114">Contém o identificador e alterar a chave de uma pasta de destino para operações de atualização, enviar e crie itens no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="781d4-114">Contains the identifier and change key of a target folder for operations that update, send, and create items in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="781d4-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="781d4-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="781d4-116">Identifica uma pasta de destino por um identificador nomeado nas operações que atualizar, enviar e criar itens no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="781d4-116">Identifies a target folder by a named identifier for operations that update, send, and create items in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="781d4-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="781d4-117">Parent elements</span></span>

|<span data-ttu-id="781d4-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="781d4-118">**Element**</span></span>|<span data-ttu-id="781d4-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="781d4-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="781d4-120">CreateItem</span><span class="sxs-lookup"><span data-stu-id="781d4-120">CreateItem</span></span>](createitem.md) <br/> |<span data-ttu-id="781d4-121">Define uma solicitação para criar um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="781d4-121">Defines a request to create an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="781d4-122">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="781d4-122">The following is the XPath expression to this element:</span></span>  <br/>  `/CreateItem` <br/> |
|[<span data-ttu-id="781d4-123">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="781d4-123">UpdateItem</span></span>](updateitem.md) <br/> |<span data-ttu-id="781d4-124">Define uma solicitação de atualização de um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="781d4-124">Defines a request to update an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="781d4-125">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="781d4-125">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateItem` <br/> |
|[<span data-ttu-id="781d4-126">SendItem</span><span class="sxs-lookup"><span data-stu-id="781d4-126">SendItem</span></span>](senditem.md) <br/> |<span data-ttu-id="781d4-127">Define uma solicitação para enviar um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="781d4-127">Defines a request to send an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="781d4-128">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="781d4-128">The following is the XPath expression to this element:</span></span>  <br/>  `/SendItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="781d4-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="781d4-129">Remarks</span></span>

<span data-ttu-id="781d4-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="781d4-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="781d4-131">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="781d4-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="781d4-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="781d4-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="781d4-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="781d4-133">Schema Name</span></span>  <br/> |<span data-ttu-id="781d4-134">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="781d4-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="781d4-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="781d4-135">Validation File</span></span>  <br/> |<span data-ttu-id="781d4-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="781d4-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="781d4-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="781d4-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="781d4-138">False</span><span class="sxs-lookup"><span data-stu-id="781d4-138">False</span></span>  <br/> |
   

