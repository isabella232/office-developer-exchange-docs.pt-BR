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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752002"
---
# <a name="emailaddresses-arrayofemailaddressestype"></a><span data-ttu-id="97c89-103">EmailAddresses (ArrayOfEmailAddressesType)</span><span class="sxs-lookup"><span data-stu-id="97c89-103">EmailAddresses (ArrayOfEmailAddressesType)</span></span>

<span data-ttu-id="97c89-104">O elemento **EmailAddresses** Especifica uma matriz de todos os endereços de email da pessoa a associado.</span><span class="sxs-lookup"><span data-stu-id="97c89-104">The **EmailAddresses** element specifies an array of all email addresses of the associated persona.</span></span> 
  
```XML
<EmailAddresses>
    <Address></Address>
</EmailAddresses>
```

 <span data-ttu-id="97c89-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="97c89-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="97c89-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="97c89-106">Attributes and elements</span></span>

<span data-ttu-id="97c89-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="97c89-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="97c89-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="97c89-108">Attributes</span></span>

<span data-ttu-id="97c89-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="97c89-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="97c89-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="97c89-110">Child elements</span></span>

|<span data-ttu-id="97c89-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="97c89-111">**Element**</span></span>|<span data-ttu-id="97c89-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="97c89-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97c89-113">Endereço (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="97c89-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="97c89-114">Representa um endereço de email totalmente resolvido.</span><span class="sxs-lookup"><span data-stu-id="97c89-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="97c89-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="97c89-115">Parent elements</span></span>

|<span data-ttu-id="97c89-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="97c89-116">**Element**</span></span>|<span data-ttu-id="97c89-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="97c89-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97c89-118">Pessoa</span><span class="sxs-lookup"><span data-stu-id="97c89-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="97c89-119">Especifica um conjunto de dados de pessoa retornados por uma solicitação **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="97c89-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="97c89-120">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="97c89-120">Remarks</span></span>

<span data-ttu-id="97c89-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="97c89-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="97c89-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="97c89-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="97c89-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="97c89-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="97c89-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="97c89-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="97c89-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="97c89-125">Schema Name</span></span>  <br/> |<span data-ttu-id="97c89-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="97c89-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="97c89-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="97c89-127">Validation File</span></span>  <br/> |<span data-ttu-id="97c89-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="97c89-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="97c89-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="97c89-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="97c89-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="97c89-130">See also</span></span>



- [<span data-ttu-id="97c89-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="97c89-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

