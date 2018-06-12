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
description: O elemento StringSetting representa uma configuração de usuário que o valor da qual é do tipo string.
ms.openlocfilehash: af2c8ed243182e3491723be172ae162554250951
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825606"
---
# <a name="stringsetting-soap"></a><span data-ttu-id="742d2-103">StringSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="742d2-103">StringSetting (SOAP)</span></span>

<span data-ttu-id="742d2-104">O elemento **StringSetting** representa uma configuração de usuário que o valor da qual é do tipo string.</span><span class="sxs-lookup"><span data-stu-id="742d2-104">The **StringSetting** element represents a user setting the value of which is of type string.</span></span> 
  
```XML
<StringSetting>
   <Name/>
   <Value/>
</StringSetting>
```

 <span data-ttu-id="742d2-105">**StringSetting**</span><span class="sxs-lookup"><span data-stu-id="742d2-105">**StringSetting**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="742d2-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="742d2-106">Attributes and elements</span></span>

<span data-ttu-id="742d2-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="742d2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="742d2-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="742d2-108">Attributes</span></span>

<span data-ttu-id="742d2-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="742d2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="742d2-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="742d2-110">Child elements</span></span>

|<span data-ttu-id="742d2-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="742d2-111">**Element**</span></span>|<span data-ttu-id="742d2-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="742d2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="742d2-113">Nome (SOAP)</span><span class="sxs-lookup"><span data-stu-id="742d2-113">Name (SOAP)</span></span>](name-soap.md) <br/> |<span data-ttu-id="742d2-114">Representa um nome de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="742d2-114">Represents a user setting name.</span></span>  <br/> |
|[<span data-ttu-id="742d2-115">Valor (SOAP)</span><span class="sxs-lookup"><span data-stu-id="742d2-115">Value (SOAP)</span></span>](value-soap.md) <br/> |<span data-ttu-id="742d2-116">Representa um valor de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="742d2-116">Represents a user setting value.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="742d2-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="742d2-117">Parent elements</span></span>

<span data-ttu-id="742d2-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="742d2-118">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="742d2-119">Text value</span><span class="sxs-lookup"><span data-stu-id="742d2-119">Text value</span></span>

<span data-ttu-id="742d2-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="742d2-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="742d2-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="742d2-121">Remarks</span></span>

<span data-ttu-id="742d2-122">O tipo de **StringSetting** estende o tipo de **UserSetting** .</span><span class="sxs-lookup"><span data-stu-id="742d2-122">The **StringSetting** type extends the **UserSetting** type.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="742d2-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="742d2-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="742d2-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="742d2-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="742d2-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="742d2-125">Schema Name</span></span>  <br/> |<span data-ttu-id="742d2-126">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="742d2-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="742d2-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="742d2-127">Validation File</span></span>  <br/> |<span data-ttu-id="742d2-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="742d2-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="742d2-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="742d2-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="742d2-130">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="742d2-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="742d2-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="742d2-131">See also</span></span>



[<span data-ttu-id="742d2-132">Operação de GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="742d2-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="742d2-133">Operação de GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="742d2-133">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="742d2-134">Operação de GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="742d2-134">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

