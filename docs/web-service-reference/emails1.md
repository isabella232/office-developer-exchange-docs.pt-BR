---
title: Emails1
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cc02bd86-c618-446a-92f0-749423cbc4ee
description: O elemento Emails1 Especifica uma matriz de valores de EmailAddressAttributedValue e os identificadores de suas atribuições de origem para a pessoa associada.
ms.openlocfilehash: f1a1223244c91731b1a5a1beb9daed6d680d3bc4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752006"
---
# <a name="emails1"></a><span data-ttu-id="b56f7-103">Emails1</span><span class="sxs-lookup"><span data-stu-id="b56f7-103">Emails1</span></span>

<span data-ttu-id="b56f7-104">O elemento **Emails1** Especifica uma matriz de valores de **EmailAddressAttributedValue** e os identificadores de suas atribuições de origem para a pessoa associada.</span><span class="sxs-lookup"><span data-stu-id="b56f7-104">The **Emails1** element specifies an array of **EmailAddressAttributedValue** values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Emails1>
    <EmailAddressAttributedValue></EmailAddressAttributedValue>
</Emails1>
```

 <span data-ttu-id="b56f7-105">**ArrayOfEmailAddressAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="b56f7-105">**ArrayOfEmailAddressAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b56f7-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b56f7-106">Attributes and elements</span></span>

<span data-ttu-id="b56f7-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b56f7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b56f7-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b56f7-108">Attributes</span></span>

<span data-ttu-id="b56f7-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b56f7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b56f7-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b56f7-110">Child elements</span></span>

|<span data-ttu-id="b56f7-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b56f7-111">**Element**</span></span>|<span data-ttu-id="b56f7-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b56f7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b56f7-113">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="b56f7-113">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md) <br/> |<span data-ttu-id="b56f7-114">Especifica uma instância de uma matriz de endereços de email e suas atribuições associadas.</span><span class="sxs-lookup"><span data-stu-id="b56f7-114">Specifies an instance of an array of email addresses and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b56f7-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b56f7-115">Parent elements</span></span>

|<span data-ttu-id="b56f7-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b56f7-116">**Element**</span></span>|<span data-ttu-id="b56f7-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b56f7-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b56f7-118">Pessoa</span><span class="sxs-lookup"><span data-stu-id="b56f7-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="b56f7-119">Especifica um conjunto de dados de pessoa retornados por uma solicitação **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="b56f7-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b56f7-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="b56f7-120">Remarks</span></span>

<span data-ttu-id="b56f7-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b56f7-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b56f7-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b56f7-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b56f7-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b56f7-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b56f7-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="b56f7-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b56f7-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b56f7-125">Schema Name</span></span>  <br/> |<span data-ttu-id="b56f7-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="b56f7-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="b56f7-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b56f7-127">Validation File</span></span>  <br/> |<span data-ttu-id="b56f7-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b56f7-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="b56f7-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="b56f7-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="b56f7-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="b56f7-130">See also</span></span>



- [<span data-ttu-id="b56f7-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b56f7-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

