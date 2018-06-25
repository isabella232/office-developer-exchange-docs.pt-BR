---
title: ImAddresses (ArrayOfStringAttributedValuesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b95d0a8b-15a6-4711-b014-55698dbd679c
description: O elemento ImAddresses Especifica uma matriz de endereços de mensagem instantânea e os identificadores de suas atribuições de origem para a pessoa associada.
ms.openlocfilehash: 6f238e26083366320ba04b187e3e41771cbd14ba
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823863"
---
# <a name="imaddresses-arrayofstringattributedvaluestype"></a><span data-ttu-id="94123-103">ImAddresses (ArrayOfStringAttributedValuesType)</span><span class="sxs-lookup"><span data-stu-id="94123-103">ImAddresses (ArrayOfStringAttributedValuesType)</span></span>

<span data-ttu-id="94123-104">O elemento **ImAddresses** Especifica uma matriz de endereços de mensagem instantânea e os identificadores de suas atribuições de origem para a pessoa associada.</span><span class="sxs-lookup"><span data-stu-id="94123-104">The **ImAddresses** element specifies an array of instant message addresses and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<ImAddresses>
    <StringAttributedValue/>
</ImAddresses>
```

 <span data-ttu-id="94123-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="94123-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="94123-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="94123-106">Attributes and elements</span></span>

<span data-ttu-id="94123-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="94123-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="94123-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="94123-108">Attributes</span></span>

<span data-ttu-id="94123-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="94123-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="94123-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="94123-110">Child elements</span></span>

|<span data-ttu-id="94123-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="94123-111">**Element**</span></span>|<span data-ttu-id="94123-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="94123-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="94123-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="94123-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="94123-114">Especifica uma instância em uma matriz de atributos associados a um elemento de pessoa.</span><span class="sxs-lookup"><span data-stu-id="94123-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="94123-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="94123-115">Parent elements</span></span>

|<span data-ttu-id="94123-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="94123-116">**Element**</span></span>|<span data-ttu-id="94123-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="94123-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="94123-118">Pessoa</span><span class="sxs-lookup"><span data-stu-id="94123-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="94123-119">Especifica um conjunto de dados de pessoa retornados por uma solicitação **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="94123-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="94123-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="94123-120">Remarks</span></span>

<span data-ttu-id="94123-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="94123-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="94123-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="94123-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="94123-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="94123-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="94123-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="94123-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="94123-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="94123-125">Schema Name</span></span>  <br/> |<span data-ttu-id="94123-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="94123-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="94123-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="94123-127">Validation File</span></span>  <br/> |<span data-ttu-id="94123-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="94123-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="94123-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="94123-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="94123-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="94123-130">See also</span></span>



- [<span data-ttu-id="94123-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="94123-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

