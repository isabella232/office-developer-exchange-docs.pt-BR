---
title: Localização
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fc4d77d5-6200-4cf3-848a-1088fec0e0d6
description: O elemento LocalName especifica informações sobre a origem do endereço postal associado, por exemplo, um contato ou um catálogo telefônico.
ms.openlocfilehash: ceba52c43d1c798bb8f5492b779c7c45d7d00b0b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467099"
---
# <a name="locationsource"></a><span data-ttu-id="5d41d-103">Localização</span><span class="sxs-lookup"><span data-stu-id="5d41d-103">LocationSource</span></span>

<span data-ttu-id="5d41d-104">O elemento **LocalName** especifica informações sobre a origem do endereço postal associado, por exemplo, um contato ou um catálogo telefônico.</span><span class="sxs-lookup"><span data-stu-id="5d41d-104">The **LocationSource** element specifies information about the origin of the associated postal address, for example, a contact or a telephone book.</span></span> 
  
```XML
<LocationSource> None | LocationServices | PhonebookServices | Device | Contact | Resource </LocationSource>
```

 <span data-ttu-id="5d41d-105">**LocationSourceType**</span><span class="sxs-lookup"><span data-stu-id="5d41d-105">**LocationSourceType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5d41d-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5d41d-106">Attributes and elements</span></span>

<span data-ttu-id="5d41d-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5d41d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5d41d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5d41d-108">Attributes</span></span>

<span data-ttu-id="5d41d-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5d41d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5d41d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5d41d-110">Child elements</span></span>

<span data-ttu-id="5d41d-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5d41d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5d41d-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5d41d-112">Parent elements</span></span>

<span data-ttu-id="5d41d-113">[Valor (PersonaPostalAddressType)](value-personapostaladdresstype.md)  |  [Address (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md)</span><span class="sxs-lookup"><span data-stu-id="5d41d-113">[Value (PersonaPostalAddressType)](value-personapostaladdresstype.md) | [PostalAddress (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="5d41d-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="5d41d-114">Text value</span></span>

<span data-ttu-id="5d41d-115">Os valores de texto para o elemento **LocationName** estão listados na tabela a seguir:</span><span class="sxs-lookup"><span data-stu-id="5d41d-115">The text values for the **LocationSource** element are listed in the following table:</span></span> 
  
<span data-ttu-id="5d41d-116">**Valores de texto do elemento local**</span><span class="sxs-lookup"><span data-stu-id="5d41d-116">**LocationSource element text values**</span></span>

|<span data-ttu-id="5d41d-117">**Valor**</span><span class="sxs-lookup"><span data-stu-id="5d41d-117">**Value**</span></span>|<span data-ttu-id="5d41d-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5d41d-118">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5d41d-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5d41d-119">None</span></span>  <br/> |<span data-ttu-id="5d41d-120">Não há nenhuma origem de local.</span><span class="sxs-lookup"><span data-stu-id="5d41d-120">There is no location source.</span></span>  <br/> |
|<span data-ttu-id="5d41d-121">LocalServices</span><span class="sxs-lookup"><span data-stu-id="5d41d-121">LocationServices</span></span>  <br/> |<span data-ttu-id="5d41d-122">As informações foram obtidas dos serviços de localização.</span><span class="sxs-lookup"><span data-stu-id="5d41d-122">The information was obtained from location services.</span></span>  <br/> |
|<span data-ttu-id="5d41d-123">Catálogos telefônicos</span><span class="sxs-lookup"><span data-stu-id="5d41d-123">PhonebookServices</span></span>  <br/> |<span data-ttu-id="5d41d-124">As informações foram obtidas de serviços de catálogo telefônico.</span><span class="sxs-lookup"><span data-stu-id="5d41d-124">The information was obtained from phonebook services.</span></span>  <br/> |
|<span data-ttu-id="5d41d-125">Dispositivo</span><span class="sxs-lookup"><span data-stu-id="5d41d-125">Device</span></span>  <br/> |<span data-ttu-id="5d41d-126">As informações foram obtidas do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5d41d-126">The information was obtained from the device.</span></span>  <br/> |
|<span data-ttu-id="5d41d-127">Contato</span><span class="sxs-lookup"><span data-stu-id="5d41d-127">Contact</span></span>  <br/> |<span data-ttu-id="5d41d-128">As informações foram obtidas de um contato.</span><span class="sxs-lookup"><span data-stu-id="5d41d-128">The information was obtained from a contact.</span></span>  <br/> |
|<span data-ttu-id="5d41d-129">Resource</span><span class="sxs-lookup"><span data-stu-id="5d41d-129">Resource</span></span>  <br/> |<span data-ttu-id="5d41d-130">As informações foram obtidas de um recurso.</span><span class="sxs-lookup"><span data-stu-id="5d41d-130">The information was obtained from a resource.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5d41d-131">Comentários</span><span class="sxs-lookup"><span data-stu-id="5d41d-131">Remarks</span></span>

<span data-ttu-id="5d41d-132">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5d41d-132">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5d41d-133">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5d41d-133">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  

