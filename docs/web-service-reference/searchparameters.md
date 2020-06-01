---
title: SearchParameters
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SearchParameters
api_type:
- schema
ms.assetid: 34602cb1-dc33-4552-a98c-3e77f614daa3
description: O elemento SearchParameters representa os parâmetros que definem uma pasta de pesquisa.
ms.openlocfilehash: cd9f255621b17d01113392e67a0301b01b70f326
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466665"
---
# <a name="searchparameters"></a><span data-ttu-id="6dd25-103">SearchParameters</span><span class="sxs-lookup"><span data-stu-id="6dd25-103">SearchParameters</span></span>

<span data-ttu-id="6dd25-104">O elemento **SearchParameters** representa os parâmetros que definem uma pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="6dd25-104">The **SearchParameters** element represents the parameters that define a search folder.</span></span> 
  
```xml
<SearchParameters Traversal="">
   <Restriction/>
   <BaseFolderIds/>
</SearchParameters>
```

 <span data-ttu-id="6dd25-105">**SearchParametersType**</span><span class="sxs-lookup"><span data-stu-id="6dd25-105">**SearchParametersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6dd25-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="6dd25-106">Attributes and elements</span></span>

<span data-ttu-id="6dd25-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6dd25-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6dd25-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="6dd25-108">Attributes</span></span>

|<span data-ttu-id="6dd25-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="6dd25-109">**Attribute**</span></span>|<span data-ttu-id="6dd25-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6dd25-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6dd25-111">**Passagem**</span><span class="sxs-lookup"><span data-stu-id="6dd25-111">**Traversal**</span></span> <br/> |<span data-ttu-id="6dd25-112">Descreve como uma pasta de pesquisa atravessa a hierarquia de pastas.</span><span class="sxs-lookup"><span data-stu-id="6dd25-112">Describes how a search folder traverses the folder hierarchy.</span></span> <span data-ttu-id="6dd25-113">As opções são para uma pesquisa **profunda** ou **superficial** .</span><span class="sxs-lookup"><span data-stu-id="6dd25-113">The options are for either a **Deep** or a **Shallow** search.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6dd25-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6dd25-114">Child elements</span></span>

|<span data-ttu-id="6dd25-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6dd25-115">**Element**</span></span>|<span data-ttu-id="6dd25-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6dd25-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6dd25-117">Restriction</span><span class="sxs-lookup"><span data-stu-id="6dd25-117">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="6dd25-118">Representa a restrição ou a consulta usada para filtrar itens ou pastas no FindItem/FindFolder e operações de pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="6dd25-118">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="6dd25-119">BaseFolderIds</span><span class="sxs-lookup"><span data-stu-id="6dd25-119">BaseFolderIds</span></span>](basefolderids.md) <br/> |<span data-ttu-id="6dd25-120">Representa a coleção de pastas que será minada para determinar o conteúdo de uma pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="6dd25-120">Represents the collection of folders that will be mined to determine the contents of a search folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6dd25-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6dd25-121">Parent elements</span></span>

|<span data-ttu-id="6dd25-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6dd25-122">**Element**</span></span>|<span data-ttu-id="6dd25-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6dd25-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6dd25-124">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="6dd25-124">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="6dd25-125">Representa uma pasta de pesquisa que está contida em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6dd25-125">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6dd25-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="6dd25-126">Remarks</span></span>

<span data-ttu-id="6dd25-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="6dd25-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6dd25-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="6dd25-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6dd25-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="6dd25-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6dd25-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6dd25-130">Schema Name</span></span>  <br/> |<span data-ttu-id="6dd25-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="6dd25-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="6dd25-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6dd25-132">Validation File</span></span>  <br/> |<span data-ttu-id="6dd25-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="6dd25-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6dd25-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6dd25-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="6dd25-135">False</span><span class="sxs-lookup"><span data-stu-id="6dd25-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6dd25-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="6dd25-136">See also</span></span>



- [<span data-ttu-id="6dd25-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6dd25-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

