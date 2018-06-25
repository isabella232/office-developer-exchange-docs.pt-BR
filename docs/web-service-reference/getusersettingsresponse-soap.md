---
title: GetUserSettingsResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: e7cd470d-5861-41e7-9e66-73ef7a59700b
description: O elemento GetUserSettingsResponse representa uma resposta a uma solicitação de operação (SOAP) GetUserSettings.
ms.openlocfilehash: 24dbfb1582f628fd0130aa82ea5f1beedd31b156
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823705"
---
# <a name="getusersettingsresponse-soap"></a><span data-ttu-id="4662f-103">GetUserSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4662f-103">GetUserSettingsResponse (SOAP)</span></span>

<span data-ttu-id="4662f-104">O elemento **GetUserSettingsResponse** representa uma resposta a uma solicitação de [operação GetUserSettings (SOAP)](getusersettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="4662f-104">The **GetUserSettingsResponse** element represents a response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request.</span></span> 
  
```XML
<GetUserSettingsResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <UserResponses/>
</GetUserSettingsResponse>
```

 <span data-ttu-id="4662f-105">**GetUserSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="4662f-105">**GetUserSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4662f-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="4662f-106">Attributes and elements</span></span>

<span data-ttu-id="4662f-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4662f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4662f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4662f-108">Attributes</span></span>

<span data-ttu-id="4662f-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4662f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4662f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4662f-110">Child elements</span></span>

|<span data-ttu-id="4662f-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4662f-111">**Element**</span></span>|<span data-ttu-id="4662f-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4662f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4662f-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4662f-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="4662f-114">Representa um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="4662f-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="4662f-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4662f-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="4662f-116">Representa uma mensagem que está associada um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="4662f-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="4662f-117">UserResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4662f-117">UserResponses (SOAP)</span></span>](userresponses-soap.md) <br/> |<span data-ttu-id="4662f-118">Contém as definições de configuração para cada usuário solicitado.</span><span class="sxs-lookup"><span data-stu-id="4662f-118">Contains the configuration settings for each requested user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4662f-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4662f-119">Parent elements</span></span>

<span data-ttu-id="4662f-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4662f-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="4662f-121">Text value</span><span class="sxs-lookup"><span data-stu-id="4662f-121">Text value</span></span>

<span data-ttu-id="4662f-122">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4662f-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4662f-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="4662f-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4662f-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="4662f-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="4662f-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4662f-125">Schema Name</span></span>  <br/> |<span data-ttu-id="4662f-126">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="4662f-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="4662f-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4662f-127">Validation File</span></span>  <br/> |<span data-ttu-id="4662f-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4662f-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4662f-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="4662f-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="4662f-130">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="4662f-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4662f-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="4662f-131">See also</span></span>



[<span data-ttu-id="4662f-132">Operação de GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4662f-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

