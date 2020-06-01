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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463073"
---
# <a name="stringsetting-soap"></a><span data-ttu-id="9d118-103">StringSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9d118-103">StringSetting (SOAP)</span></span>

<span data-ttu-id="9d118-104">O elemento **StringSetting** representa uma configuração de usuário do valor que é do tipo cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="9d118-104">The **StringSetting** element represents a user setting the value of which is of type string.</span></span> 
  
```XML
<StringSetting>
   <Name/>
   <Value/>
</StringSetting>
```

 <span data-ttu-id="9d118-105">**StringSetting**</span><span class="sxs-lookup"><span data-stu-id="9d118-105">**StringSetting**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9d118-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="9d118-106">Attributes and elements</span></span>

<span data-ttu-id="9d118-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9d118-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9d118-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9d118-108">Attributes</span></span>

<span data-ttu-id="9d118-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9d118-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9d118-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9d118-110">Child elements</span></span>

|<span data-ttu-id="9d118-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9d118-111">**Element**</span></span>|<span data-ttu-id="9d118-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9d118-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d118-113">Nome (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9d118-113">Name (SOAP)</span></span>](name-soap.md) <br/> |<span data-ttu-id="9d118-114">Representa um nome de configuração de usuário.</span><span class="sxs-lookup"><span data-stu-id="9d118-114">Represents a user setting name.</span></span>  <br/> |
|[<span data-ttu-id="9d118-115">Valor (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9d118-115">Value (SOAP)</span></span>](value-soap.md) <br/> |<span data-ttu-id="9d118-116">Representa um valor de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="9d118-116">Represents a user setting value.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9d118-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9d118-117">Parent elements</span></span>

<span data-ttu-id="9d118-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9d118-118">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="9d118-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="9d118-119">Text value</span></span>

<span data-ttu-id="9d118-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9d118-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9d118-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="9d118-121">Remarks</span></span>

<span data-ttu-id="9d118-122">O tipo **StringSetting** estende o tipo **usersetting** .</span><span class="sxs-lookup"><span data-stu-id="9d118-122">The **StringSetting** type extends the **UserSetting** type.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="9d118-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="9d118-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9d118-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="9d118-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="9d118-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9d118-125">Schema Name</span></span>  <br/> |<span data-ttu-id="9d118-126">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="9d118-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="9d118-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9d118-127">Validation File</span></span>  <br/> |<span data-ttu-id="9d118-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9d118-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9d118-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9d118-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="9d118-130">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="9d118-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9d118-131">Também consulte</span><span class="sxs-lookup"><span data-stu-id="9d118-131">See also</span></span>



[<span data-ttu-id="9d118-132">Operação GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9d118-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="9d118-133">Operação GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9d118-133">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="9d118-134">Operação GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9d118-134">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

