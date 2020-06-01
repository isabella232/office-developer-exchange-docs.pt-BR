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
description: O elemento Request contém as definições de configuração solicitadas e os usuários de destino.
ms.openlocfilehash: 4358713d19e763b75d2a43f147385026f43b1255
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44448986"
---
# <a name="request-soap"></a><span data-ttu-id="83d98-103">Solicitação (SOAP)</span><span class="sxs-lookup"><span data-stu-id="83d98-103">Request (SOAP)</span></span>

<span data-ttu-id="83d98-104">O elemento **Request** contém as definições de configuração solicitadas e os usuários de destino.</span><span class="sxs-lookup"><span data-stu-id="83d98-104">The **Request** element contains the requested configuration settings and the target users.</span></span> 
  
```XML
<Request>
   <Users/>
   <RequestedSettings/>
   <RequestedVersion/>
</Request>
```

 <span data-ttu-id="83d98-105">**GetUserSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="83d98-105">**GetUserSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="83d98-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="83d98-106">Attributes and elements</span></span>

<span data-ttu-id="83d98-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="83d98-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="83d98-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="83d98-108">Attributes</span></span>

<span data-ttu-id="83d98-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="83d98-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="83d98-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="83d98-110">Child elements</span></span>

|<span data-ttu-id="83d98-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="83d98-111">**Element**</span></span>|<span data-ttu-id="83d98-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="83d98-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="83d98-113">Usuários (SOAP)</span><span class="sxs-lookup"><span data-stu-id="83d98-113">Users (SOAP)</span></span>](users-soap.md) <br/> |<span data-ttu-id="83d98-114">Representa uma coleção de endereços de email dos usuários para os quais as configurações devem ser recuperadas.</span><span class="sxs-lookup"><span data-stu-id="83d98-114">Represents a collection of e-mail addresses of the users for whom settings should be retrieved.</span></span>  <br/> |
|[<span data-ttu-id="83d98-115">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="83d98-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="83d98-116">Contém os nomes das definições de configuração solicitadas.</span><span class="sxs-lookup"><span data-stu-id="83d98-116">Contains the names of the requested configuration settings.</span></span>  <br/> |
|[<span data-ttu-id="83d98-117">RequestedVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="83d98-117">RequestedVersion (SOAP)</span></span>](requestedversion-soap.md) <br/> |<span data-ttu-id="83d98-118">Especifica a versão de servidor específica que o provedor gostaria de usar.</span><span class="sxs-lookup"><span data-stu-id="83d98-118">Specifies the specific server version that the provider would like to use.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="83d98-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="83d98-119">Parent elements</span></span>

|<span data-ttu-id="83d98-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="83d98-120">**Element**</span></span>|<span data-ttu-id="83d98-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="83d98-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="83d98-122">GetUserSettingsRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="83d98-122">GetUserSettingsRequestMessage (SOAP)</span></span>](getusersettingsrequestmessage-soap.md) <br/> |<span data-ttu-id="83d98-123">Representa uma solicitação de [operação de GetUserSettings (SOAP)](getusersettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="83d98-123">Represents a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="83d98-124">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="83d98-124">Text value</span></span>

<span data-ttu-id="83d98-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="83d98-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="83d98-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="83d98-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="83d98-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="83d98-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="83d98-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="83d98-128">Schema Name</span></span>  <br/> |<span data-ttu-id="83d98-129">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="83d98-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="83d98-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="83d98-130">Validation File</span></span>  <br/> |<span data-ttu-id="83d98-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="83d98-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="83d98-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="83d98-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="83d98-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="83d98-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="83d98-134">Também consulte</span><span class="sxs-lookup"><span data-stu-id="83d98-134">See also</span></span>



[<span data-ttu-id="83d98-135">Operação GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="83d98-135">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

