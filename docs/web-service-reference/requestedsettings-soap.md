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
description: O elemento RequestedSettings contém os nomes das definições de configuração solicitadas.
ms.openlocfilehash: e94c02d8f92d7aaac619c58f093c536cc1a098bf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465293"
---
# <a name="requestedsettings-soap"></a><span data-ttu-id="d6d35-103">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d6d35-103">RequestedSettings (SOAP)</span></span>

<span data-ttu-id="d6d35-104">O elemento **RequestedSettings** contém os nomes das definições de configuração solicitadas.</span><span class="sxs-lookup"><span data-stu-id="d6d35-104">The **RequestedSettings** element contains the names of the requested configuration settings.</span></span> 
  
```XML
<RequestedSettings>
   <Setting/>
</RequestedSettings>
```

 <span data-ttu-id="d6d35-105">**RequestedSettings**</span><span class="sxs-lookup"><span data-stu-id="d6d35-105">**RequestedSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d6d35-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d6d35-106">Attributes and elements</span></span>

<span data-ttu-id="d6d35-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d6d35-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d6d35-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d6d35-108">Attributes</span></span>

<span data-ttu-id="d6d35-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d6d35-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d6d35-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d6d35-110">Child elements</span></span>

|<span data-ttu-id="d6d35-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d6d35-111">**Element**</span></span>|<span data-ttu-id="d6d35-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d6d35-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d6d35-113">Configuração (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d6d35-113">Setting (SOAP)</span></span>](setting-soap.md) <br/> |<span data-ttu-id="d6d35-114">Representa uma configuração a ser retornada.</span><span class="sxs-lookup"><span data-stu-id="d6d35-114">Represents a configuration setting to be returned.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d6d35-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d6d35-115">Parent elements</span></span>

|<span data-ttu-id="d6d35-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d6d35-116">**Element**</span></span>|<span data-ttu-id="d6d35-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d6d35-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d6d35-118">GetUserSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d6d35-118">GetUserSettingsRequest (SOAP)</span></span>](getusersettingsrequest-soap.md) <br/> |<span data-ttu-id="d6d35-119">Representa uma solicitação para recuperar as configurações especificadas de um ou mais usuários.</span><span class="sxs-lookup"><span data-stu-id="d6d35-119">Represents a request to retrieve specified settings for one or more users.</span></span>  <br/> |
|[<span data-ttu-id="d6d35-120">Solicitação (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d6d35-120">Request (SOAP)</span></span>](request-soap.md) <br/> |<span data-ttu-id="d6d35-121">Contém as definições de configuração solicitadas e os usuários de destino.</span><span class="sxs-lookup"><span data-stu-id="d6d35-121">Contains the requested configuration settings and the target users.</span></span>  <br/> |
|[<span data-ttu-id="d6d35-122">GetDomainSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d6d35-122">GetDomainSettingsRequest (SOAP)</span></span>](getdomainsettingsrequest-soap.md) <br/> |<span data-ttu-id="d6d35-123">Representa uma solicitação de [operação de GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="d6d35-123">Represents a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="d6d35-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d6d35-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d6d35-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="d6d35-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="d6d35-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d6d35-126">Schema Name</span></span>  <br/> |<span data-ttu-id="d6d35-127">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="d6d35-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="d6d35-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d6d35-128">Validation File</span></span>  <br/> |<span data-ttu-id="d6d35-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d6d35-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d6d35-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d6d35-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="d6d35-131">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="d6d35-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d6d35-132">Também consulte</span><span class="sxs-lookup"><span data-stu-id="d6d35-132">See also</span></span>



[<span data-ttu-id="d6d35-133">Operação GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d6d35-133">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="d6d35-134">Operação GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d6d35-134">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

