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
description: O elemento SearchParameters representa os parâmetros que definem a uma pasta de pesquisa.
ms.openlocfilehash: b534574a1292d78c8df99f5186990b114fc4e70a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825299"
---
# <a name="searchparameters"></a><span data-ttu-id="55f7e-103">SearchParameters</span><span class="sxs-lookup"><span data-stu-id="55f7e-103">SearchParameters</span></span>

<span data-ttu-id="55f7e-104">O elemento **SearchParameters** representa os parâmetros que definem a uma pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="55f7e-104">The **SearchParameters** element represents the parameters that define a search folder.</span></span> 
  
```xml
<SearchParameters Traversal="">
   <Restriction/>
   <BaseFolderIds/>
</SearchParameters>
```

 <span data-ttu-id="55f7e-105">**SearchParametersType**</span><span class="sxs-lookup"><span data-stu-id="55f7e-105">**SearchParametersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="55f7e-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="55f7e-106">Attributes and elements</span></span>

<span data-ttu-id="55f7e-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="55f7e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="55f7e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="55f7e-108">Attributes</span></span>

|<span data-ttu-id="55f7e-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="55f7e-109">**Attribute**</span></span>|<span data-ttu-id="55f7e-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="55f7e-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="55f7e-111">**Passagem**</span><span class="sxs-lookup"><span data-stu-id="55f7e-111">**Traversal**</span></span> <br/> |<span data-ttu-id="55f7e-112">Descreve como uma pasta de pesquisa percorre a hierarquia de pastas.</span><span class="sxs-lookup"><span data-stu-id="55f7e-112">Describes how a search folder traverses the folder hierarchy.</span></span> <span data-ttu-id="55f7e-113">As opções são para uma pesquisa **superficial** ou uma **profundidade** .</span><span class="sxs-lookup"><span data-stu-id="55f7e-113">The options are for either a **Deep** or a **Shallow** search.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="55f7e-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="55f7e-114">Child elements</span></span>

|<span data-ttu-id="55f7e-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="55f7e-115">**Element**</span></span>|<span data-ttu-id="55f7e-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="55f7e-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55f7e-117">Restriction</span><span class="sxs-lookup"><span data-stu-id="55f7e-117">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="55f7e-118">Representa a restrição ou a consulta que é usada para filtrar itens ou pastas nas operações da pasta FindItem/FindFolder e pesquisa.</span><span class="sxs-lookup"><span data-stu-id="55f7e-118">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="55f7e-119">BaseFolderIds</span><span class="sxs-lookup"><span data-stu-id="55f7e-119">BaseFolderIds</span></span>](basefolderids.md) <br/> |<span data-ttu-id="55f7e-120">Representa a coleção das pastas que serão extraídos para determinar o conteúdo de uma pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="55f7e-120">Represents the collection of folders that will be mined to determine the contents of a search folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="55f7e-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="55f7e-121">Parent elements</span></span>

|<span data-ttu-id="55f7e-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="55f7e-122">**Element**</span></span>|<span data-ttu-id="55f7e-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="55f7e-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55f7e-124">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="55f7e-124">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="55f7e-125">Representa uma pasta de pesquisa que está contida em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="55f7e-125">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="55f7e-126">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="55f7e-126">Remarks</span></span>

<span data-ttu-id="55f7e-127">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="55f7e-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="55f7e-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="55f7e-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="55f7e-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="55f7e-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="55f7e-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="55f7e-130">Schema Name</span></span>  <br/> |<span data-ttu-id="55f7e-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="55f7e-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="55f7e-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="55f7e-132">Validation File</span></span>  <br/> |<span data-ttu-id="55f7e-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="55f7e-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="55f7e-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="55f7e-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="55f7e-135">False</span><span class="sxs-lookup"><span data-stu-id="55f7e-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="55f7e-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="55f7e-136">See also</span></span>



- [<span data-ttu-id="55f7e-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="55f7e-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

