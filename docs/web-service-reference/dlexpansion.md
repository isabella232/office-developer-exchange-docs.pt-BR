---
title: DLExpansion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DLExpansion
api_type:
- schema
ms.assetid: 9e50278d-fe6a-45e2-a72b-0fb06809e128
description: O elemento DLExpansion contém uma matriz de caixas de correio que estão contidos em uma lista de distribuição.
ms.openlocfilehash: 06081b4aba761a7137f921b3bc1c8d6b2afab88c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751909"
---
# <a name="dlexpansion"></a><span data-ttu-id="079eb-103">DLExpansion</span><span class="sxs-lookup"><span data-stu-id="079eb-103">DLExpansion</span></span>

<span data-ttu-id="079eb-104">O elemento **DLExpansion** contém uma matriz de caixas de correio que estão contidos em uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="079eb-104">The **DLExpansion** element contains an array of mailboxes that are contained in a distribution list.</span></span> 
  
- [<span data-ttu-id="079eb-105">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="079eb-105">ExpandDLResponse</span></span>](expanddlresponse.md) 
- [<span data-ttu-id="079eb-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="079eb-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="079eb-107">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="079eb-107">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
- [<span data-ttu-id="079eb-108">DLExpansion</span><span class="sxs-lookup"><span data-stu-id="079eb-108">DLExpansion</span></span>](dlexpansion.md)
  
```xml
<DLExpansion AbsoluteDenominator"" IncludesLastItemInRange="" IndexedPagingOffset="" NumeratorOffset="" TotalItemsInView="">
   <Mailbox/>
</DLExpansion>
```

 <span data-ttu-id="079eb-109">**ArrayOfDLExpansionType**</span><span class="sxs-lookup"><span data-stu-id="079eb-109">**ArrayOfDLExpansionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="079eb-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="079eb-110">Attributes and elements</span></span>

<span data-ttu-id="079eb-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="079eb-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="079eb-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="079eb-112">Attributes</span></span>

|<span data-ttu-id="079eb-113">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="079eb-113">**Attribute**</span></span>|<span data-ttu-id="079eb-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="079eb-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="079eb-115">**IndexedPagingOffset**</span><span class="sxs-lookup"><span data-stu-id="079eb-115">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="079eb-116">Representa o próximo índice que deve ser usado para a próxima solicitação quando você estiver usando um modo de exibição de página indexados.</span><span class="sxs-lookup"><span data-stu-id="079eb-116">Represents the next index that should be used for the next request when you are using an indexed page view.</span></span>  <br/> |
|<span data-ttu-id="079eb-117">**NumeratorOffset**</span><span class="sxs-lookup"><span data-stu-id="079eb-117">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="079eb-118">Representa o novo valor numerador a ser usado para a próxima solicitação quando você estiver usando os modos de exibição de página de fração.</span><span class="sxs-lookup"><span data-stu-id="079eb-118">Represents the new numerator value to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="079eb-119">**AbsoluteDenominator**</span><span class="sxs-lookup"><span data-stu-id="079eb-119">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="079eb-120">Representa o denominador próximo a ser usado para a próxima solicitação quando você estiver usando os modos de exibição de página de fração.</span><span class="sxs-lookup"><span data-stu-id="079eb-120">Represents the next denominator to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="079eb-121">**IncludesLastItemInRange**</span><span class="sxs-lookup"><span data-stu-id="079eb-121">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="079eb-122">Indica se os resultados atuais contêm o último item na consulta de forma que não é necessária a paginação adicional.</span><span class="sxs-lookup"><span data-stu-id="079eb-122">Indicates whether the current results contain the last item in the query so that additional paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="079eb-123">**TotalItemsInView**</span><span class="sxs-lookup"><span data-stu-id="079eb-123">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="079eb-124">Representa o número total de itens no modo de exibição.</span><span class="sxs-lookup"><span data-stu-id="079eb-124">Represents the total number of items in the view.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="079eb-125">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="079eb-125">Child elements</span></span>

|<span data-ttu-id="079eb-126">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="079eb-126">**Element**</span></span>|<span data-ttu-id="079eb-127">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="079eb-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="079eb-128">Caixa de correio</span><span class="sxs-lookup"><span data-stu-id="079eb-128">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="079eb-129">Identifica um objeto de serviço de diretório do Active Directory habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="079eb-129">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="079eb-130">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="079eb-130">Parent elements</span></span>

|<span data-ttu-id="079eb-131">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="079eb-131">**Element**</span></span>|<span data-ttu-id="079eb-132">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="079eb-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="079eb-133">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="079eb-133">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md) <br/> |<span data-ttu-id="079eb-134">Contém o status e o resultado de uma única solicitação ExpandDL.</span><span class="sxs-lookup"><span data-stu-id="079eb-134">Contains the status and result of a single ExpandDL request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="079eb-135">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="079eb-135">Remarks</span></span>

<span data-ttu-id="079eb-136">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="079eb-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="079eb-137">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="079eb-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="079eb-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="079eb-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="079eb-139">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="079eb-139">Schema Name</span></span>  <br/> |<span data-ttu-id="079eb-140">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="079eb-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="079eb-141">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="079eb-141">Validation File</span></span>  <br/> |<span data-ttu-id="079eb-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="079eb-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="079eb-143">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="079eb-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="079eb-144">False</span><span class="sxs-lookup"><span data-stu-id="079eb-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="079eb-145">Ver também</span><span class="sxs-lookup"><span data-stu-id="079eb-145">See also</span></span>

- [<span data-ttu-id="079eb-146">Operação ExpandDL</span><span class="sxs-lookup"><span data-stu-id="079eb-146">ExpandDL operation</span></span>](expanddl-operation.md)
- [<span data-ttu-id="079eb-147">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="079eb-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md) 
- [<span data-ttu-id="079eb-148">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="079eb-148">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

