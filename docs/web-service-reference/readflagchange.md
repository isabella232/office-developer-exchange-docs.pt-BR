---
title: ReadFlagChange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReadFlagChange
api_type:
- schema
ms.assetid: 527bfe90-63d0-4b2f-97f7-7875b3a516b2
description: O elemento ReadFlagChange é retornado em respostas de operação SyncFolderItems quando um item foi lido. Essa propriedade é somente leitura.
ms.openlocfilehash: 354f8085a6ea5b738d8619e2ffeb0fbccefd51da
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468303"
---
# <a name="readflagchange"></a><span data-ttu-id="25a00-104">ReadFlagChange</span><span class="sxs-lookup"><span data-stu-id="25a00-104">ReadFlagChange</span></span>

<span data-ttu-id="25a00-105">O elemento **ReadFlagChange** é retornado em respostas de [operação SyncFolderItems](syncfolderitems-operation.md) quando um item foi lido.</span><span class="sxs-lookup"><span data-stu-id="25a00-105">The **ReadFlagChange** element is returned in [SyncFolderItems operation](syncfolderitems-operation.md) responses when an item has been read.</span></span> <span data-ttu-id="25a00-106">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25a00-106">This property is read-only.</span></span> 
  
```xml
<ReadFlagChange>
   <ItemId/>
   <IsRead/>
</ReadFlagChange>
```

 <span data-ttu-id="25a00-107">**SyncFolderItemsReadFlagType**</span><span class="sxs-lookup"><span data-stu-id="25a00-107">**SyncFolderItemsReadFlagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="25a00-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="25a00-108">Attributes and elements</span></span>

<span data-ttu-id="25a00-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="25a00-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="25a00-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="25a00-110">Attributes</span></span>

<span data-ttu-id="25a00-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="25a00-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="25a00-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="25a00-112">Child elements</span></span>

|<span data-ttu-id="25a00-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="25a00-113">**Element**</span></span>|<span data-ttu-id="25a00-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="25a00-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="25a00-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="25a00-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="25a00-116">Identifica o item para o qual o sinalizador de leitura foi alterado.</span><span class="sxs-lookup"><span data-stu-id="25a00-116">Identifies the item for which the read-flag has been changed.</span></span>  <br/> |
|[<span data-ttu-id="25a00-117">IsRead</span><span class="sxs-lookup"><span data-stu-id="25a00-117">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="25a00-118">Indica se o sinalizador de leitura foi definido como **true**.</span><span class="sxs-lookup"><span data-stu-id="25a00-118">Indicates whether the read-flag has been set to **true**.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="25a00-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="25a00-119">Parent elements</span></span>

|<span data-ttu-id="25a00-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="25a00-120">**Element**</span></span>|<span data-ttu-id="25a00-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="25a00-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="25a00-122">Alterações (itens)</span><span class="sxs-lookup"><span data-stu-id="25a00-122">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="25a00-123">Contém uma matriz de sequência de tipos de alteração que representam os tipos de diferenças entre os itens no cliente e os itens no servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="25a00-123">Contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="25a00-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="25a00-124">Remarks</span></span>

<span data-ttu-id="25a00-125">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="25a00-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="25a00-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="25a00-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="25a00-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="25a00-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="25a00-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="25a00-128">Schema Name</span></span>  <br/> |<span data-ttu-id="25a00-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="25a00-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="25a00-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="25a00-130">Validation File</span></span>  <br/> |<span data-ttu-id="25a00-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="25a00-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="25a00-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="25a00-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="25a00-133">False</span><span class="sxs-lookup"><span data-stu-id="25a00-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="25a00-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="25a00-134">See also</span></span>



- [<span data-ttu-id="25a00-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="25a00-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

