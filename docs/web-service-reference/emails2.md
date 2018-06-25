---
title: Emails2
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6ad95936-f61b-431a-9d86-df160b5d4b2d
description: O elemento Emails2 contém uma matriz de valores de EmailAddressAttributedValue e os identificadores de suas atribuições de origem para a pessoa associada.
ms.openlocfilehash: 1767d6bfaee335717e33e0345c605025a073335c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752005"
---
# <a name="emails2"></a><span data-ttu-id="eb1ad-103">Emails2</span><span class="sxs-lookup"><span data-stu-id="eb1ad-103">Emails2</span></span>

<span data-ttu-id="eb1ad-104">O elemento **Emails2** contém uma matriz de valores de **EmailAddressAttributedValue** e os identificadores de suas atribuições de origem para a pessoa associada.</span><span class="sxs-lookup"><span data-stu-id="eb1ad-104">The **Emails2** element contains an array of **EmailAddressAttributedValue** values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Emails2>
    <EmailAddressAttributedValue></EmailAddressAttributedValue>
</Emails2>
```

 <span data-ttu-id="eb1ad-105">**ArrayOfEmailAddressAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="eb1ad-105">**ArrayOfEmailAddressAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eb1ad-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="eb1ad-106">Attributes and elements</span></span>

<span data-ttu-id="eb1ad-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="eb1ad-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eb1ad-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="eb1ad-108">Attributes</span></span>

<span data-ttu-id="eb1ad-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="eb1ad-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eb1ad-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="eb1ad-110">Child elements</span></span>

|<span data-ttu-id="eb1ad-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="eb1ad-111">**Element**</span></span>|<span data-ttu-id="eb1ad-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="eb1ad-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eb1ad-113">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="eb1ad-113">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md) <br/> |<span data-ttu-id="eb1ad-114">Especifica uma instância de uma matriz de endereços de email e suas atribuições associadas.</span><span class="sxs-lookup"><span data-stu-id="eb1ad-114">Specifies an instance of an array of email addresses and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="eb1ad-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="eb1ad-115">Parent elements</span></span>

|<span data-ttu-id="eb1ad-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="eb1ad-116">**Element**</span></span>|<span data-ttu-id="eb1ad-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="eb1ad-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eb1ad-118">Pessoa</span><span class="sxs-lookup"><span data-stu-id="eb1ad-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="eb1ad-119">Especifica um conjunto de dados de pessoa retornados por uma solicitação **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="eb1ad-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="eb1ad-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="eb1ad-120">Remarks</span></span>

<span data-ttu-id="eb1ad-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="eb1ad-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="eb1ad-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="eb1ad-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eb1ad-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="eb1ad-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eb1ad-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="eb1ad-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="eb1ad-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="eb1ad-125">Schema Name</span></span>  <br/> |<span data-ttu-id="eb1ad-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="eb1ad-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="eb1ad-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="eb1ad-127">Validation File</span></span>  <br/> |<span data-ttu-id="eb1ad-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="eb1ad-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="eb1ad-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="eb1ad-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="eb1ad-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="eb1ad-130">See also</span></span>



- [<span data-ttu-id="eb1ad-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="eb1ad-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

