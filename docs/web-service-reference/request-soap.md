---
title: Solicitação (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 75696436-997e-49f1-a31b-eb9a8c3526f3
description: O elemento de solicitação contém as definições de configuração solicitado e os usuários de destino.
ms.openlocfilehash: dfea33786066dd7803d0fd061cbb87bb06d11531
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825125"
---
# <a name="request-soap"></a><span data-ttu-id="c2cf6-103">Solicitação (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c2cf6-103">Request (SOAP)</span></span>

<span data-ttu-id="c2cf6-104">O elemento de **solicitação** contém as definições de configuração solicitado e os usuários de destino.</span><span class="sxs-lookup"><span data-stu-id="c2cf6-104">The **Request** element contains the requested configuration settings and the target users.</span></span> 
  
```XML
<Request>
   <Users/>
   <RequestedSettings/>
   <RequestedVersion/>
</Request>
```

 <span data-ttu-id="c2cf6-105">**GetUserSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="c2cf6-105">**GetUserSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c2cf6-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c2cf6-106">Attributes and elements</span></span>

<span data-ttu-id="c2cf6-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c2cf6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c2cf6-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c2cf6-108">Attributes</span></span>

<span data-ttu-id="c2cf6-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c2cf6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c2cf6-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c2cf6-110">Child elements</span></span>

|<span data-ttu-id="c2cf6-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c2cf6-111">**Element**</span></span>|<span data-ttu-id="c2cf6-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c2cf6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2cf6-113">Usuários (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c2cf6-113">Users (SOAP)</span></span>](users-soap.md) <br/> |<span data-ttu-id="c2cf6-114">Representa uma coleção de endereços de email dos usuários cujas configurações devem ser recuperadas.</span><span class="sxs-lookup"><span data-stu-id="c2cf6-114">Represents a collection of e-mail addresses of the users for whom settings should be retrieved.</span></span>  <br/> |
|[<span data-ttu-id="c2cf6-115">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c2cf6-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="c2cf6-116">Contém os nomes das definições de configuração solicitada.</span><span class="sxs-lookup"><span data-stu-id="c2cf6-116">Contains the names of the requested configuration settings.</span></span>  <br/> |
|[<span data-ttu-id="c2cf6-117">RequestedVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c2cf6-117">RequestedVersion (SOAP)</span></span>](requestedversion-soap.md) <br/> |<span data-ttu-id="c2cf6-118">Especifica a versão de servidor específico que o provedor gostaria de usar.</span><span class="sxs-lookup"><span data-stu-id="c2cf6-118">Specifies the specific server version that the provider would like to use.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c2cf6-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c2cf6-119">Parent elements</span></span>

|<span data-ttu-id="c2cf6-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c2cf6-120">**Element**</span></span>|<span data-ttu-id="c2cf6-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c2cf6-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2cf6-122">GetUserSettingsRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c2cf6-122">GetUserSettingsRequestMessage (SOAP)</span></span>](getusersettingsrequestmessage-soap.md) <br/> |<span data-ttu-id="c2cf6-123">Representa uma solicitação de [operação GetUserSettings (SOAP)](getusersettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="c2cf6-123">Represents a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c2cf6-124">Text value</span><span class="sxs-lookup"><span data-stu-id="c2cf6-124">Text value</span></span>

<span data-ttu-id="c2cf6-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c2cf6-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c2cf6-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c2cf6-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c2cf6-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="c2cf6-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="c2cf6-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c2cf6-128">Schema Name</span></span>  <br/> |<span data-ttu-id="c2cf6-129">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="c2cf6-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="c2cf6-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c2cf6-130">Validation File</span></span>  <br/> |<span data-ttu-id="c2cf6-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c2cf6-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c2cf6-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c2cf6-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="c2cf6-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="c2cf6-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c2cf6-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="c2cf6-134">See also</span></span>



[<span data-ttu-id="c2cf6-135">Operação de GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c2cf6-135">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

