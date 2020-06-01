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
description: O elemento DLExpansion contém uma matriz de caixas de correio que estão contidas em uma lista de distribuição.
ms.openlocfilehash: 079ad1c0f114d201f5d1b91c3fd9bb45b943cc1a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456994"
---
# <a name="dlexpansion"></a><span data-ttu-id="6b1fc-103">DLExpansion</span><span class="sxs-lookup"><span data-stu-id="6b1fc-103">DLExpansion</span></span>

<span data-ttu-id="6b1fc-104">O elemento **DLExpansion** contém uma matriz de caixas de correio que estão contidas em uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="6b1fc-104">The **DLExpansion** element contains an array of mailboxes that are contained in a distribution list.</span></span> 
  
- [<span data-ttu-id="6b1fc-105">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="6b1fc-105">ExpandDLResponse</span></span>](expanddlresponse.md) 
- [<span data-ttu-id="6b1fc-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="6b1fc-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="6b1fc-107">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6b1fc-107">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
- [<span data-ttu-id="6b1fc-108">DLExpansion</span><span class="sxs-lookup"><span data-stu-id="6b1fc-108">DLExpansion</span></span>](dlexpansion.md)
  
```xml
<DLExpansion AbsoluteDenominator"" IncludesLastItemInRange="" IndexedPagingOffset="" NumeratorOffset="" TotalItemsInView="">
   <Mailbox/>
</DLExpansion>
```

 <span data-ttu-id="6b1fc-109">**ArrayOfDLExpansionType**</span><span class="sxs-lookup"><span data-stu-id="6b1fc-109">**ArrayOfDLExpansionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6b1fc-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="6b1fc-110">Attributes and elements</span></span>

<span data-ttu-id="6b1fc-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6b1fc-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6b1fc-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="6b1fc-112">Attributes</span></span>

|<span data-ttu-id="6b1fc-113">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="6b1fc-113">**Attribute**</span></span>|<span data-ttu-id="6b1fc-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6b1fc-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6b1fc-115">**IndexedPagingOffset**</span><span class="sxs-lookup"><span data-stu-id="6b1fc-115">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="6b1fc-116">Representa o próximo índice que deve ser usado para a próxima solicitação quando você estiver usando um modo de exibição de página indexado.</span><span class="sxs-lookup"><span data-stu-id="6b1fc-116">Represents the next index that should be used for the next request when you are using an indexed page view.</span></span>  <br/> |
|<span data-ttu-id="6b1fc-117">**NumeratorOffset**</span><span class="sxs-lookup"><span data-stu-id="6b1fc-117">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="6b1fc-118">Representa o novo valor do numerador a ser usado para a próxima solicitação quando você estiver usando modos de exibição de página de fração.</span><span class="sxs-lookup"><span data-stu-id="6b1fc-118">Represents the new numerator value to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="6b1fc-119">**AbsoluteDenominator**</span><span class="sxs-lookup"><span data-stu-id="6b1fc-119">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="6b1fc-120">Representa o próximo denominador a ser usado para a próxima solicitação quando você estiver usando modos de exibição de página de fração.</span><span class="sxs-lookup"><span data-stu-id="6b1fc-120">Represents the next denominator to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="6b1fc-121">**IncludesLastItemInRange**</span><span class="sxs-lookup"><span data-stu-id="6b1fc-121">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="6b1fc-122">Indica se os resultados atuais contêm o último item na consulta para que a paginação adicional não seja necessária.</span><span class="sxs-lookup"><span data-stu-id="6b1fc-122">Indicates whether the current results contain the last item in the query so that additional paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="6b1fc-123">**TotalItemsInView**</span><span class="sxs-lookup"><span data-stu-id="6b1fc-123">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="6b1fc-124">Representa o número total de itens no modo de exibição.</span><span class="sxs-lookup"><span data-stu-id="6b1fc-124">Represents the total number of items in the view.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6b1fc-125">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6b1fc-125">Child elements</span></span>

|<span data-ttu-id="6b1fc-126">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6b1fc-126">**Element**</span></span>|<span data-ttu-id="6b1fc-127">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6b1fc-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6b1fc-128">Caixa de Correio</span><span class="sxs-lookup"><span data-stu-id="6b1fc-128">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="6b1fc-129">Identifica um objeto de serviço de diretório do Active Directory habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="6b1fc-129">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6b1fc-130">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6b1fc-130">Parent elements</span></span>

|<span data-ttu-id="6b1fc-131">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6b1fc-131">**Element**</span></span>|<span data-ttu-id="6b1fc-132">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6b1fc-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6b1fc-133">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6b1fc-133">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md) <br/> |<span data-ttu-id="6b1fc-134">Contém o status e o resultado de uma única solicitação de ExpandDL.</span><span class="sxs-lookup"><span data-stu-id="6b1fc-134">Contains the status and result of a single ExpandDL request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6b1fc-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="6b1fc-135">Remarks</span></span>

<span data-ttu-id="6b1fc-136">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="6b1fc-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6b1fc-137">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="6b1fc-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6b1fc-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="6b1fc-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6b1fc-139">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6b1fc-139">Schema Name</span></span>  <br/> |<span data-ttu-id="6b1fc-140">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="6b1fc-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="6b1fc-141">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6b1fc-141">Validation File</span></span>  <br/> |<span data-ttu-id="6b1fc-142">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="6b1fc-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6b1fc-143">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6b1fc-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="6b1fc-144">False</span><span class="sxs-lookup"><span data-stu-id="6b1fc-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6b1fc-145">Confira também</span><span class="sxs-lookup"><span data-stu-id="6b1fc-145">See also</span></span>

- [<span data-ttu-id="6b1fc-146">Operação ExpandDL</span><span class="sxs-lookup"><span data-stu-id="6b1fc-146">ExpandDL operation</span></span>](expanddl-operation.md)
- [<span data-ttu-id="6b1fc-147">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6b1fc-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md) 
- [<span data-ttu-id="6b1fc-148">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="6b1fc-148">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

