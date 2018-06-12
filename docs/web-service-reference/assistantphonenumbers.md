---
title: AssistantPhoneNumbers
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9bd9ac1-7db3-44ea-9117-18488dddde15
description: O elemento AssistantPhoneNumbers Especifica uma matriz de números de telefone do assistente e os identificadores de suas atribuições de origem para a pessoa associada.
ms.openlocfilehash: 747835102af28d94d60b763fdbc5b2ea0947d47e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751215"
---
# <a name="assistantphonenumbers"></a><span data-ttu-id="4ff42-103">AssistantPhoneNumbers</span><span class="sxs-lookup"><span data-stu-id="4ff42-103">AssistantPhoneNumbers</span></span>

<span data-ttu-id="4ff42-104">O elemento **AssistantPhoneNumbers** Especifica uma matriz de números de telefone do assistente e os identificadores de suas atribuições de origem para a pessoa associada.</span><span class="sxs-lookup"><span data-stu-id="4ff42-104">The **AssistantPhoneNumbers** element specifies an array of assistant phone numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<AssistantPhoneNumbers>
    <PhoneNumberAttributedValue></PhoneNumberAttributedValue>
</AssistantPhoneNumbers>
```

 <span data-ttu-id="4ff42-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="4ff42-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4ff42-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="4ff42-106">Attributes and elements</span></span>

<span data-ttu-id="4ff42-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4ff42-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4ff42-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4ff42-108">Attributes</span></span>

<span data-ttu-id="4ff42-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4ff42-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4ff42-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4ff42-110">Child elements</span></span>

|<span data-ttu-id="4ff42-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4ff42-111">**Element**</span></span>|<span data-ttu-id="4ff42-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4ff42-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ff42-113">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="4ff42-113">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md) <br/> |<span data-ttu-id="4ff42-114">Especifica uma instância de uma matriz de números de telefone e suas atribuições associadas.</span><span class="sxs-lookup"><span data-stu-id="4ff42-114">Specifies an instance of an array of phone numbers and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4ff42-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4ff42-115">Parent elements</span></span>

|<span data-ttu-id="4ff42-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4ff42-116">**Element**</span></span>|<span data-ttu-id="4ff42-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4ff42-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ff42-118">Pessoa</span><span class="sxs-lookup"><span data-stu-id="4ff42-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="4ff42-119">Especifica um conjunto de dados de pessoa retornados por uma solicitação **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="4ff42-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4ff42-120">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="4ff42-120">Remarks</span></span>

<span data-ttu-id="4ff42-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4ff42-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4ff42-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4ff42-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4ff42-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="4ff42-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4ff42-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="4ff42-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4ff42-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4ff42-125">Schema Name</span></span>  <br/> |<span data-ttu-id="4ff42-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="4ff42-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="4ff42-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4ff42-127">Validation File</span></span>  <br/> |<span data-ttu-id="4ff42-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4ff42-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="4ff42-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="4ff42-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4ff42-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="4ff42-130">See also</span></span>

- [<span data-ttu-id="4ff42-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4ff42-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

