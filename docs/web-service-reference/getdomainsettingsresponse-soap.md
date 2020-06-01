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
description: O elemento GetDomainSettingsResponse representa a resposta a uma operação GetDomainSettings (SOAP), que retorna as configurações de domínio.
ms.openlocfilehash: 94cb202948e6a0d5a34f5547132c052d1d1b6a40
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461874"
---
# <a name="getdomainsettingsresponse-soap"></a><span data-ttu-id="06fa7-103">GetDomainSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="06fa7-103">GetDomainSettingsResponse (SOAP)</span></span>

<span data-ttu-id="06fa7-104">O elemento **GetDomainSettingsResponse** representa a resposta a uma [operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md), que retorna as configurações de domínio.</span><span class="sxs-lookup"><span data-stu-id="06fa7-104">The **GetDomainSettingsResponse** element represents the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), which returns the domain settings.</span></span>
  
```XML
<GetDomainSettingsResponse>
   <DomainResponses/>
   <ErrorCode/>
   <ErrorMessage/>
</GetDomainSettingsResponse>
```

 <span data-ttu-id="06fa7-105">**GetDomainSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="06fa7-105">**GetDomainSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="06fa7-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="06fa7-106">Attributes and elements</span></span>

<span data-ttu-id="06fa7-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="06fa7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="06fa7-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="06fa7-108">Attributes</span></span>

<span data-ttu-id="06fa7-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="06fa7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="06fa7-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="06fa7-110">Child elements</span></span>

|<span data-ttu-id="06fa7-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="06fa7-111">**Element**</span></span>|<span data-ttu-id="06fa7-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="06fa7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="06fa7-113">DomainResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="06fa7-113">DomainResponses (SOAP)</span></span>](domainresponses-soap.md) <br/> |<span data-ttu-id="06fa7-114">Contém uma matriz de respostas para cada configuração de domínio solicitada.</span><span class="sxs-lookup"><span data-stu-id="06fa7-114">Contains an array of responses for each requested domain's settings.</span></span>  <br/> |
|[<span data-ttu-id="06fa7-115">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="06fa7-115">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="06fa7-116">Representa um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="06fa7-116">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="06fa7-117">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="06fa7-117">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="06fa7-118">Representa uma mensagem que é associada a um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="06fa7-118">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="06fa7-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="06fa7-119">Parent elements</span></span>

<span data-ttu-id="06fa7-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="06fa7-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="06fa7-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="06fa7-121">Text value</span></span>

<span data-ttu-id="06fa7-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="06fa7-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="06fa7-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="06fa7-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="06fa7-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="06fa7-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="06fa7-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="06fa7-125">Schema Name</span></span>  <br/> |<span data-ttu-id="06fa7-126">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="06fa7-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="06fa7-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="06fa7-127">Validation File</span></span>  <br/> |<span data-ttu-id="06fa7-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="06fa7-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="06fa7-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="06fa7-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="06fa7-130">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="06fa7-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="06fa7-131">Também consulte</span><span class="sxs-lookup"><span data-stu-id="06fa7-131">See also</span></span>



[<span data-ttu-id="06fa7-132">Operação GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="06fa7-132">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

