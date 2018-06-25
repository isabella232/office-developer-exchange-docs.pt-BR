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
description: O elemento ReadFlagChange é retornado em SyncFolderItems respostas da operação quando um item foi lido. Esta propriedade é somente leitura.
ms.openlocfilehash: 28ef0267e8308ba58057bec01ab2672a19ee94a1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824953"
---
# <a name="readflagchange"></a><span data-ttu-id="b91a5-104">ReadFlagChange</span><span class="sxs-lookup"><span data-stu-id="b91a5-104">ReadFlagChange</span></span>

<span data-ttu-id="b91a5-105">O elemento **ReadFlagChange** é retornado em [operação SyncFolderItems](syncfolderitems-operation.md) respostas quando um item foi lido.</span><span class="sxs-lookup"><span data-stu-id="b91a5-105">The **ReadFlagChange** element is returned in [SyncFolderItems operation](syncfolderitems-operation.md) responses when an item has been read.</span></span> <span data-ttu-id="b91a5-106">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b91a5-106">This property is read-only.</span></span> 
  
```xml
<ReadFlagChange>
   <ItemId/>
   <IsRead/>
</ReadFlagChange>
```

 <span data-ttu-id="b91a5-107">**SyncFolderItemsReadFlagType**</span><span class="sxs-lookup"><span data-stu-id="b91a5-107">**SyncFolderItemsReadFlagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b91a5-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b91a5-108">Attributes and elements</span></span>

<span data-ttu-id="b91a5-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b91a5-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b91a5-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="b91a5-110">Attributes</span></span>

<span data-ttu-id="b91a5-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b91a5-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b91a5-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b91a5-112">Child elements</span></span>

|<span data-ttu-id="b91a5-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b91a5-113">**Element**</span></span>|<span data-ttu-id="b91a5-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b91a5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b91a5-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="b91a5-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="b91a5-116">Identifica o item para o qual o sinalizador de leitura tiver sido alterado.</span><span class="sxs-lookup"><span data-stu-id="b91a5-116">Identifies the item for which the read-flag has been changed.</span></span>  <br/> |
|[<span data-ttu-id="b91a5-117">Foi lido</span><span class="sxs-lookup"><span data-stu-id="b91a5-117">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="b91a5-118">Indica se o sinalizador de leitura tiver sido definido como **true**.</span><span class="sxs-lookup"><span data-stu-id="b91a5-118">Indicates whether the read-flag has been set to **true**.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b91a5-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b91a5-119">Parent elements</span></span>

|<span data-ttu-id="b91a5-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b91a5-120">**Element**</span></span>|<span data-ttu-id="b91a5-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b91a5-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b91a5-122">Alterações (itens)</span><span class="sxs-lookup"><span data-stu-id="b91a5-122">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="b91a5-123">Contém uma matriz de sequência de tipos de alteração que representam os tipos de diferenças entre os itens no cliente e os itens no servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="b91a5-123">Contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b91a5-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="b91a5-124">Remarks</span></span>

<span data-ttu-id="b91a5-125">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="b91a5-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b91a5-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b91a5-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b91a5-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="b91a5-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b91a5-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b91a5-128">Schema Name</span></span>  <br/> |<span data-ttu-id="b91a5-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b91a5-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="b91a5-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b91a5-130">Validation File</span></span>  <br/> |<span data-ttu-id="b91a5-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b91a5-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b91a5-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b91a5-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="b91a5-133">False</span><span class="sxs-lookup"><span data-stu-id="b91a5-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b91a5-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="b91a5-134">See also</span></span>



- [<span data-ttu-id="b91a5-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b91a5-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

