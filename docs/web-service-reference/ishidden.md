---
title: IsHidden
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2377b584-bd1e-49fc-b80a-a6634721a297
description: O elemento IsHidden contém um valor Boolean que indica se o contato subjacente deve oculto ou exibido como parte da pessoa.
ms.openlocfilehash: ee20bf0af287e3cddaedb5bc6d3c63ef9a7a7006
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824032"
---
# <a name="ishidden"></a><span data-ttu-id="817bb-103">IsHidden</span><span class="sxs-lookup"><span data-stu-id="817bb-103">IsHidden</span></span>

<span data-ttu-id="817bb-104">O elemento **IsHidden** contém um valor Boolean que indica se o contato subjacente deve oculto ou exibido como parte da pessoa.</span><span class="sxs-lookup"><span data-stu-id="817bb-104">The **IsHidden** element contains a Boolean value that indicates whether the underlying contact should be hidden or displayed as part of the persona.</span></span> 
  
```XML
<IsHidden>true | false</IsHidden>
```

 <span data-ttu-id="817bb-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="817bb-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="817bb-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="817bb-106">Attributes and elements</span></span>

<span data-ttu-id="817bb-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="817bb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="817bb-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="817bb-108">Attributes</span></span>

<span data-ttu-id="817bb-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="817bb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="817bb-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="817bb-110">Child elements</span></span>

<span data-ttu-id="817bb-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="817bb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="817bb-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="817bb-112">Parent elements</span></span>

|<span data-ttu-id="817bb-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="817bb-113">**Element**</span></span>|<span data-ttu-id="817bb-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="817bb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="817bb-115">Atribuição (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="817bb-115">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md) <br/> |<span data-ttu-id="817bb-116">Especifica uma instância em uma matriz de atributos de um elemento de **pessoa** .</span><span class="sxs-lookup"><span data-stu-id="817bb-116">Specifies an instance in an array of attributes for a **Persona** element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="817bb-117">Text value</span><span class="sxs-lookup"><span data-stu-id="817bb-117">Text value</span></span>

<span data-ttu-id="817bb-118">Um valor de texto de **true** para o elemento **IsHidden** indica que o contato subjacente deve ser oculto ou exibido como parte da pessoa.</span><span class="sxs-lookup"><span data-stu-id="817bb-118">A text value of **true** for the **IsHidden** element indicates that the underlying contact should be hidden or displayed as part of the persona.</span></span> <span data-ttu-id="817bb-119">Um valor **false** indica que o contato subjacente não deve ser oculto ou exibido como parte da pessoa.</span><span class="sxs-lookup"><span data-stu-id="817bb-119">A value of **false** indicates that the underlying contact should not be hidden or displayed as part of the persona.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="817bb-120">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="817bb-120">Remarks</span></span>

<span data-ttu-id="817bb-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="817bb-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="817bb-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="817bb-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="817bb-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="817bb-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="817bb-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="817bb-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="817bb-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="817bb-125">Schema Name</span></span>  <br/> |<span data-ttu-id="817bb-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="817bb-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="817bb-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="817bb-127">Validation File</span></span>  <br/> |<span data-ttu-id="817bb-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="817bb-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="817bb-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="817bb-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="817bb-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="817bb-130">See also</span></span>



- [<span data-ttu-id="817bb-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="817bb-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

