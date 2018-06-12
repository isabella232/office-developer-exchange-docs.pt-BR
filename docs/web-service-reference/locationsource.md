---
title: LocationSource
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fc4d77d5-6200-4cf3-848a-1088fec0e0d6
description: O elemento LocationSource Especifica as informações sobre a origem do endereço associado postal, por exemplo, um contato ou um catálogo de telefone.
ms.openlocfilehash: 7f5cf5fcca0a72287593349fcf5090a74225d012
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824248"
---
# <a name="locationsource"></a><span data-ttu-id="57347-103">LocationSource</span><span class="sxs-lookup"><span data-stu-id="57347-103">LocationSource</span></span>

<span data-ttu-id="57347-104">O elemento **LocationSource** Especifica as informações sobre a origem do endereço associado postal, por exemplo, um contato ou um catálogo de telefone.</span><span class="sxs-lookup"><span data-stu-id="57347-104">The **LocationSource** element specifies information about the origin of the associated postal address, for example, a contact or a telephone book.</span></span> 
  
```XML
<LocationSource> None | LocationServices | PhonebookServices | Device | Contact | Resource </LocationSource>
```

 <span data-ttu-id="57347-105">**LocationSourceType**</span><span class="sxs-lookup"><span data-stu-id="57347-105">**LocationSourceType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="57347-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="57347-106">Attributes and elements</span></span>

<span data-ttu-id="57347-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="57347-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="57347-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="57347-108">Attributes</span></span>

<span data-ttu-id="57347-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="57347-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="57347-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="57347-110">Child elements</span></span>

<span data-ttu-id="57347-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="57347-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="57347-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="57347-112">Parent elements</span></span>

<span data-ttu-id="57347-113">[Valor (PersonaPostalAddressType)](value-personapostaladdresstype.md) | [Address (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md)</span><span class="sxs-lookup"><span data-stu-id="57347-113">[Value (PersonaPostalAddressType)](value-personapostaladdresstype.md) | [PostalAddress (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="57347-114">Text value</span><span class="sxs-lookup"><span data-stu-id="57347-114">Text value</span></span>

<span data-ttu-id="57347-115">Os valores de texto para o elemento **LocationSource** estão listados na tabela a seguir:</span><span class="sxs-lookup"><span data-stu-id="57347-115">The text values for the **LocationSource** element are listed in the following table:</span></span> 
  
<span data-ttu-id="57347-116">**Valores de texto do elemento LocationSource**</span><span class="sxs-lookup"><span data-stu-id="57347-116">**LocationSource element text values**</span></span>

|<span data-ttu-id="57347-117">**Valor**</span><span class="sxs-lookup"><span data-stu-id="57347-117">**Value**</span></span>|<span data-ttu-id="57347-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="57347-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="57347-119">None</span><span class="sxs-lookup"><span data-stu-id="57347-119">None</span></span>  <br/> |<span data-ttu-id="57347-120">Não há fonte local.</span><span class="sxs-lookup"><span data-stu-id="57347-120">There is no location source.</span></span>  <br/> |
|<span data-ttu-id="57347-121">LocationServices</span><span class="sxs-lookup"><span data-stu-id="57347-121">LocationServices</span></span>  <br/> |<span data-ttu-id="57347-122">As informações foram obtidas dos serviços de local.</span><span class="sxs-lookup"><span data-stu-id="57347-122">The information was obtained from location services.</span></span>  <br/> |
|<span data-ttu-id="57347-123">PhonebookServices</span><span class="sxs-lookup"><span data-stu-id="57347-123">PhonebookServices</span></span>  <br/> |<span data-ttu-id="57347-124">As informações foram obtidas dos serviços de catálogo telefônico.</span><span class="sxs-lookup"><span data-stu-id="57347-124">The information was obtained from phonebook services.</span></span>  <br/> |
|<span data-ttu-id="57347-125">Dispositivo</span><span class="sxs-lookup"><span data-stu-id="57347-125">Device</span></span>  <br/> |<span data-ttu-id="57347-126">As informações foram obtidas do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="57347-126">The information was obtained from the device.</span></span>  <br/> |
|<span data-ttu-id="57347-127">Contato</span><span class="sxs-lookup"><span data-stu-id="57347-127">Contact</span></span>  <br/> |<span data-ttu-id="57347-128">As informações foi obtidas de um contato.</span><span class="sxs-lookup"><span data-stu-id="57347-128">The information was obtained from a contact.</span></span>  <br/> |
|<span data-ttu-id="57347-129">Recurso</span><span class="sxs-lookup"><span data-stu-id="57347-129">Resource</span></span>  <br/> |<span data-ttu-id="57347-130">As informações foi obtidas de um recurso.</span><span class="sxs-lookup"><span data-stu-id="57347-130">The information was obtained from a resource.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="57347-131">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="57347-131">Remarks</span></span>

<span data-ttu-id="57347-132">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="57347-132">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="57347-133">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="57347-133">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  

