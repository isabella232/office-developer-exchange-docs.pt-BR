---
title: RootFolder (FindFolderResponseMessage)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RootFolder
api_type:
- schema
ms.assetid: 5089c815-663f-46be-bc59-aed9ee20f94a
description: O elemento RootFolder contém os resultados de uma pesquisa de uma única pasta raiz durante uma operação FindFolder.
ms.openlocfilehash: b5601d6abec67196c9991908e272a2122a201d69
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457134"
---
# <a name="rootfolder-findfolderresponsemessage"></a><span data-ttu-id="d4a9b-103">RootFolder (FindFolderResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="d4a9b-103">RootFolder (FindFolderResponseMessage)</span></span>

<span data-ttu-id="d4a9b-104">O elemento **RootFolder** contém os resultados de uma pesquisa de uma única pasta raiz durante uma [operação FindFolder](findfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="d4a9b-104">The **RootFolder** element contains the results of a search of a single root folder during a [FindFolder operation](findfolder-operation.md).</span></span>
  
```xml
<RootFolder IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Folders/>
</RootFolder>
```

 <span data-ttu-id="d4a9b-105">**FindFolderParentType**</span><span class="sxs-lookup"><span data-stu-id="d4a9b-105">**FindFolderParentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d4a9b-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d4a9b-106">Attributes and elements</span></span>

<span data-ttu-id="d4a9b-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d4a9b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d4a9b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d4a9b-108">Attributes</span></span>

|<span data-ttu-id="d4a9b-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="d4a9b-109">**Attribute**</span></span>|<span data-ttu-id="d4a9b-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d4a9b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d4a9b-111">IndexedPagingOffset</span><span class="sxs-lookup"><span data-stu-id="d4a9b-111">IndexedPagingOffset</span></span>  <br/> |<span data-ttu-id="d4a9b-112">Representa o próximo índice que deve ser usado para a próxima solicitação ao usar um modo de exibição de paginação indexado.</span><span class="sxs-lookup"><span data-stu-id="d4a9b-112">Represents the next index that should be used for the next request when using an indexed paging view.</span></span>  <br/> |
|<span data-ttu-id="d4a9b-113">NumeratorOffset</span><span class="sxs-lookup"><span data-stu-id="d4a9b-113">NumeratorOffset</span></span>  <br/> |<span data-ttu-id="d4a9b-114">Representa o novo valor do numerador a ser usado para a próxima solicitação ao usar as exibições de página fracionada.</span><span class="sxs-lookup"><span data-stu-id="d4a9b-114">Represents the new numerator value to use for the next request when using fractional page views.</span></span>  <br/> |
|<span data-ttu-id="d4a9b-115">AbsoluteDenominator</span><span class="sxs-lookup"><span data-stu-id="d4a9b-115">AbsoluteDenominator</span></span>  <br/> |<span data-ttu-id="d4a9b-116">Representa o próximo denominador a ser usado para a próxima solicitação ao fazer paginação fracionária.</span><span class="sxs-lookup"><span data-stu-id="d4a9b-116">Represents the next denominator to use for the next request when doing fractional paging.</span></span>  <br/> |
|<span data-ttu-id="d4a9b-117">IncludesLastItemInRange</span><span class="sxs-lookup"><span data-stu-id="d4a9b-117">IncludesLastItemInRange</span></span>  <br/> |<span data-ttu-id="d4a9b-118">Indica se os resultados atuais contêm a última pasta na consulta, de modo que a paginação adicional não será necessária.</span><span class="sxs-lookup"><span data-stu-id="d4a9b-118">Indicates whether the current results contain the last folder in the query, such that further paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="d4a9b-119">TotalItemsInView</span><span class="sxs-lookup"><span data-stu-id="d4a9b-119">TotalItemsInView</span></span>  <br/> |<span data-ttu-id="d4a9b-120">Representa o número total de pastas que passam a restrição.</span><span class="sxs-lookup"><span data-stu-id="d4a9b-120">Represents the total number of folders that pass the restriction.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d4a9b-121">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d4a9b-121">Child elements</span></span>

|<span data-ttu-id="d4a9b-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d4a9b-122">**Element**</span></span>|<span data-ttu-id="d4a9b-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d4a9b-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4a9b-124">Pastas</span><span class="sxs-lookup"><span data-stu-id="d4a9b-124">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d4a9b-125">Contém uma matriz de pastas encontradas usando a [operação FindFolder](findfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="d4a9b-125">Contains an array of folders found by using the [FindFolder operation](findfolder-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d4a9b-126">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d4a9b-126">Parent elements</span></span>

|<span data-ttu-id="d4a9b-127">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d4a9b-127">**Element**</span></span>|<span data-ttu-id="d4a9b-128">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d4a9b-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4a9b-129">FindFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d4a9b-129">FindFolderResponseMessage</span></span>](findfolderresponsemessage.md) <br/> |<span data-ttu-id="d4a9b-130">Contém o status e o resultado de uma solicitação de [operação FindFolder](findfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="d4a9b-130">Contains the status and result of a [FindFolder operation](findfolder-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d4a9b-131">Comentários</span><span class="sxs-lookup"><span data-stu-id="d4a9b-131">Remarks</span></span>

<span data-ttu-id="d4a9b-132">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="d4a9b-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d4a9b-133">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d4a9b-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d4a9b-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="d4a9b-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d4a9b-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d4a9b-135">Schema name</span></span>  <br/> |<span data-ttu-id="d4a9b-136">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="d4a9b-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d4a9b-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d4a9b-137">Validation file</span></span>  <br/> |<span data-ttu-id="d4a9b-138">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d4a9b-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d4a9b-139">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="d4a9b-139">Can be empty</span></span>  <br/> |<span data-ttu-id="d4a9b-140">False</span><span class="sxs-lookup"><span data-stu-id="d4a9b-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d4a9b-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="d4a9b-141">See also</span></span>



[<span data-ttu-id="d4a9b-142">Operação FindFolder</span><span class="sxs-lookup"><span data-stu-id="d4a9b-142">FindFolder operation</span></span>](findfolder-operation.md)


[<span data-ttu-id="d4a9b-143">Localizando pastas</span><span class="sxs-lookup"><span data-stu-id="d4a9b-143">Finding Folders</span></span>](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

