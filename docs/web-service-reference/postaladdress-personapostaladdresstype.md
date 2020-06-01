---
title: Address (PersonaPostalAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 075f7d65-9d05-47cb-af26-0dd6d5593439
description: O elemento address especifica o endereço postal de um persona.
ms.openlocfilehash: 9e316e5e0135c2d18fab4067241988c65eceec66
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465384"
---
# <a name="postaladdress-personapostaladdresstype"></a><span data-ttu-id="6ac58-103">Address (PersonaPostalAddressType)</span><span class="sxs-lookup"><span data-stu-id="6ac58-103">PostalAddress (PersonaPostalAddressType)</span></span>

<span data-ttu-id="6ac58-104">O elemento **Address** especifica o endereço postal de um persona.</span><span class="sxs-lookup"><span data-stu-id="6ac58-104">The **PostalAddress** element specifies the postal address for a persona.</span></span> 
  
```XML
<PostalAddress>
   <Street/>
   <City/>
   <State/>
   <Country/>
   <PostalCode/>
   <PostOfficeBox/>
   <Type/>
   <Latitude/>
   <Longitude/>
   <Accuracy/>
   <Altitude/>
   <AltitudeAccuracy/>
   <FormattedAddress/>
   <LocationUri/>
   <LocationSource/>
</PostalAddress>
```

 <span data-ttu-id="6ac58-105">**PersonaPostalAddressType**</span><span class="sxs-lookup"><span data-stu-id="6ac58-105">**PersonaPostalAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6ac58-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="6ac58-106">Attributes and elements</span></span>

<span data-ttu-id="6ac58-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6ac58-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6ac58-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="6ac58-108">Attributes</span></span>

<span data-ttu-id="6ac58-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6ac58-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6ac58-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6ac58-110">Child elements</span></span>

<span data-ttu-id="6ac58-111">[Rua](street.md)  |  [Cidade](city.md)  |  [Estado](state-ex15websvcsotherref.md)  |  [País/região](country.md)  |  [PostalCode](postalcode.md)  |  [PostOfficeBox](postofficebox.md)  |  [Tipo (cadeia de caracteres)](type-string.md)  |  [Latitude](latitude.md)  |  [Longitude](longitude.md)  |  [Precisão](accuracy.md)  |  [Altitude](altitude.md)  |  [AltitudeAccuracy](altitudeaccuracy.md)  |  [FormattedAddress](formattedaddress.md)  |  [LocationUri](locationuri.md)  |  [Localização](locationsource.md)</span><span class="sxs-lookup"><span data-stu-id="6ac58-111">[Street](street.md) | [City](city.md) | [State](state-ex15websvcsotherref.md) | [Country](country.md) | [PostalCode](postalcode.md) | [PostOfficeBox](postofficebox.md) | [Type (string)](type-string.md) | [Latitude](latitude.md) | [Longitude](longitude.md) | [Accuracy](accuracy.md) | [Altitude](altitude.md) | [AltitudeAccuracy](altitudeaccuracy.md) | [FormattedAddress](formattedaddress.md) | [LocationUri](locationuri.md) | [LocationSource](locationsource.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6ac58-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6ac58-112">Parent elements</span></span>

[<span data-ttu-id="6ac58-113">EnhancedLocation</span><span class="sxs-lookup"><span data-stu-id="6ac58-113">EnhancedLocation</span></span>](enhancedlocation.md)
  
## <a name="remarks"></a><span data-ttu-id="6ac58-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="6ac58-114">Remarks</span></span>

<span data-ttu-id="6ac58-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6ac58-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6ac58-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6ac58-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6ac58-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="6ac58-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6ac58-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="6ac58-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6ac58-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6ac58-119">Schema name</span></span>  <br/> |<span data-ttu-id="6ac58-120">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="6ac58-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="6ac58-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6ac58-121">Validation file</span></span>  <br/> |<span data-ttu-id="6ac58-122">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="6ac58-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6ac58-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="6ac58-123">Can be empty</span></span>  <br/> ||
   

