---
title: IndexedPageFolderView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IndexedPageFolderView
api_type:
- schema
ms.assetid: c6dac232-244b-4db0-9a15-5e01b8aa7a7d
description: O elemento IndexedPageFolderView descreve como paginados informações de item são retornados em uma resposta FindFolder.
ms.openlocfilehash: f32f778daa6fa3fea93ab2bc1951f2407dcf7f80
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823910"
---
# <a name="indexedpagefolderview"></a><span data-ttu-id="7e1d3-103">IndexedPageFolderView</span><span class="sxs-lookup"><span data-stu-id="7e1d3-103">IndexedPageFolderView</span></span>

<span data-ttu-id="7e1d3-104">O elemento **IndexedPageFolderView** descreve como paginados informações de item são retornados em uma resposta [FindFolder](findfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="7e1d3-104">The **IndexedPageFolderView** element describes how paged item information is returned in a [FindFolder](findfolder.md) response.</span></span> 
  
[<span data-ttu-id="7e1d3-105">FindFolder</span><span class="sxs-lookup"><span data-stu-id="7e1d3-105">FindFolder</span></span>](findfolder.md)
  
[<span data-ttu-id="7e1d3-106">IndexedPageFolderView</span><span class="sxs-lookup"><span data-stu-id="7e1d3-106">IndexedPageFolderView</span></span>](indexedpagefolderview.md)
  
```xml
<IndexedPageFolderView MaxEntriesReturned="" Offset="" BasePoint="" />
```

 <span data-ttu-id="7e1d3-107">**IndexedPageViewType**</span><span class="sxs-lookup"><span data-stu-id="7e1d3-107">**IndexedPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7e1d3-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="7e1d3-108">Attributes and elements</span></span>

<span data-ttu-id="7e1d3-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7e1d3-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e1d3-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="7e1d3-110">Attributes</span></span>

|<span data-ttu-id="7e1d3-111">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="7e1d3-111">**Attribute**</span></span>|<span data-ttu-id="7e1d3-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7e1d3-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7e1d3-113">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="7e1d3-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="7e1d3-114">Descreve o número máximo de pastas para retornar na resposta.</span><span class="sxs-lookup"><span data-stu-id="7e1d3-114">Describes the maximum number of folders to return in the response.</span></span> <span data-ttu-id="7e1d3-115">Este atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="7e1d3-115">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="7e1d3-116">**Offset**</span><span class="sxs-lookup"><span data-stu-id="7e1d3-116">**Offset**</span></span> <br/> |<span data-ttu-id="7e1d3-117">Descreve o deslocamento, desde o **ponto de base**.</span><span class="sxs-lookup"><span data-stu-id="7e1d3-117">Describes the offset from the **BasePoint**.</span></span> <span data-ttu-id="7e1d3-118">Deslocamento deve ser maior ou igual a zero.</span><span class="sxs-lookup"><span data-stu-id="7e1d3-118">Offset must be greater than or equal to zero.</span></span> <span data-ttu-id="7e1d3-119">Se o **ponto de base** é igual ao início, o deslocamento for positivo.</span><span class="sxs-lookup"><span data-stu-id="7e1d3-119">If **BasePoint** is equal to Beginning, the offset is positive.</span></span> <span data-ttu-id="7e1d3-120">Se o **ponto de base** for igual ao fim, o deslocamento é tratado como se fosse negativo.</span><span class="sxs-lookup"><span data-stu-id="7e1d3-120">If **BasePoint** is equal to End, the offset is handled as if it were negative.</span></span>  <br/> <span data-ttu-id="7e1d3-121">Isso identifica a pasta na qual será a primeira pasta entregue na resposta.</span><span class="sxs-lookup"><span data-stu-id="7e1d3-121">This identifies which folder will be the first folder delivered in the response.</span></span> <span data-ttu-id="7e1d3-122">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="7e1d3-122">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="7e1d3-123">**Ponto de base**</span><span class="sxs-lookup"><span data-stu-id="7e1d3-123">**BasePoint**</span></span> <br/> |<span data-ttu-id="7e1d3-124">Descreve como se a página de pastas será iniciado a partir do início ou no final do conjunto de pastas que são localizadas com os critérios de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="7e1d3-124">Describes whether the page of folders will start from the start or the end of the set of folders that are found with the search criteria.</span></span> <span data-ttu-id="7e1d3-125">Procurando a partir do término do sempre pesquisa para trás.</span><span class="sxs-lookup"><span data-stu-id="7e1d3-125">Seeking from the end always searches backward.</span></span> <span data-ttu-id="7e1d3-126">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="7e1d3-126">This attribute is required.</span></span>  <br/> |
   
#### <a name="basepoint-attribute"></a><span data-ttu-id="7e1d3-127">Atributo de ponto de base</span><span class="sxs-lookup"><span data-stu-id="7e1d3-127">BasePoint Attribute</span></span>

|<span data-ttu-id="7e1d3-128">**Valor**</span><span class="sxs-lookup"><span data-stu-id="7e1d3-128">**Value**</span></span>|<span data-ttu-id="7e1d3-129">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7e1d3-129">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7e1d3-130">Início</span><span class="sxs-lookup"><span data-stu-id="7e1d3-130">Beginning</span></span>  <br/> |<span data-ttu-id="7e1d3-131">O modo de exibição paginado começa no início do conjunto de pasta encontrado.</span><span class="sxs-lookup"><span data-stu-id="7e1d3-131">The paged view starts at the beginning of the found folder set.</span></span>  <br/> |
|<span data-ttu-id="7e1d3-132">End</span><span class="sxs-lookup"><span data-stu-id="7e1d3-132">End</span></span>  <br/> |<span data-ttu-id="7e1d3-133">O modo de exibição paginado inicia no final do conjunto de pasta encontrado.</span><span class="sxs-lookup"><span data-stu-id="7e1d3-133">The paged view starts at the end of the found folder set.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7e1d3-134">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7e1d3-134">Child elements</span></span>

<span data-ttu-id="7e1d3-135">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7e1d3-135">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7e1d3-136">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7e1d3-136">Parent elements</span></span>

|<span data-ttu-id="7e1d3-137">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7e1d3-137">**Element**</span></span>|<span data-ttu-id="7e1d3-138">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7e1d3-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e1d3-139">FindFolder</span><span class="sxs-lookup"><span data-stu-id="7e1d3-139">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="7e1d3-140">Define uma solicitação para localizar pastas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7e1d3-140">Defines a request to find folders in a mailbox.</span></span>  <br/> <span data-ttu-id="7e1d3-141">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="7e1d3-141">The following is the XPath expression to this element:</span></span>  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7e1d3-142">Comentários</span><span class="sxs-lookup"><span data-stu-id="7e1d3-142">Remarks</span></span>

<span data-ttu-id="7e1d3-143">Buscando a partir do término envolve mover para a origem identificada pelo deslocamento.</span><span class="sxs-lookup"><span data-stu-id="7e1d3-143">Seeking from end involves moving to the origin identified by the offset.</span></span> <span data-ttu-id="7e1d3-144">Além disso, o ponteiro é movido de volta pelo número de registros solicitados.</span><span class="sxs-lookup"><span data-stu-id="7e1d3-144">Additionally, the pointer is moved back by the number of requested records.</span></span> <span data-ttu-id="7e1d3-145">Por exemplo, se existem 100 registros e o deslocamento for 25 do fim, a pesquisa começa a partir 75.</span><span class="sxs-lookup"><span data-stu-id="7e1d3-145">For example, if there are 100 records and the offset is 25 from the end, the search starts from 75.</span></span> <span data-ttu-id="7e1d3-146">Se 10 registros forem retornados, o ponteiro é movido para trás uma 10 adicionais registra como 65 e retorna registros 65 por meio de 75.</span><span class="sxs-lookup"><span data-stu-id="7e1d3-146">If 10 records are returned, the pointer is moved backward an additional 10 records to 65 and returns records 65 through 75.</span></span> <span data-ttu-id="7e1d3-147">O próximo índice é 64.</span><span class="sxs-lookup"><span data-stu-id="7e1d3-147">The next index is 64.</span></span> <span data-ttu-id="7e1d3-148">O deslocamento próximo do final de uma página é 100 menos 64 que é igual a 36.</span><span class="sxs-lookup"><span data-stu-id="7e1d3-148">The next offset from the end for a page is 100 minus 64 which equals 36.</span></span> <span data-ttu-id="7e1d3-149">O valor para o próximo deslocamento do final para obter a próxima página indexada é 36.</span><span class="sxs-lookup"><span data-stu-id="7e1d3-149">The value for the next offset from the end to get the next indexed page is 36.</span></span>
  
<span data-ttu-id="7e1d3-150">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="7e1d3-150">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7e1d3-151">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="7e1d3-151">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e1d3-152">Namespace</span><span class="sxs-lookup"><span data-stu-id="7e1d3-152">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7e1d3-153">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7e1d3-153">Schema Name</span></span>  <br/> |<span data-ttu-id="7e1d3-154">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="7e1d3-154">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7e1d3-155">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7e1d3-155">Validation File</span></span>  <br/> |<span data-ttu-id="7e1d3-156">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7e1d3-156">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7e1d3-157">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="7e1d3-157">Can be Empty</span></span>  <br/> |<span data-ttu-id="7e1d3-158">False</span><span class="sxs-lookup"><span data-stu-id="7e1d3-158">False</span></span>  <br/> |
   

