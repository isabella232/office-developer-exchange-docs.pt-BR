---
title: GetDomainSettingsResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 43ebd17b-3a70-4878-9254-97a4c2c87b77
description: O elemento GetDomainSettingsResponse representa a resposta a uma operação de GetDomainSettings (SOAP), que retorna as configurações de domínio.
ms.openlocfilehash: c4984c2c6c532fcbd45c1a75733e578f6d9491fa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752468"
---
# <a name="getdomainsettingsresponse-soap"></a><span data-ttu-id="c6066-103">GetDomainSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c6066-103">GetDomainSettingsResponse (SOAP)</span></span>

<span data-ttu-id="c6066-104">O elemento **GetDomainSettingsResponse** representa a resposta a uma [operação de GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md), que retorna as configurações de domínio.</span><span class="sxs-lookup"><span data-stu-id="c6066-104">The **GetDomainSettingsResponse** element represents the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), which returns the domain settings.</span></span>
  
```XML
<GetDomainSettingsResponse>
   <DomainResponses/>
   <ErrorCode/>
   <ErrorMessage/>
</GetDomainSettingsResponse>
```

 <span data-ttu-id="c6066-105">**GetDomainSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="c6066-105">**GetDomainSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c6066-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c6066-106">Attributes and elements</span></span>

<span data-ttu-id="c6066-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c6066-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c6066-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c6066-108">Attributes</span></span>

<span data-ttu-id="c6066-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c6066-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c6066-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c6066-110">Child elements</span></span>

|<span data-ttu-id="c6066-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c6066-111">**Element**</span></span>|<span data-ttu-id="c6066-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c6066-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c6066-113">DomainResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c6066-113">DomainResponses (SOAP)</span></span>](domainresponses-soap.md) <br/> |<span data-ttu-id="c6066-114">Contém uma matriz de respostas para as configurações do cada domínio solicitada.</span><span class="sxs-lookup"><span data-stu-id="c6066-114">Contains an array of responses for each requested domain's settings.</span></span>  <br/> |
|[<span data-ttu-id="c6066-115">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c6066-115">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="c6066-116">Representa um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="c6066-116">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="c6066-117">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c6066-117">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="c6066-118">Representa uma mensagem que está associada um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="c6066-118">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c6066-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c6066-119">Parent elements</span></span>

<span data-ttu-id="c6066-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c6066-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="c6066-121">Text value</span><span class="sxs-lookup"><span data-stu-id="c6066-121">Text value</span></span>

<span data-ttu-id="c6066-122">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c6066-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c6066-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c6066-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c6066-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="c6066-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="c6066-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c6066-125">Schema Name</span></span>  <br/> |<span data-ttu-id="c6066-126">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="c6066-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="c6066-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c6066-127">Validation File</span></span>  <br/> |<span data-ttu-id="c6066-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c6066-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c6066-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c6066-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="c6066-130">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="c6066-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c6066-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="c6066-131">See also</span></span>



[<span data-ttu-id="c6066-132">Operação de GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c6066-132">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

