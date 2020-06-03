---
title: FractionalPageFolderView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FractionalPageFolderView
api_type:
- schema
ms.assetid: ef681f8a-136a-4c0e-ade6-ddcdbf2d85ad
description: O elemento FractionalPageFolderView descreve onde o modo de exibição paginado começa e o número máximo de pastas retornadas em uma solicitação FindFolder.
ms.openlocfilehash: a8627c6277b49655d3933679128b844118633cda
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463066"
---
# <a name="fractionalpagefolderview"></a><span data-ttu-id="1ea81-103">FractionalPageFolderView</span><span class="sxs-lookup"><span data-stu-id="1ea81-103">FractionalPageFolderView</span></span>

<span data-ttu-id="1ea81-104">O elemento **FractionalPageFolderView** descreve onde o modo de exibição paginado começa e o número máximo de pastas retornadas em uma solicitação [FindFolder](findfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="1ea81-104">The **FractionalPageFolderView** element describes where the paged view starts and the maximum number of folders returned in a [FindFolder](findfolder.md) request.</span></span> 
  
[<span data-ttu-id="1ea81-105">FindFolder</span><span class="sxs-lookup"><span data-stu-id="1ea81-105">FindFolder</span></span>](findfolder.md)
  
[<span data-ttu-id="1ea81-106">FractionalPageFolderView</span><span class="sxs-lookup"><span data-stu-id="1ea81-106">FractionalPageFolderView</span></span>](fractionalpagefolderview.md)
  
```xml
<FractionalPageFolderView MaxEntriesReturned="" Numerator="" Denominator=""/>
```

 <span data-ttu-id="1ea81-107">**FractionalPageViewType**</span><span class="sxs-lookup"><span data-stu-id="1ea81-107">**FractionalPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1ea81-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="1ea81-108">Attributes and elements</span></span>

<span data-ttu-id="1ea81-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1ea81-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1ea81-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="1ea81-110">Attributes</span></span>

|<span data-ttu-id="1ea81-111">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="1ea81-111">**Attribute**</span></span>|<span data-ttu-id="1ea81-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1ea81-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1ea81-113">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="1ea81-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="1ea81-114">Identifica o número máximo de resultados a serem retornados na resposta [FindFolder](findfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="1ea81-114">Identifies the maximum number of results to return in the [FindFolder](findfolder.md) response.</span></span> <span data-ttu-id="1ea81-115">Esse atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="1ea81-115">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="1ea81-116">**Numera**</span><span class="sxs-lookup"><span data-stu-id="1ea81-116">**Numerator**</span></span> <br/> |<span data-ttu-id="1ea81-117">Representa o numerador do deslocamento fracionado do início do conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="1ea81-117">Represents the numerator of the fractional offset from the start of the result set.</span></span> <span data-ttu-id="1ea81-118">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="1ea81-118">This attribute is required.</span></span> <span data-ttu-id="1ea81-119">O numerador deve ser igual ou menor que o denominador.</span><span class="sxs-lookup"><span data-stu-id="1ea81-119">The numerator must be equal to or less than the denominator.</span></span> <span data-ttu-id="1ea81-120">Este atributo deve representar um valor inteiro igual ou maior que zero.</span><span class="sxs-lookup"><span data-stu-id="1ea81-120">This attribute must represent an integral value that is equal to or greater than zero.</span></span> <span data-ttu-id="1ea81-121">Para obter mais informações, consulte comentários mais adiante neste tópico.</span><span class="sxs-lookup"><span data-stu-id="1ea81-121">For more information, see Remarks later in this topic.</span></span>  <br/> |
|<span data-ttu-id="1ea81-122">**Denominado**</span><span class="sxs-lookup"><span data-stu-id="1ea81-122">**Denominator**</span></span> <br/> |<span data-ttu-id="1ea81-123">Representa o denominador do deslocamento fracionado desde o início do número total de pastas no conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="1ea81-123">Represents the denominator of the fractional offset from the start of the total number of folders in the result set.</span></span> <span data-ttu-id="1ea81-124">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="1ea81-124">This attribute is required.</span></span> <span data-ttu-id="1ea81-125">Este atributo deve representar um valor integral maior que um.</span><span class="sxs-lookup"><span data-stu-id="1ea81-125">This attribute must represent an integral value that is greater than one.</span></span> <span data-ttu-id="1ea81-126">Para obter mais informações, consulte comentários mais adiante neste tópico.</span><span class="sxs-lookup"><span data-stu-id="1ea81-126">For more information, see Remarks later in this topic.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1ea81-127">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1ea81-127">Child elements</span></span>

<span data-ttu-id="1ea81-128">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1ea81-128">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1ea81-129">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1ea81-129">Parent elements</span></span>

|<span data-ttu-id="1ea81-130">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1ea81-130">**Element**</span></span>|<span data-ttu-id="1ea81-131">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1ea81-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1ea81-132">FindFolder</span><span class="sxs-lookup"><span data-stu-id="1ea81-132">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="1ea81-133">Define uma solicitação para identificar pastas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="1ea81-133">Defines a request to identify folders in a mailbox.</span></span>  <br/> <span data-ttu-id="1ea81-134">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="1ea81-134">The following is the XPath expression to this element:</span></span>  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1ea81-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="1ea81-135">Remarks</span></span>

<span data-ttu-id="1ea81-136">O deslocamento de modo de exibição paginado desde o início do conjunto de pastas encontradas é descrito por uma fração.</span><span class="sxs-lookup"><span data-stu-id="1ea81-136">The paged view offset from the start of the set of found folders is described by a fraction.</span></span> <span data-ttu-id="1ea81-137">A fração, que é definida pelos atributos **numerador** e **denominador** , descreve onde a página de informações é iniciada.</span><span class="sxs-lookup"><span data-stu-id="1ea81-137">The fraction, which is defined by the **Numerator** and **Denominator** attributes, describes where the page of information starts.</span></span> <span data-ttu-id="1ea81-138">Por exemplo, se o **numerador** for igual a quatro e o **denominador** for igual a cinco, a página de informações retornadas será iniciada em uma entrada localizada em quatro cinco quinto da forma no conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="1ea81-138">For example, if **Numerator** equals four and **Denominator** equals five, the page of returned information starts at an entry located four-fifths of the way in to the result set.</span></span> 
  
<span data-ttu-id="1ea81-139">Se a fração for avaliada como zero, isso indica o início do conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="1ea81-139">If the fraction evaluates to zero, that indicates the start of the results set.</span></span> <span data-ttu-id="1ea81-140">Se a fração for avaliada como um, isso indica o final do conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="1ea81-140">If the fraction evaluates to one, that indicates the end of the result set.</span></span>
  
> [!NOTE]
> <span data-ttu-id="1ea81-141">A fração representa o ponto de início da página, não quantos resultados serão retornados no conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="1ea81-141">The fraction represents the start point of page, not how many results in the result set will be returned.</span></span> 
  
<span data-ttu-id="1ea81-142">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="1ea81-142">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1ea81-143">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="1ea81-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1ea81-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="1ea81-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1ea81-145">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1ea81-145">Schema Name</span></span>  <br/> |<span data-ttu-id="1ea81-146">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="1ea81-146">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1ea81-147">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1ea81-147">Validation File</span></span>  <br/> |<span data-ttu-id="1ea81-148">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1ea81-148">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1ea81-149">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="1ea81-149">Can be Empty</span></span>  <br/> |<span data-ttu-id="1ea81-150">False</span><span class="sxs-lookup"><span data-stu-id="1ea81-150">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1ea81-151">Confira também</span><span class="sxs-lookup"><span data-stu-id="1ea81-151">See also</span></span>



[<span data-ttu-id="1ea81-152">Operação FindFolder</span><span class="sxs-lookup"><span data-stu-id="1ea81-152">FindFolder operation</span></span>](findfolder-operation.md)


[<span data-ttu-id="1ea81-153">Localizando pastas</span><span class="sxs-lookup"><span data-stu-id="1ea81-153">Finding Folders</span></span>](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

