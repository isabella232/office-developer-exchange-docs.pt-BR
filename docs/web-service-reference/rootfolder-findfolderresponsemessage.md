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
description: O elemento RootFolder contém os resultados de uma pesquisa de uma pasta raiz única durante uma operação FindFolder.
ms.openlocfilehash: 1cd79d5fa34318e7fe29606df84cbf0ef0520b93
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825253"
---
# <a name="rootfolder-findfolderresponsemessage"></a><span data-ttu-id="f4b3c-103">RootFolder (FindFolderResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="f4b3c-103">RootFolder (FindFolderResponseMessage)</span></span>

<span data-ttu-id="f4b3c-104">O elemento **RootFolder** contém os resultados de uma pesquisa de uma pasta raiz única durante uma [operação FindFolder](findfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="f4b3c-104">The **RootFolder** element contains the results of a search of a single root folder during a [FindFolder operation](findfolder-operation.md).</span></span>
  
```xml
<RootFolder IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Folders/>
</RootFolder>
```

 <span data-ttu-id="f4b3c-105">**FindFolderParentType**</span><span class="sxs-lookup"><span data-stu-id="f4b3c-105">**FindFolderParentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f4b3c-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f4b3c-106">Attributes and elements</span></span>

<span data-ttu-id="f4b3c-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f4b3c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f4b3c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f4b3c-108">Attributes</span></span>

|<span data-ttu-id="f4b3c-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="f4b3c-109">**Attribute**</span></span>|<span data-ttu-id="f4b3c-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f4b3c-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f4b3c-111">IndexedPagingOffset</span><span class="sxs-lookup"><span data-stu-id="f4b3c-111">IndexedPagingOffset</span></span>  <br/> |<span data-ttu-id="f4b3c-112">Representa o próximo índice que deve ser usado para a próxima solicitação ao usar o modo de exibição indexada paginação.</span><span class="sxs-lookup"><span data-stu-id="f4b3c-112">Represents the next index that should be used for the next request when using an indexed paging view.</span></span>  <br/> |
|<span data-ttu-id="f4b3c-113">NumeratorOffset</span><span class="sxs-lookup"><span data-stu-id="f4b3c-113">NumeratorOffset</span></span>  <br/> |<span data-ttu-id="f4b3c-114">Representa o novo valor numerador usada para a próxima solicitação quando usar exibições de página fracionais.</span><span class="sxs-lookup"><span data-stu-id="f4b3c-114">Represents the new numerator value to use for the next request when using fractional page views.</span></span>  <br/> |
|<span data-ttu-id="f4b3c-115">AbsoluteDenominator</span><span class="sxs-lookup"><span data-stu-id="f4b3c-115">AbsoluteDenominator</span></span>  <br/> |<span data-ttu-id="f4b3c-116">Representa o denominador próximo a ser usado para a próxima solicitação ao fazer a paginação fracional.</span><span class="sxs-lookup"><span data-stu-id="f4b3c-116">Represents the next denominator to use for the next request when doing fractional paging.</span></span>  <br/> |
|<span data-ttu-id="f4b3c-117">IncludesLastItemInRange</span><span class="sxs-lookup"><span data-stu-id="f4b3c-117">IncludesLastItemInRange</span></span>  <br/> |<span data-ttu-id="f4b3c-118">Indica se os resultados atuais contêm a última pasta na consulta, de forma que não seja necessário paginação ainda mais.</span><span class="sxs-lookup"><span data-stu-id="f4b3c-118">Indicates whether the current results contain the last folder in the query, such that further paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="f4b3c-119">TotalItemsInView</span><span class="sxs-lookup"><span data-stu-id="f4b3c-119">TotalItemsInView</span></span>  <br/> |<span data-ttu-id="f4b3c-120">Representa o número total de pastas que passam a restrição.</span><span class="sxs-lookup"><span data-stu-id="f4b3c-120">Represents the total number of folders that pass the restriction.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f4b3c-121">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f4b3c-121">Child elements</span></span>

|<span data-ttu-id="f4b3c-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f4b3c-122">**Element**</span></span>|<span data-ttu-id="f4b3c-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f4b3c-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f4b3c-124">Pastas</span><span class="sxs-lookup"><span data-stu-id="f4b3c-124">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f4b3c-125">Contém uma matriz das pastas encontrado usando a [operação FindFolder](findfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="f4b3c-125">Contains an array of folders found by using the [FindFolder operation](findfolder-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f4b3c-126">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f4b3c-126">Parent elements</span></span>

|<span data-ttu-id="f4b3c-127">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f4b3c-127">**Element**</span></span>|<span data-ttu-id="f4b3c-128">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f4b3c-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f4b3c-129">FindFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f4b3c-129">FindFolderResponseMessage</span></span>](findfolderresponsemessage.md) <br/> |<span data-ttu-id="f4b3c-130">Contém o status e o resultado de uma solicitação de [operação FindFolder](findfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="f4b3c-130">Contains the status and result of a [FindFolder operation](findfolder-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f4b3c-131">Comentários</span><span class="sxs-lookup"><span data-stu-id="f4b3c-131">Remarks</span></span>

<span data-ttu-id="f4b3c-132">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="f4b3c-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f4b3c-133">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f4b3c-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f4b3c-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="f4b3c-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f4b3c-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f4b3c-135">Schema name</span></span>  <br/> |<span data-ttu-id="f4b3c-136">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="f4b3c-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f4b3c-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f4b3c-137">Validation file</span></span>  <br/> |<span data-ttu-id="f4b3c-138">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f4b3c-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f4b3c-139">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="f4b3c-139">Can be empty</span></span>  <br/> |<span data-ttu-id="f4b3c-140">False</span><span class="sxs-lookup"><span data-stu-id="f4b3c-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f4b3c-141">Ver também</span><span class="sxs-lookup"><span data-stu-id="f4b3c-141">See also</span></span>



[<span data-ttu-id="f4b3c-142">Operação FindFolder</span><span class="sxs-lookup"><span data-stu-id="f4b3c-142">FindFolder operation</span></span>](findfolder-operation.md)


[<span data-ttu-id="f4b3c-143">Localizando pastas</span><span class="sxs-lookup"><span data-stu-id="f4b3c-143">Finding Folders</span></span>](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

