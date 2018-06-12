---
title: BaseFolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BaseFolderIds
api_type:
- schema
ms.assetid: bdaa6093-f960-469a-b338-0e75aaa536c6
description: O elemento BaseFolderIds representa a coleção das pastas que serão extraídos para determinar o conteúdo de uma pasta de pesquisa.
ms.openlocfilehash: 960e4d9c1d6eb37bf988bf163e696cbba3e1ef6f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751250"
---
# <a name="basefolderids"></a><span data-ttu-id="0121b-103">BaseFolderIds</span><span class="sxs-lookup"><span data-stu-id="0121b-103">BaseFolderIds</span></span>

<span data-ttu-id="0121b-104">O elemento **BaseFolderIds** representa a coleção das pastas que serão extraídos para determinar o conteúdo de uma pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="0121b-104">The **BaseFolderIds** element represents the collection of folders that will be mined to determine the contents of a search folder.</span></span> 
  
```xml
<BaseFolderIds>
   <FolderId/>
   <DistinguishedFolderId/>
</BaseFolderIds>
```

 <span data-ttu-id="0121b-105">**NonEmptyArrayOfBaseFolderIdsType**</span><span class="sxs-lookup"><span data-stu-id="0121b-105">**NonEmptyArrayOfBaseFolderIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0121b-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="0121b-106">Attributes and elements</span></span>

<span data-ttu-id="0121b-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0121b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0121b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0121b-108">Attributes</span></span>

<span data-ttu-id="0121b-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0121b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0121b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0121b-110">Child elements</span></span>

|<span data-ttu-id="0121b-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0121b-111">**Element**</span></span>|<span data-ttu-id="0121b-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0121b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0121b-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="0121b-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="0121b-114">Contém o identificador e alterar a chave de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="0121b-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="0121b-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="0121b-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="0121b-116">Identifica as pastas de MicrosoftExchange Server 2007 que podem ser referidas por nome.</span><span class="sxs-lookup"><span data-stu-id="0121b-116">Identifies MicrosoftExchange Server 2007 folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0121b-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0121b-117">Parent elements</span></span>

|<span data-ttu-id="0121b-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0121b-118">**Element**</span></span>|<span data-ttu-id="0121b-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0121b-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0121b-120">SearchParameters</span><span class="sxs-lookup"><span data-stu-id="0121b-120">SearchParameters</span></span>](searchparameters.md) <br/> |<span data-ttu-id="0121b-121">Representa os parâmetros que definem a uma pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="0121b-121">Represents the parameters that define a search folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0121b-122">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="0121b-122">Remarks</span></span>

<span data-ttu-id="0121b-123">O elemento **BaseFolderIds** deve conter pelo menos um elemento [FolderId](folderid.md) ou [DistinguishedFolderId](distinguishedfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="0121b-123">The **BaseFolderIds** element must contain at least one [FolderId](folderid.md) or [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span> 
  
<span data-ttu-id="0121b-124">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="0121b-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0121b-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="0121b-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0121b-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="0121b-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0121b-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0121b-127">Schema name</span></span>  <br/> |<span data-ttu-id="0121b-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="0121b-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="0121b-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0121b-129">Validation file</span></span>  <br/> |<span data-ttu-id="0121b-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0121b-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0121b-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="0121b-131">Can be empty</span></span>  <br/> |<span data-ttu-id="0121b-132">False</span><span class="sxs-lookup"><span data-stu-id="0121b-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0121b-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="0121b-133">See also</span></span>



- [<span data-ttu-id="0121b-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0121b-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

