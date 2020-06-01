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
description: O elemento SavedItemFolderId identifica a pasta de destino para operações que atualizam, enviam e criam itens em uma caixa de correio.
ms.openlocfilehash: 8e18b8863a54aa4e9d6e65f7a54e20904f5a9599
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465272"
---
# <a name="saveditemfolderid"></a><span data-ttu-id="12342-103">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="12342-103">SavedItemFolderId</span></span>

<span data-ttu-id="12342-104">O elemento **SavedItemFolderId** identifica a pasta de destino para operações que atualizam, enviam e criam itens em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="12342-104">The **SavedItemFolderId** element identifies the target folder for operations that update, send, and create items in a mailbox.</span></span> 
  
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

<span data-ttu-id="12342-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="12342-105">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="12342-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="12342-106">Attributes and elements</span></span>

<span data-ttu-id="12342-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="12342-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="12342-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="12342-108">Attributes</span></span>

<span data-ttu-id="12342-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="12342-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="12342-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="12342-110">Child elements</span></span>

|<span data-ttu-id="12342-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="12342-111">**Element**</span></span>|<span data-ttu-id="12342-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="12342-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="12342-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="12342-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="12342-114">Contém o identificador e a chave de alteração de uma pasta de destino para operações que atualizam, enviam e criam itens no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="12342-114">Contains the identifier and change key of a target folder for operations that update, send, and create items in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="12342-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="12342-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="12342-116">Identifica uma pasta de destino por um identificador nomeado para operações que atualizam, enviam e criam itens no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="12342-116">Identifies a target folder by a named identifier for operations that update, send, and create items in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="12342-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="12342-117">Parent elements</span></span>

|<span data-ttu-id="12342-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="12342-118">**Element**</span></span>|<span data-ttu-id="12342-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="12342-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="12342-120">CreateItem</span><span class="sxs-lookup"><span data-stu-id="12342-120">CreateItem</span></span>](createitem.md) <br/> |<span data-ttu-id="12342-121">Define uma solicitação para criar um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="12342-121">Defines a request to create an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="12342-122">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="12342-122">The following is the XPath expression to this element:</span></span>  <br/>  `/CreateItem` <br/> |
|[<span data-ttu-id="12342-123">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="12342-123">UpdateItem</span></span>](updateitem.md) <br/> |<span data-ttu-id="12342-124">Define uma solicitação para atualizar um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="12342-124">Defines a request to update an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="12342-125">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="12342-125">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateItem` <br/> |
|[<span data-ttu-id="12342-126">SendItem</span><span class="sxs-lookup"><span data-stu-id="12342-126">SendItem</span></span>](senditem.md) <br/> |<span data-ttu-id="12342-127">Define uma solicitação para enviar um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="12342-127">Defines a request to send an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="12342-128">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="12342-128">The following is the XPath expression to this element:</span></span>  <br/>  `/SendItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="12342-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="12342-129">Remarks</span></span>

<span data-ttu-id="12342-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="12342-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="12342-131">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="12342-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="12342-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="12342-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="12342-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="12342-133">Schema Name</span></span>  <br/> |<span data-ttu-id="12342-134">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="12342-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="12342-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="12342-135">Validation File</span></span>  <br/> |<span data-ttu-id="12342-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="12342-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="12342-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="12342-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="12342-138">Falso</span><span class="sxs-lookup"><span data-stu-id="12342-138">False</span></span>  <br/> |
   

