---
title: Dados fornecidos
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 64d86c24-07b8-448d-ad37-47f104777df3
description: O elemento Especificadonames especifica uma matriz de valores de nome fornecidos e os identificadores de suas atribuições de origem para o persona associado.
ms.openlocfilehash: c76d69344b59fb56377a13b9ea4a588acc382013
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530124"
---
# <a name="givennames"></a><span data-ttu-id="04180-103">Dados fornecidos</span><span class="sxs-lookup"><span data-stu-id="04180-103">GivenNames</span></span>

<span data-ttu-id="04180-104">O elemento **especificadonames** especifica uma matriz de valores de nome fornecidos e os identificadores de suas atribuições de origem para o persona associado.</span><span class="sxs-lookup"><span data-stu-id="04180-104">The **GivenNames** element specifies an array of given name values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```xml
<GivenNames>
    <StringAttributedValue/>
</GivenNames>
```

 <span data-ttu-id="04180-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="04180-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="04180-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="04180-106">Attributes and elements</span></span>

<span data-ttu-id="04180-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="04180-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="04180-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="04180-108">Attributes</span></span>

<span data-ttu-id="04180-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="04180-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="04180-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="04180-110">Child elements</span></span>

|<span data-ttu-id="04180-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="04180-111">**Element**</span></span>|<span data-ttu-id="04180-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="04180-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04180-113">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="04180-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="04180-114">Especifica uma instância em uma matriz de atributos associados a um elemento persona.</span><span class="sxs-lookup"><span data-stu-id="04180-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="04180-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="04180-115">Parent elements</span></span>

|<span data-ttu-id="04180-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="04180-116">**Element**</span></span>|<span data-ttu-id="04180-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="04180-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04180-118">Pessoal</span><span class="sxs-lookup"><span data-stu-id="04180-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="04180-119">Especifica um conjunto de dados persona retornados por uma solicitação **Getpersona** .</span><span class="sxs-lookup"><span data-stu-id="04180-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="04180-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="04180-120">Remarks</span></span>

<span data-ttu-id="04180-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="04180-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="04180-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="04180-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="04180-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="04180-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="04180-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="04180-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="04180-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="04180-125">Schema Name</span></span>  <br/> |<span data-ttu-id="04180-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="04180-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="04180-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="04180-127">Validation File</span></span>  <br/> |<span data-ttu-id="04180-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="04180-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="04180-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="04180-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="04180-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="04180-130">See also</span></span>



- [<span data-ttu-id="04180-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="04180-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

