---
title: Resposta (GetFederationInformation) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ca48a4b3-5006-4bb7-973e-d9137ce67e16
description: O elemento Response contém as informações de resposta da operação GetFederationInformation (SOAP).
ms.openlocfilehash: 0b9a2c518b968faa6ef86b7c1f544eac40f8e5c8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530583"
---
# <a name="response-getfederationinformation-soap"></a><span data-ttu-id="beaf4-103">Resposta (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="beaf4-103">Response (GetFederationInformation) (SOAP)</span></span>

<span data-ttu-id="beaf4-104">O elemento **Response** contém as informações de resposta da [operação GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="beaf4-104">The **Response** element contains the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) response information.</span></span> 
  
```XML
<Response>
   <ErrorCode/>
   <ErrorMessage/>
   <ApplicationUri/>
   <Domains/>
</Response>
```

 <span data-ttu-id="beaf4-105">**GetFederationInformationResponse**</span><span class="sxs-lookup"><span data-stu-id="beaf4-105">**GetFederationInformationResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="beaf4-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="beaf4-106">Attributes and elements</span></span>

<span data-ttu-id="beaf4-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="beaf4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="beaf4-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="beaf4-108">Attributes</span></span>

<span data-ttu-id="beaf4-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="beaf4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="beaf4-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="beaf4-110">Child elements</span></span>

|<span data-ttu-id="beaf4-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="beaf4-111">**Element**</span></span>|<span data-ttu-id="beaf4-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="beaf4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="beaf4-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="beaf4-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="beaf4-114">Representa um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="beaf4-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="beaf4-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="beaf4-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="beaf4-116">Representa uma mensagem que é associada a um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="beaf4-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="beaf4-117">ApplicationUri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="beaf4-117">ApplicationUri (SOAP)</span></span>](applicationuri-soap.md) <br/> |<span data-ttu-id="beaf4-118">Define o local de um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="beaf4-118">Defines the location of an application.</span></span>  <br/> |
|[<span data-ttu-id="beaf4-119">Domínios (SOAP)</span><span class="sxs-lookup"><span data-stu-id="beaf4-119">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="beaf4-120">Representa a coleção Domain as configurações para as quais são retornadas em uma [operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)ou os domínios que a organização tenha federado em uma [operação do GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="beaf4-120">Represents the domain collection the configurations for which are returned in a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), or the domains that the organization has federated in a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="beaf4-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="beaf4-121">Parent elements</span></span>

|<span data-ttu-id="beaf4-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="beaf4-122">**Element**</span></span>|<span data-ttu-id="beaf4-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="beaf4-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="beaf4-124">GetFederationInformationResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="beaf4-124">GetFederationInformationResponseMessage (SOAP)</span></span>](getfederationinformationresponsemessage-soap.md) <br/> |<span data-ttu-id="beaf4-125">Define uma resposta a uma solicitação de [operação de GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="beaf4-125">Defines a response to a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="beaf4-126">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="beaf4-126">Text value</span></span>

<span data-ttu-id="beaf4-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="beaf4-127">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="beaf4-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="beaf4-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="beaf4-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="beaf4-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="beaf4-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="beaf4-130">Schema Name</span></span>  <br/> |<span data-ttu-id="beaf4-131">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="beaf4-131">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="beaf4-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="beaf4-132">Validation File</span></span>  <br/> |<span data-ttu-id="beaf4-133">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="beaf4-133">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="beaf4-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="beaf4-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="beaf4-135">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="beaf4-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="beaf4-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="beaf4-136">See also</span></span>



[<span data-ttu-id="beaf4-137">Operação GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="beaf4-137">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

