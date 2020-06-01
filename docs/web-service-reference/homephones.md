---
title: HomePhones
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8ea43d5a-4bcf-497e-a559-6efe94fa604b
description: O elemento HomePhones especifica uma matriz de números de telefone residenciais e os identificadores de suas atribuições de origem para o persona associado.
ms.openlocfilehash: b55d6ca752a5b00a27eb158c6a22412a9f4ecdda
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460831"
---
# <a name="homephones"></a><span data-ttu-id="2e403-103">HomePhones</span><span class="sxs-lookup"><span data-stu-id="2e403-103">HomePhones</span></span>

<span data-ttu-id="2e403-104">O elemento **HomePhones** especifica uma matriz de números de telefone residenciais e os identificadores de suas atribuições de origem para o persona associado.</span><span class="sxs-lookup"><span data-stu-id="2e403-104">The **HomePhones** element specifies an array of home phone numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<HomePhones>
    <PhoneNumberAttributedValue/>
</HomePhones>
```

 <span data-ttu-id="2e403-105">**ArrayOfPhoneNumberAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="2e403-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2e403-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="2e403-106">Attributes and elements</span></span>

<span data-ttu-id="2e403-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2e403-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2e403-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2e403-108">Attributes</span></span>

<span data-ttu-id="2e403-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2e403-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2e403-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2e403-110">Child elements</span></span>

|<span data-ttu-id="2e403-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2e403-111">**Element**</span></span>|<span data-ttu-id="2e403-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2e403-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2e403-113">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="2e403-113">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md) <br/> |<span data-ttu-id="2e403-114">Contém um único número de telefone atribuído para uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="2e403-114">Contains a single attributed phone number for a persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2e403-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2e403-115">Parent elements</span></span>

|<span data-ttu-id="2e403-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2e403-116">**Element**</span></span>|<span data-ttu-id="2e403-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2e403-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2e403-118">Pessoal</span><span class="sxs-lookup"><span data-stu-id="2e403-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="2e403-119">Especifica um conjunto de dados persona retornados por uma solicitação **Getpersona** .</span><span class="sxs-lookup"><span data-stu-id="2e403-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2e403-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="2e403-120">Remarks</span></span>

<span data-ttu-id="2e403-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2e403-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2e403-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2e403-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2e403-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="2e403-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2e403-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="2e403-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2e403-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2e403-125">Schema Name</span></span>  <br/> |<span data-ttu-id="2e403-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="2e403-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="2e403-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2e403-127">Validation File</span></span>  <br/> |<span data-ttu-id="2e403-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2e403-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="2e403-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="2e403-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="2e403-130">Também consulte</span><span class="sxs-lookup"><span data-stu-id="2e403-130">See also</span></span>



- [<span data-ttu-id="2e403-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2e403-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

