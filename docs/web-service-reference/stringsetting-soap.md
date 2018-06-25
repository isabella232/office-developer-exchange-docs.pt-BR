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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825606"
---
# <a name="stringsetting-soap"></a><span data-ttu-id="aaa21-103">StringSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="aaa21-103">StringSetting (SOAP)</span></span>

<span data-ttu-id="aaa21-104">O elemento **StringSetting** representa uma configuração de usuário que o valor da qual é do tipo string.</span><span class="sxs-lookup"><span data-stu-id="aaa21-104">The **StringSetting** element represents a user setting the value of which is of type string.</span></span> 
  
```XML
<StringSetting>
   <Name/>
   <Value/>
</StringSetting>
```

 <span data-ttu-id="aaa21-105">**StringSetting**</span><span class="sxs-lookup"><span data-stu-id="aaa21-105">**StringSetting**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aaa21-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="aaa21-106">Attributes and elements</span></span>

<span data-ttu-id="aaa21-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="aaa21-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aaa21-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="aaa21-108">Attributes</span></span>

<span data-ttu-id="aaa21-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="aaa21-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aaa21-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="aaa21-110">Child elements</span></span>

|<span data-ttu-id="aaa21-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="aaa21-111">**Element**</span></span>|<span data-ttu-id="aaa21-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="aaa21-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aaa21-113">Nome (SOAP)</span><span class="sxs-lookup"><span data-stu-id="aaa21-113">Name (SOAP)</span></span>](name-soap.md) <br/> |<span data-ttu-id="aaa21-114">Representa um nome de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="aaa21-114">Represents a user setting name.</span></span>  <br/> |
|[<span data-ttu-id="aaa21-115">Valor (SOAP)</span><span class="sxs-lookup"><span data-stu-id="aaa21-115">Value (SOAP)</span></span>](value-soap.md) <br/> |<span data-ttu-id="aaa21-116">Representa um valor de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="aaa21-116">Represents a user setting value.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aaa21-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="aaa21-117">Parent elements</span></span>

<span data-ttu-id="aaa21-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="aaa21-118">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="aaa21-119">Text value</span><span class="sxs-lookup"><span data-stu-id="aaa21-119">Text value</span></span>

<span data-ttu-id="aaa21-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="aaa21-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="aaa21-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="aaa21-121">Remarks</span></span>

<span data-ttu-id="aaa21-122">O tipo de **StringSetting** estende o tipo de **UserSetting** .</span><span class="sxs-lookup"><span data-stu-id="aaa21-122">The **StringSetting** type extends the **UserSetting** type.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="aaa21-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="aaa21-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aaa21-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="aaa21-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="aaa21-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="aaa21-125">Schema Name</span></span>  <br/> |<span data-ttu-id="aaa21-126">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="aaa21-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="aaa21-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="aaa21-127">Validation File</span></span>  <br/> |<span data-ttu-id="aaa21-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="aaa21-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="aaa21-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="aaa21-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="aaa21-130">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="aaa21-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aaa21-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="aaa21-131">See also</span></span>



[<span data-ttu-id="aaa21-132">Operação de GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="aaa21-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="aaa21-133">Operação de GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="aaa21-133">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="aaa21-134">Operação de GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="aaa21-134">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

