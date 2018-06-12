---
title: ImAddresses2
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 328f29b9-3a9c-4d9a-a85f-5ffff84e266a
description: O elemento ImAddresses2 Especifica uma matriz de endereços de mensagem instantânea e os identificadores de suas atribuições de origem para a pessoa associada.
ms.openlocfilehash: f61084f22eb9d38766c45e63dfbacc0882ccaaca
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823870"
---
# <a name="imaddresses2"></a><span data-ttu-id="1624e-103">ImAddresses2</span><span class="sxs-lookup"><span data-stu-id="1624e-103">ImAddresses2</span></span>

<span data-ttu-id="1624e-104">O elemento **ImAddresses2** Especifica uma matriz de endereços de mensagem instantânea e os identificadores de suas atribuições de origem para a pessoa associada.</span><span class="sxs-lookup"><span data-stu-id="1624e-104">The **ImAddresses2** element specifies an array of instant message addresses and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<ImAddresses2>
    <StringAttributedValue/>
</ImAddresses2>
```

 <span data-ttu-id="1624e-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="1624e-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1624e-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="1624e-106">Attributes and elements</span></span>

<span data-ttu-id="1624e-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1624e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1624e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="1624e-108">Attributes</span></span>

<span data-ttu-id="1624e-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1624e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1624e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1624e-110">Child elements</span></span>

|<span data-ttu-id="1624e-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1624e-111">**Element**</span></span>|<span data-ttu-id="1624e-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1624e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1624e-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="1624e-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="1624e-114">Especifica uma instância em uma matriz de atributos associados a um elemento de pessoa.</span><span class="sxs-lookup"><span data-stu-id="1624e-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1624e-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1624e-115">Parent elements</span></span>

|<span data-ttu-id="1624e-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1624e-116">**Element**</span></span>|<span data-ttu-id="1624e-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1624e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1624e-118">Pessoa</span><span class="sxs-lookup"><span data-stu-id="1624e-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="1624e-119">Especifica um conjunto de dados de pessoa retornados por uma solicitação **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="1624e-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1624e-120">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="1624e-120">Remarks</span></span>

<span data-ttu-id="1624e-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1624e-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1624e-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1624e-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1624e-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="1624e-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1624e-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="1624e-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1624e-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1624e-125">Schema Name</span></span>  <br/> |<span data-ttu-id="1624e-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="1624e-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="1624e-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1624e-127">Validation File</span></span>  <br/> |<span data-ttu-id="1624e-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1624e-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="1624e-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="1624e-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="1624e-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="1624e-130">See also</span></span>



- [<span data-ttu-id="1624e-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1624e-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

