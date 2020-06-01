---
title: BusinessAddresses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 828f8f62-7abf-44d4-8d58-f706d595a812
description: O elemento BusinessAddresses especifica uma matriz de endereços de negócios e os identificadores de suas atribuições de origem para o persona associado.
ms.openlocfilehash: d314d0de679f8eabc51dc9ee3b2e9a57cd0b8da1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465923"
---
# <a name="businessaddresses"></a><span data-ttu-id="6daaa-103">BusinessAddresses</span><span class="sxs-lookup"><span data-stu-id="6daaa-103">BusinessAddresses</span></span>

<span data-ttu-id="6daaa-104">O elemento **BusinessAddresses** especifica uma matriz de endereços de negócios e os identificadores de suas atribuições de origem para o persona associado.</span><span class="sxs-lookup"><span data-stu-id="6daaa-104">The **BusinessAddresses** element specifies an array of business addresses and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<BusinessAddresses>
    <PostalAddressAttributedValue></PostalAddressAttributedValue>
</BusinessAddresses
```

 <span data-ttu-id="6daaa-105">**ArrayOfPostalAddressAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="6daaa-105">**ArrayOfPostalAddressAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6daaa-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="6daaa-106">Attributes and elements</span></span>

<span data-ttu-id="6daaa-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6daaa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6daaa-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="6daaa-108">Attributes</span></span>

<span data-ttu-id="6daaa-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6daaa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6daaa-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6daaa-110">Child elements</span></span>

|<span data-ttu-id="6daaa-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6daaa-111">**Element**</span></span>|<span data-ttu-id="6daaa-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6daaa-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6daaa-113">PostalAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="6daaa-113">PostalAddressAttributedValue</span></span>](postaladdressattributedvalue.md) <br/> |<span data-ttu-id="6daaa-114">Especifica uma instância de uma matriz de endereços postais e suas atribuições associadas.</span><span class="sxs-lookup"><span data-stu-id="6daaa-114">Specifies an instance of an array of postal addresses and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6daaa-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6daaa-115">Parent elements</span></span>

|<span data-ttu-id="6daaa-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6daaa-116">**Element**</span></span>|<span data-ttu-id="6daaa-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6daaa-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6daaa-118">Pessoal</span><span class="sxs-lookup"><span data-stu-id="6daaa-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="6daaa-119">Especifica um conjunto de dados persona retornados por uma solicitação **Getpersona** .</span><span class="sxs-lookup"><span data-stu-id="6daaa-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6daaa-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="6daaa-120">Remarks</span></span>

<span data-ttu-id="6daaa-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6daaa-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6daaa-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6daaa-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6daaa-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="6daaa-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6daaa-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="6daaa-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6daaa-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6daaa-125">Schema Name</span></span>  <br/> |<span data-ttu-id="6daaa-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="6daaa-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="6daaa-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6daaa-127">Validation File</span></span>  <br/> |<span data-ttu-id="6daaa-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="6daaa-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="6daaa-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="6daaa-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="6daaa-130">Também consulte</span><span class="sxs-lookup"><span data-stu-id="6daaa-130">See also</span></span>



- [<span data-ttu-id="6daaa-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6daaa-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

