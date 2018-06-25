---
title: EmailAddresses (ArrayOfEmailAddressesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 95084659-aa5a-4bac-8977-00db3b87883e
description: O elemento EmailAddresses Especifica uma matriz de todos os endereços de email da pessoa a associado.
ms.openlocfilehash: 292d4c3f12b01f25fd094b2ab6d9c2d484d37694
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752002"
---
# <a name="emailaddresses-arrayofemailaddressestype"></a><span data-ttu-id="b8ff0-103">EmailAddresses (ArrayOfEmailAddressesType)</span><span class="sxs-lookup"><span data-stu-id="b8ff0-103">EmailAddresses (ArrayOfEmailAddressesType)</span></span>

<span data-ttu-id="b8ff0-104">O elemento **EmailAddresses** Especifica uma matriz de todos os endereços de email da pessoa a associado.</span><span class="sxs-lookup"><span data-stu-id="b8ff0-104">The **EmailAddresses** element specifies an array of all email addresses of the associated persona.</span></span> 
  
```XML
<EmailAddresses>
    <Address></Address>
</EmailAddresses>
```

 <span data-ttu-id="b8ff0-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="b8ff0-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b8ff0-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b8ff0-106">Attributes and elements</span></span>

<span data-ttu-id="b8ff0-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b8ff0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b8ff0-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b8ff0-108">Attributes</span></span>

<span data-ttu-id="b8ff0-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b8ff0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b8ff0-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b8ff0-110">Child elements</span></span>

|<span data-ttu-id="b8ff0-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b8ff0-111">**Element**</span></span>|<span data-ttu-id="b8ff0-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b8ff0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b8ff0-113">Endereço (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="b8ff0-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="b8ff0-114">Representa um endereço de email totalmente resolvido.</span><span class="sxs-lookup"><span data-stu-id="b8ff0-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b8ff0-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b8ff0-115">Parent elements</span></span>

|<span data-ttu-id="b8ff0-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b8ff0-116">**Element**</span></span>|<span data-ttu-id="b8ff0-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b8ff0-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b8ff0-118">Pessoa</span><span class="sxs-lookup"><span data-stu-id="b8ff0-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="b8ff0-119">Especifica um conjunto de dados de pessoa retornados por uma solicitação **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="b8ff0-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b8ff0-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="b8ff0-120">Remarks</span></span>

<span data-ttu-id="b8ff0-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b8ff0-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b8ff0-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b8ff0-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b8ff0-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b8ff0-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b8ff0-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="b8ff0-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b8ff0-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b8ff0-125">Schema Name</span></span>  <br/> |<span data-ttu-id="b8ff0-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="b8ff0-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="b8ff0-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b8ff0-127">Validation File</span></span>  <br/> |<span data-ttu-id="b8ff0-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b8ff0-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="b8ff0-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="b8ff0-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="b8ff0-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="b8ff0-130">See also</span></span>



- [<span data-ttu-id="b8ff0-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b8ff0-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

