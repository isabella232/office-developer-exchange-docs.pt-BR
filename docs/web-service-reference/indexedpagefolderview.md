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
description: O elemento IndexedPageFolderView descreve como as informações de item paginado são retornadas em uma resposta FindFolder.
ms.openlocfilehash: 6e9e2796c0bdcd9a15487f0e1bc7cbdf09d0a492
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457197"
---
# <a name="indexedpagefolderview"></a><span data-ttu-id="e069d-103">IndexedPageFolderView</span><span class="sxs-lookup"><span data-stu-id="e069d-103">IndexedPageFolderView</span></span>

<span data-ttu-id="e069d-104">O elemento **IndexedPageFolderView** descreve como as informações de item paginado são retornadas em uma resposta [FindFolder](findfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="e069d-104">The **IndexedPageFolderView** element describes how paged item information is returned in a [FindFolder](findfolder.md) response.</span></span> 
  
[<span data-ttu-id="e069d-105">FindFolder</span><span class="sxs-lookup"><span data-stu-id="e069d-105">FindFolder</span></span>](findfolder.md)
  
[<span data-ttu-id="e069d-106">IndexedPageFolderView</span><span class="sxs-lookup"><span data-stu-id="e069d-106">IndexedPageFolderView</span></span>](indexedpagefolderview.md)
  
```xml
<IndexedPageFolderView MaxEntriesReturned="" Offset="" BasePoint="" />
```

 <span data-ttu-id="e069d-107">**IndexedPageViewType**</span><span class="sxs-lookup"><span data-stu-id="e069d-107">**IndexedPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e069d-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e069d-108">Attributes and elements</span></span>

<span data-ttu-id="e069d-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e069d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e069d-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="e069d-110">Attributes</span></span>

|<span data-ttu-id="e069d-111">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="e069d-111">**Attribute**</span></span>|<span data-ttu-id="e069d-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e069d-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e069d-113">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="e069d-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="e069d-114">Descreve o número máximo de pastas a serem retornadas na resposta.</span><span class="sxs-lookup"><span data-stu-id="e069d-114">Describes the maximum number of folders to return in the response.</span></span> <span data-ttu-id="e069d-115">Esse atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="e069d-115">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="e069d-116">**Offset**</span><span class="sxs-lookup"><span data-stu-id="e069d-116">**Offset**</span></span> <br/> |<span data-ttu-id="e069d-117">Descreve o deslocamento do **BasePoint**.</span><span class="sxs-lookup"><span data-stu-id="e069d-117">Describes the offset from the **BasePoint**.</span></span> <span data-ttu-id="e069d-118">Offset deve ser maior ou igual a zero.</span><span class="sxs-lookup"><span data-stu-id="e069d-118">Offset must be greater than or equal to zero.</span></span> <span data-ttu-id="e069d-119">Se **BasePoint** for igual a início, o deslocamento será positivo.</span><span class="sxs-lookup"><span data-stu-id="e069d-119">If **BasePoint** is equal to Beginning, the offset is positive.</span></span> <span data-ttu-id="e069d-120">Se **BasePoint** for igual a end, o deslocamento será tratado como se fosse negativo.</span><span class="sxs-lookup"><span data-stu-id="e069d-120">If **BasePoint** is equal to End, the offset is handled as if it were negative.</span></span>  <br/> <span data-ttu-id="e069d-121">Isso identifica qual pasta será a primeira pasta entregue na resposta.</span><span class="sxs-lookup"><span data-stu-id="e069d-121">This identifies which folder will be the first folder delivered in the response.</span></span> <span data-ttu-id="e069d-122">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="e069d-122">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="e069d-123">**BasePoint**</span><span class="sxs-lookup"><span data-stu-id="e069d-123">**BasePoint**</span></span> <br/> |<span data-ttu-id="e069d-124">Descreve se a página de pastas será iniciada a partir do início ou do final do conjunto de pastas encontrado com os critérios de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="e069d-124">Describes whether the page of folders will start from the start or the end of the set of folders that are found with the search criteria.</span></span> <span data-ttu-id="e069d-125">Procurar a partir do fim sempre pesquisa retroativamente.</span><span class="sxs-lookup"><span data-stu-id="e069d-125">Seeking from the end always searches backward.</span></span> <span data-ttu-id="e069d-126">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="e069d-126">This attribute is required.</span></span>  <br/> |
   
#### <a name="basepoint-attribute"></a><span data-ttu-id="e069d-127">Atributo BasePoint</span><span class="sxs-lookup"><span data-stu-id="e069d-127">BasePoint Attribute</span></span>

|<span data-ttu-id="e069d-128">**Valor**</span><span class="sxs-lookup"><span data-stu-id="e069d-128">**Value**</span></span>|<span data-ttu-id="e069d-129">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e069d-129">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e069d-130">Extremidade</span><span class="sxs-lookup"><span data-stu-id="e069d-130">Beginning</span></span>  <br/> |<span data-ttu-id="e069d-131">O modo de exibição paginado começa no início do conjunto de pastas localizado.</span><span class="sxs-lookup"><span data-stu-id="e069d-131">The paged view starts at the beginning of the found folder set.</span></span>  <br/> |
|<span data-ttu-id="e069d-132">Final</span><span class="sxs-lookup"><span data-stu-id="e069d-132">End</span></span>  <br/> |<span data-ttu-id="e069d-133">O modo de exibição paginado começa no final do conjunto de pastas encontrado.</span><span class="sxs-lookup"><span data-stu-id="e069d-133">The paged view starts at the end of the found folder set.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e069d-134">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e069d-134">Child elements</span></span>

<span data-ttu-id="e069d-135">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e069d-135">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e069d-136">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e069d-136">Parent elements</span></span>

|<span data-ttu-id="e069d-137">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e069d-137">**Element**</span></span>|<span data-ttu-id="e069d-138">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e069d-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e069d-139">FindFolder</span><span class="sxs-lookup"><span data-stu-id="e069d-139">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="e069d-140">Define uma solicitação para localizar pastas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e069d-140">Defines a request to find folders in a mailbox.</span></span>  <br/> <span data-ttu-id="e069d-141">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="e069d-141">The following is the XPath expression to this element:</span></span>  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e069d-142">Comentários</span><span class="sxs-lookup"><span data-stu-id="e069d-142">Remarks</span></span>

<span data-ttu-id="e069d-143">Procurar de end envolve mover para a origem identificada pelo deslocamento.</span><span class="sxs-lookup"><span data-stu-id="e069d-143">Seeking from end involves moving to the origin identified by the offset.</span></span> <span data-ttu-id="e069d-144">Além disso, o ponteiro é movido de volta pelo número de registros solicitados.</span><span class="sxs-lookup"><span data-stu-id="e069d-144">Additionally, the pointer is moved back by the number of requested records.</span></span> <span data-ttu-id="e069d-145">Por exemplo, se houver 100 registros e o deslocamento for 25 a partir do final, a pesquisa iniciará de 75.</span><span class="sxs-lookup"><span data-stu-id="e069d-145">For example, if there are 100 records and the offset is 25 from the end, the search starts from 75.</span></span> <span data-ttu-id="e069d-146">Se 10 registros forem retornados, o ponteiro será movido para trás de 10 registros adicionais para 65 e retornará os registros 65 a 75.</span><span class="sxs-lookup"><span data-stu-id="e069d-146">If 10 records are returned, the pointer is moved backward an additional 10 records to 65 and returns records 65 through 75.</span></span> <span data-ttu-id="e069d-147">O próximo índice é 64.</span><span class="sxs-lookup"><span data-stu-id="e069d-147">The next index is 64.</span></span> <span data-ttu-id="e069d-148">O próximo deslocamento do final de uma página é 100 menos 64, que é igual a 36.</span><span class="sxs-lookup"><span data-stu-id="e069d-148">The next offset from the end for a page is 100 minus 64 which equals 36.</span></span> <span data-ttu-id="e069d-149">O valor do próximo deslocamento do fim para obter a próxima página indexada é 36.</span><span class="sxs-lookup"><span data-stu-id="e069d-149">The value for the next offset from the end to get the next indexed page is 36.</span></span>
  
<span data-ttu-id="e069d-150">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="e069d-150">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e069d-151">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e069d-151">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e069d-152">Namespace</span><span class="sxs-lookup"><span data-stu-id="e069d-152">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e069d-153">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e069d-153">Schema Name</span></span>  <br/> |<span data-ttu-id="e069d-154">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="e069d-154">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e069d-155">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e069d-155">Validation File</span></span>  <br/> |<span data-ttu-id="e069d-156">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e069d-156">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e069d-157">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e069d-157">Can be Empty</span></span>  <br/> |<span data-ttu-id="e069d-158">Falso</span><span class="sxs-lookup"><span data-stu-id="e069d-158">False</span></span>  <br/> |
   

