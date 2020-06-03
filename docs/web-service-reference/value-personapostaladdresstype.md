---
title: Valor (PersonaPostalAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: be838fc2-cfcb-4856-b095-a8e5366bb6c6
description: O elemento Value especifica informações associadas a um endereço postal.
ms.openlocfilehash: 2d644ff45fe89061ccd90279773f3a5a5b7fe7cc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466469"
---
# <a name="value-personapostaladdresstype"></a><span data-ttu-id="00387-103">Valor (PersonaPostalAddressType)</span><span class="sxs-lookup"><span data-stu-id="00387-103">Value (PersonaPostalAddressType)</span></span>

<span data-ttu-id="00387-104">O elemento **Value** especifica informações associadas a um endereço postal.</span><span class="sxs-lookup"><span data-stu-id="00387-104">The **Value** element specifies information associated with a postal address.</span></span> 
  
```XML
<Value>
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
</Value>
```

<span data-ttu-id="00387-105">**PersonaPostalAddressType**</span><span class="sxs-lookup"><span data-stu-id="00387-105">**PersonaPostalAddressType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="00387-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="00387-106">Attributes and elements</span></span>

<span data-ttu-id="00387-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="00387-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="00387-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="00387-108">Attributes</span></span>

<span data-ttu-id="00387-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="00387-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="00387-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="00387-110">Child elements</span></span>

<span data-ttu-id="00387-111">[Rua](street.md)  |  [Cidade](city.md)  |  [Estado](state-ex15websvcsotherref.md)  |  [País/região](country.md)  |  [PostalCode](postalcode.md)  |  [PostOfficeBox](postofficebox.md)  |  [Tipo (cadeia de caracteres)](type-string.md)  |  [Latitude](latitude.md)  |  [Longitude](longitude.md)  |  [Precisão](accuracy.md)  |  [Altitude](altitude.md)  |  [AltitudeAccuracy](altitudeaccuracy.md)  |  [FormattedAddress](formattedaddress.md)  |  [LocationUri](locationuri.md)  |  [Localização](locationsource.md)</span><span class="sxs-lookup"><span data-stu-id="00387-111">[Street](street.md) | [City](city.md) | [State](state-ex15websvcsotherref.md) | [Country](country.md) | [PostalCode](postalcode.md) | [PostOfficeBox](postofficebox.md) | [Type (string)](type-string.md) | [Latitude](latitude.md) | [Longitude](longitude.md) | [Accuracy](accuracy.md) | [Altitude](altitude.md) | [AltitudeAccuracy](altitudeaccuracy.md) | [FormattedAddress](formattedaddress.md) | [LocationUri](locationuri.md) | [LocationSource](locationsource.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="00387-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="00387-112">Parent elements</span></span>

[<span data-ttu-id="00387-113">PostalAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="00387-113">PostalAddressAttributedValue</span></span>](postaladdressattributedvalue.md)
  
## <a name="remarks"></a><span data-ttu-id="00387-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="00387-114">Remarks</span></span>

<span data-ttu-id="00387-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="00387-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="00387-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="00387-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="00387-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="00387-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="00387-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="00387-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="00387-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="00387-119">Schema name</span></span>  <br/> |<span data-ttu-id="00387-120">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="00387-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="00387-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="00387-121">Validation file</span></span>  <br/> |<span data-ttu-id="00387-122">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="00387-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="00387-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="00387-123">Can be empty</span></span>  <br/> ||
   

