---
title: Valor (PersonaPostalAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: be838fc2-cfcb-4856-b095-a8e5366bb6c6
description: O elemento de valor especifica informações associado a um endereço postal.
ms.openlocfilehash: 048d3a49552f1a9e89744e4cd16ec1745417e923
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838022"
---
# <a name="value-personapostaladdresstype"></a><span data-ttu-id="4b1ce-103">Valor (PersonaPostalAddressType)</span><span class="sxs-lookup"><span data-stu-id="4b1ce-103">Value (PersonaPostalAddressType)</span></span>

<span data-ttu-id="4b1ce-104">O elemento de **valor** Especifica informações associadas a um endereço postal.</span><span class="sxs-lookup"><span data-stu-id="4b1ce-104">The **Value** element specifies information associated with a postal address.</span></span> 
  
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

<span data-ttu-id="4b1ce-105">**PersonaPostalAddressType**</span><span class="sxs-lookup"><span data-stu-id="4b1ce-105">**PersonaPostalAddressType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4b1ce-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="4b1ce-106">Attributes and elements</span></span>

<span data-ttu-id="4b1ce-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4b1ce-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4b1ce-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4b1ce-108">Attributes</span></span>

<span data-ttu-id="4b1ce-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4b1ce-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4b1ce-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4b1ce-110">Child elements</span></span>

<span data-ttu-id="4b1ce-111">[Rua](street.md) | [City](city.md) | [estado](state-ex15websvcsotherref.md) | [país](country.md) | [PostalCode](postalcode.md) | [PostOfficeBox](postofficebox.md) | [tipo (string)](type-string.md) | [Latitude](latitude.md)  |  [ Longitude](longitude.md) | [precisão](accuracy.md) | [Altitude](altitude.md) | [AltitudeAccuracy](altitudeaccuracy.md) | [FormattedAddress](formattedaddress.md) | [LocationUri](locationuri.md) | [LocationSource](locationsource.md)</span><span class="sxs-lookup"><span data-stu-id="4b1ce-111">[Street](street.md) | [City](city.md) | [State](state-ex15websvcsotherref.md) | [Country](country.md) | [PostalCode](postalcode.md) | [PostOfficeBox](postofficebox.md) | [Type (string)](type-string.md) | [Latitude](latitude.md) | [Longitude](longitude.md) | [Accuracy](accuracy.md) | [Altitude](altitude.md) | [AltitudeAccuracy](altitudeaccuracy.md) | [FormattedAddress](formattedaddress.md) | [LocationUri](locationuri.md) | [LocationSource](locationsource.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4b1ce-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4b1ce-112">Parent elements</span></span>

[<span data-ttu-id="4b1ce-113">PostalAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="4b1ce-113">PostalAddressAttributedValue</span></span>](postaladdressattributedvalue.md)
  
## <a name="remarks"></a><span data-ttu-id="4b1ce-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="4b1ce-114">Remarks</span></span>

<span data-ttu-id="4b1ce-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4b1ce-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4b1ce-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4b1ce-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4b1ce-117">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="4b1ce-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4b1ce-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="4b1ce-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4b1ce-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4b1ce-119">Schema name</span></span>  <br/> |<span data-ttu-id="4b1ce-120">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="4b1ce-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="4b1ce-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4b1ce-121">Validation file</span></span>  <br/> |<span data-ttu-id="4b1ce-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4b1ce-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4b1ce-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="4b1ce-123">Can be empty</span></span>  <br/> ||
   

