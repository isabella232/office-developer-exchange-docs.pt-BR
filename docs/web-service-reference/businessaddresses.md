---
title: BusinessAddresses
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 828f8f62-7abf-44d4-8d58-f706d595a812
description: O elemento BusinessAddresses Especifica uma matriz de endereços corporativos e os identificadores de suas atribuições de origem para a pessoa associada.
ms.openlocfilehash: bc7ad948572c24f913ae02abb9e8fc5a7b1e0b0d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751307"
---
# <a name="businessaddresses"></a><span data-ttu-id="aeace-103">BusinessAddresses</span><span class="sxs-lookup"><span data-stu-id="aeace-103">BusinessAddresses</span></span>

<span data-ttu-id="aeace-104">O elemento **BusinessAddresses** Especifica uma matriz de endereços corporativos e os identificadores de suas atribuições de origem para a pessoa associada.</span><span class="sxs-lookup"><span data-stu-id="aeace-104">The **BusinessAddresses** element specifies an array of business addresses and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<BusinessAddresses>
    <PostalAddressAttributedValue></PostalAddressAttributedValue>
</BusinessAddresses
```

 <span data-ttu-id="aeace-105">**ArrayOfPostalAddressAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="aeace-105">**ArrayOfPostalAddressAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aeace-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="aeace-106">Attributes and elements</span></span>

<span data-ttu-id="aeace-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="aeace-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aeace-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="aeace-108">Attributes</span></span>

<span data-ttu-id="aeace-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="aeace-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aeace-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="aeace-110">Child elements</span></span>

|<span data-ttu-id="aeace-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="aeace-111">**Element**</span></span>|<span data-ttu-id="aeace-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="aeace-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aeace-113">PostalAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="aeace-113">PostalAddressAttributedValue</span></span>](postaladdressattributedvalue.md) <br/> |<span data-ttu-id="aeace-114">Especifica uma instância de uma matriz de endereços postais e suas atribuições associadas.</span><span class="sxs-lookup"><span data-stu-id="aeace-114">Specifies an instance of an array of postal addresses and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aeace-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="aeace-115">Parent elements</span></span>

|<span data-ttu-id="aeace-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="aeace-116">**Element**</span></span>|<span data-ttu-id="aeace-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="aeace-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aeace-118">Pessoa</span><span class="sxs-lookup"><span data-stu-id="aeace-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="aeace-119">Especifica um conjunto de dados de pessoa retornados por uma solicitação **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="aeace-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="aeace-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="aeace-120">Remarks</span></span>

<span data-ttu-id="aeace-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="aeace-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="aeace-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="aeace-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aeace-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="aeace-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aeace-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="aeace-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="aeace-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="aeace-125">Schema Name</span></span>  <br/> |<span data-ttu-id="aeace-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="aeace-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="aeace-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="aeace-127">Validation File</span></span>  <br/> |<span data-ttu-id="aeace-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="aeace-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="aeace-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="aeace-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="aeace-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="aeace-130">See also</span></span>



- [<span data-ttu-id="aeace-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="aeace-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

