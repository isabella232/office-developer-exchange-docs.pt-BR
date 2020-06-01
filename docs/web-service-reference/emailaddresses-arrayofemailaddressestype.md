---
title: EmailAddresses (ArrayOfEmailAddressesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 95084659-aa5a-4bac-8977-00db3b87883e
description: O elemento EmailAddresses especifica uma matriz de todos os endereços de email da pessoa associada.
ms.openlocfilehash: e6132e9ef4ed13ea2546783f65d184fafeed5530
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463416"
---
# <a name="emailaddresses-arrayofemailaddressestype"></a><span data-ttu-id="1c8bd-103">EmailAddresses (ArrayOfEmailAddressesType)</span><span class="sxs-lookup"><span data-stu-id="1c8bd-103">EmailAddresses (ArrayOfEmailAddressesType)</span></span>

<span data-ttu-id="1c8bd-104">O elemento **EmailAddresses** especifica uma matriz de todos os endereços de email da pessoa associada.</span><span class="sxs-lookup"><span data-stu-id="1c8bd-104">The **EmailAddresses** element specifies an array of all email addresses of the associated persona.</span></span> 
  
```XML
<EmailAddresses>
    <Address></Address>
</EmailAddresses>
```

 <span data-ttu-id="1c8bd-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="1c8bd-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1c8bd-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="1c8bd-106">Attributes and elements</span></span>

<span data-ttu-id="1c8bd-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1c8bd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1c8bd-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="1c8bd-108">Attributes</span></span>

<span data-ttu-id="1c8bd-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1c8bd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1c8bd-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1c8bd-110">Child elements</span></span>

|<span data-ttu-id="1c8bd-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1c8bd-111">**Element**</span></span>|<span data-ttu-id="1c8bd-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1c8bd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1c8bd-113">Endereço (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="1c8bd-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="1c8bd-114">Representa um endereço de email totalmente resolvido.</span><span class="sxs-lookup"><span data-stu-id="1c8bd-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1c8bd-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1c8bd-115">Parent elements</span></span>

|<span data-ttu-id="1c8bd-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1c8bd-116">**Element**</span></span>|<span data-ttu-id="1c8bd-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1c8bd-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1c8bd-118">Pessoal</span><span class="sxs-lookup"><span data-stu-id="1c8bd-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="1c8bd-119">Especifica um conjunto de dados persona retornados por uma solicitação **Getpersona** .</span><span class="sxs-lookup"><span data-stu-id="1c8bd-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1c8bd-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="1c8bd-120">Remarks</span></span>

<span data-ttu-id="1c8bd-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1c8bd-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1c8bd-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1c8bd-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1c8bd-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="1c8bd-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1c8bd-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="1c8bd-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1c8bd-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1c8bd-125">Schema Name</span></span>  <br/> |<span data-ttu-id="1c8bd-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="1c8bd-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="1c8bd-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1c8bd-127">Validation File</span></span>  <br/> |<span data-ttu-id="1c8bd-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="1c8bd-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="1c8bd-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="1c8bd-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="1c8bd-130">Também consulte</span><span class="sxs-lookup"><span data-stu-id="1c8bd-130">See also</span></span>



- [<span data-ttu-id="1c8bd-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1c8bd-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

