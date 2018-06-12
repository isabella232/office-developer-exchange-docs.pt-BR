---
title: RequestedSettings (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 8d713d22-580c-49a5-99f5-ee532443e89a
description: O elemento RequestedSettings contém os nomes das definições de configuração solicitada.
ms.openlocfilehash: 025f86d417ea2041a3247ac67b065d75c8f75599
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825136"
---
# <a name="requestedsettings-soap"></a><span data-ttu-id="c9558-103">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c9558-103">RequestedSettings (SOAP)</span></span>

<span data-ttu-id="c9558-104">O elemento **RequestedSettings** contém os nomes das definições de configuração solicitada.</span><span class="sxs-lookup"><span data-stu-id="c9558-104">The **RequestedSettings** element contains the names of the requested configuration settings.</span></span> 
  
```XML
<RequestedSettings>
   <Setting/>
</RequestedSettings>
```

 <span data-ttu-id="c9558-105">**RequestedSettings**</span><span class="sxs-lookup"><span data-stu-id="c9558-105">**RequestedSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c9558-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c9558-106">Attributes and elements</span></span>

<span data-ttu-id="c9558-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c9558-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c9558-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c9558-108">Attributes</span></span>

<span data-ttu-id="c9558-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c9558-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c9558-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c9558-110">Child elements</span></span>

|<span data-ttu-id="c9558-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c9558-111">**Element**</span></span>|<span data-ttu-id="c9558-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c9558-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9558-113">Configuração (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c9558-113">Setting (SOAP)</span></span>](setting-soap.md) <br/> |<span data-ttu-id="c9558-114">Representa uma definição de configuração a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="c9558-114">Represents a configuration setting to be returned.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c9558-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c9558-115">Parent elements</span></span>

|<span data-ttu-id="c9558-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c9558-116">**Element**</span></span>|<span data-ttu-id="c9558-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c9558-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9558-118">GetUserSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c9558-118">GetUserSettingsRequest (SOAP)</span></span>](getusersettingsrequest-soap.md) <br/> |<span data-ttu-id="c9558-119">Representa uma solicitação para recuperar as configurações especificadas para um ou mais usuários.</span><span class="sxs-lookup"><span data-stu-id="c9558-119">Represents a request to retrieve specified settings for one or more users.</span></span>  <br/> |
|[<span data-ttu-id="c9558-120">Solicitação (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c9558-120">Request (SOAP)</span></span>](request-soap.md) <br/> |<span data-ttu-id="c9558-121">Contém as definições de configuração solicitado e os usuários de destino.</span><span class="sxs-lookup"><span data-stu-id="c9558-121">Contains the requested configuration settings and the target users.</span></span>  <br/> |
|[<span data-ttu-id="c9558-122">GetDomainSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c9558-122">GetDomainSettingsRequest (SOAP)</span></span>](getdomainsettingsrequest-soap.md) <br/> |<span data-ttu-id="c9558-123">Representa uma solicitação de [operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="c9558-123">Represents a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="c9558-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c9558-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c9558-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="c9558-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="c9558-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c9558-126">Schema Name</span></span>  <br/> |<span data-ttu-id="c9558-127">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="c9558-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="c9558-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c9558-128">Validation File</span></span>  <br/> |<span data-ttu-id="c9558-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c9558-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c9558-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c9558-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="c9558-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="c9558-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c9558-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="c9558-132">See also</span></span>



[<span data-ttu-id="c9558-133">Operação de GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c9558-133">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="c9558-134">Operação de GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c9558-134">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

