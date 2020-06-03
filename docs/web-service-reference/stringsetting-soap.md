---
title: StringSetting (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: bf7096d8-42d4-4bf5-bbdd-851af2754000
description: O elemento StringSetting representa uma configuração de usuário do valor que é do tipo cadeia de caracteres.
ms.openlocfilehash: 215d1187c0968577e894c9f9cddea050789697b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463073"
---
# <a name="stringsetting-soap"></a><span data-ttu-id="61273-103">StringSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="61273-103">StringSetting (SOAP)</span></span>

<span data-ttu-id="61273-104">O elemento **StringSetting** representa uma configuração de usuário do valor que é do tipo cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="61273-104">The **StringSetting** element represents a user setting the value of which is of type string.</span></span> 
  
```XML
<StringSetting>
   <Name/>
   <Value/>
</StringSetting>
```

 <span data-ttu-id="61273-105">**StringSetting**</span><span class="sxs-lookup"><span data-stu-id="61273-105">**StringSetting**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="61273-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="61273-106">Attributes and elements</span></span>

<span data-ttu-id="61273-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="61273-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="61273-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="61273-108">Attributes</span></span>

<span data-ttu-id="61273-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="61273-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="61273-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="61273-110">Child elements</span></span>

|<span data-ttu-id="61273-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="61273-111">**Element**</span></span>|<span data-ttu-id="61273-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="61273-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="61273-113">Nome (SOAP)</span><span class="sxs-lookup"><span data-stu-id="61273-113">Name (SOAP)</span></span>](name-soap.md) <br/> |<span data-ttu-id="61273-114">Representa um nome de configuração de usuário.</span><span class="sxs-lookup"><span data-stu-id="61273-114">Represents a user setting name.</span></span>  <br/> |
|[<span data-ttu-id="61273-115">Valor (SOAP)</span><span class="sxs-lookup"><span data-stu-id="61273-115">Value (SOAP)</span></span>](value-soap.md) <br/> |<span data-ttu-id="61273-116">Representa um valor de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="61273-116">Represents a user setting value.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="61273-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="61273-117">Parent elements</span></span>

<span data-ttu-id="61273-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="61273-118">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="61273-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="61273-119">Text value</span></span>

<span data-ttu-id="61273-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="61273-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="61273-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="61273-121">Remarks</span></span>

<span data-ttu-id="61273-122">O tipo **StringSetting** estende o tipo **usersetting** .</span><span class="sxs-lookup"><span data-stu-id="61273-122">The **StringSetting** type extends the **UserSetting** type.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="61273-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="61273-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="61273-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="61273-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="61273-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="61273-125">Schema Name</span></span>  <br/> |<span data-ttu-id="61273-126">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="61273-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="61273-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="61273-127">Validation File</span></span>  <br/> |<span data-ttu-id="61273-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="61273-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="61273-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="61273-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="61273-130">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="61273-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="61273-131">Confira também</span><span class="sxs-lookup"><span data-stu-id="61273-131">See also</span></span>



[<span data-ttu-id="61273-132">Operação GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="61273-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="61273-133">Operação GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="61273-133">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="61273-134">Operação GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="61273-134">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

