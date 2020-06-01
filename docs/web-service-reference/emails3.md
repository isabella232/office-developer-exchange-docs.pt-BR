---
title: Emails3
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4f4dc589-4530-4a35-b2a6-0c83cac23637
description: O elemento Emails3 especifica uma matriz de valores EmailAddressAttributedValue e os identificadores de suas atribuições de origem para o persona associado.
ms.openlocfilehash: 0505b0ea248a3ab2de7ec18a344fa57651f84cca
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460719"
---
# <a name="emails3"></a><span data-ttu-id="1c04a-103">Emails3</span><span class="sxs-lookup"><span data-stu-id="1c04a-103">Emails3</span></span>

<span data-ttu-id="1c04a-104">O elemento **Emails3** especifica uma matriz de valores **EmailAddressAttributedValue** e os identificadores de suas atribuições de origem para o persona associado.</span><span class="sxs-lookup"><span data-stu-id="1c04a-104">The **Emails3** element specifies an array of **EmailAddressAttributedValue** values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Emails3>
    <EmailAddressAttributedValue></EmailAddressAttributedValue>
</Emails3>
```

 <span data-ttu-id="1c04a-105">**ArrayOfEmailAddressAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="1c04a-105">**ArrayOfEmailAddressAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1c04a-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="1c04a-106">Attributes and elements</span></span>

<span data-ttu-id="1c04a-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1c04a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1c04a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="1c04a-108">Attributes</span></span>

<span data-ttu-id="1c04a-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1c04a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1c04a-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1c04a-110">Child elements</span></span>

|<span data-ttu-id="1c04a-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1c04a-111">**Element**</span></span>|<span data-ttu-id="1c04a-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1c04a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1c04a-113">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="1c04a-113">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md) <br/> |<span data-ttu-id="1c04a-114">Especifica uma instância de uma matriz de endereços de email e suas atribuições associadas.</span><span class="sxs-lookup"><span data-stu-id="1c04a-114">Specifies an instance of an array of email addresses and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1c04a-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1c04a-115">Parent elements</span></span>

|<span data-ttu-id="1c04a-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1c04a-116">**Element**</span></span>|<span data-ttu-id="1c04a-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1c04a-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1c04a-118">Pessoal</span><span class="sxs-lookup"><span data-stu-id="1c04a-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="1c04a-119">Especifica um conjunto de dados persona retornados por uma solicitação **Getpersona** .</span><span class="sxs-lookup"><span data-stu-id="1c04a-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1c04a-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="1c04a-120">Remarks</span></span>

<span data-ttu-id="1c04a-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1c04a-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1c04a-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1c04a-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1c04a-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="1c04a-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1c04a-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="1c04a-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1c04a-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1c04a-125">Schema Name</span></span>  <br/> |<span data-ttu-id="1c04a-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="1c04a-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="1c04a-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1c04a-127">Validation File</span></span>  <br/> |<span data-ttu-id="1c04a-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="1c04a-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="1c04a-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="1c04a-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="1c04a-130">Também consulte</span><span class="sxs-lookup"><span data-stu-id="1c04a-130">See also</span></span>



- [<span data-ttu-id="1c04a-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1c04a-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

