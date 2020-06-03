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
description: O elemento BaseFolderIds representa a coleção de pastas que será minada para determinar o conteúdo de uma pasta de pesquisa.
ms.openlocfilehash: 97159ec1ded685e63aafedfaf90a06eff39adaab
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460264"
---
# <a name="basefolderids"></a><span data-ttu-id="9b1ab-103">BaseFolderIds</span><span class="sxs-lookup"><span data-stu-id="9b1ab-103">BaseFolderIds</span></span>

<span data-ttu-id="9b1ab-104">O elemento **BaseFolderIds** representa a coleção de pastas que será minada para determinar o conteúdo de uma pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="9b1ab-104">The **BaseFolderIds** element represents the collection of folders that will be mined to determine the contents of a search folder.</span></span> 
  
```xml
<BaseFolderIds>
   <FolderId/>
   <DistinguishedFolderId/>
</BaseFolderIds>
```

 <span data-ttu-id="9b1ab-105">**NonEmptyArrayOfBaseFolderIdsType**</span><span class="sxs-lookup"><span data-stu-id="9b1ab-105">**NonEmptyArrayOfBaseFolderIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9b1ab-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="9b1ab-106">Attributes and elements</span></span>

<span data-ttu-id="9b1ab-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9b1ab-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9b1ab-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9b1ab-108">Attributes</span></span>

<span data-ttu-id="9b1ab-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9b1ab-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9b1ab-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9b1ab-110">Child elements</span></span>

|<span data-ttu-id="9b1ab-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9b1ab-111">**Element**</span></span>|<span data-ttu-id="9b1ab-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9b1ab-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b1ab-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="9b1ab-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="9b1ab-114">Contém o identificador e a chave de alteração de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="9b1ab-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="9b1ab-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="9b1ab-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="9b1ab-116">Identifica as pastas do MicrosoftExchange Server 2007 que podem ser referenciadas por nome.</span><span class="sxs-lookup"><span data-stu-id="9b1ab-116">Identifies MicrosoftExchange Server 2007 folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9b1ab-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9b1ab-117">Parent elements</span></span>

|<span data-ttu-id="9b1ab-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9b1ab-118">**Element**</span></span>|<span data-ttu-id="9b1ab-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9b1ab-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b1ab-120">SearchParameters</span><span class="sxs-lookup"><span data-stu-id="9b1ab-120">SearchParameters</span></span>](searchparameters.md) <br/> |<span data-ttu-id="9b1ab-121">Representa os parâmetros que definem uma pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="9b1ab-121">Represents the parameters that define a search folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9b1ab-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="9b1ab-122">Remarks</span></span>

<span data-ttu-id="9b1ab-123">O elemento **BaseFolderIds** deve conter pelo menos um elemento [FolderId](folderid.md) ou [DistinguishedFolderId](distinguishedfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="9b1ab-123">The **BaseFolderIds** element must contain at least one [FolderId](folderid.md) or [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span> 
  
<span data-ttu-id="9b1ab-124">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="9b1ab-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9b1ab-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="9b1ab-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9b1ab-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="9b1ab-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9b1ab-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9b1ab-127">Schema name</span></span>  <br/> |<span data-ttu-id="9b1ab-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="9b1ab-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="9b1ab-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9b1ab-129">Validation file</span></span>  <br/> |<span data-ttu-id="9b1ab-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9b1ab-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9b1ab-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="9b1ab-131">Can be empty</span></span>  <br/> |<span data-ttu-id="9b1ab-132">False</span><span class="sxs-lookup"><span data-stu-id="9b1ab-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9b1ab-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="9b1ab-133">See also</span></span>



- [<span data-ttu-id="9b1ab-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9b1ab-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

