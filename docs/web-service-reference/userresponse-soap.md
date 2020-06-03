---
title: Userresponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd
description: O elemento userresponse representa uma resposta a uma solicitação GetUserSettings para um usuário individual.
ms.openlocfilehash: 73848cb19d9c859e07216f354965ac4051d0d20c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468898"
---
# <a name="userresponse-soap"></a><span data-ttu-id="011ff-103">Userresponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="011ff-103">UserResponse (SOAP)</span></span>

<span data-ttu-id="011ff-104">O elemento **userresponse** representa uma resposta a uma solicitação GetUserSettings para um usuário individual.</span><span class="sxs-lookup"><span data-stu-id="011ff-104">The **UserResponse** element represents a response to a GetUserSettings request for an individual user.</span></span> 
  
```XML
<UserResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <RedirectTarget/>
   <UserSettingErrors/>
   <UserSettings/>
</UserResponse>
```

 <span data-ttu-id="011ff-105">**Userresponse**</span><span class="sxs-lookup"><span data-stu-id="011ff-105">**UserResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="011ff-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="011ff-106">Attributes and elements</span></span>

<span data-ttu-id="011ff-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="011ff-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="011ff-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="011ff-108">Attributes</span></span>

<span data-ttu-id="011ff-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="011ff-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="011ff-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="011ff-110">Child elements</span></span>

|<span data-ttu-id="011ff-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="011ff-111">**Element**</span></span>|<span data-ttu-id="011ff-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="011ff-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="011ff-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="011ff-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="011ff-114">Representa um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="011ff-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="011ff-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="011ff-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="011ff-116">Representa uma mensagem que é associada a um código de erro retornado pelo serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="011ff-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="011ff-117">RedirectTarget (SOAP)</span><span class="sxs-lookup"><span data-stu-id="011ff-117">RedirectTarget (SOAP)</span></span>](redirecttarget-soap.md) <br/> |<span data-ttu-id="011ff-118">Contém o destino da URL de redirecionamento ou endereço de email.</span><span class="sxs-lookup"><span data-stu-id="011ff-118">Contains the target of the redirection URL or email address.</span></span>  <br/> |
|[<span data-ttu-id="011ff-119">UserSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="011ff-119">UserSettingErrors (SOAP)</span></span>](usersettingerrors-soap.md) <br/> |<span data-ttu-id="011ff-120">Representa uma coleção de informações sobre as configurações que não puderam ser retornadas.</span><span class="sxs-lookup"><span data-stu-id="011ff-120">Represents a collection of information about settings that could not be returned.</span></span>  <br/> |
|[<span data-ttu-id="011ff-121">UserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="011ff-121">UserSettings (SOAP)</span></span>](usersettings-soap.md) <br/> |<span data-ttu-id="011ff-122">As configurações solicitadas para o usuário.</span><span class="sxs-lookup"><span data-stu-id="011ff-122">The requested settings for the user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="011ff-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="011ff-123">Parent elements</span></span>

|<span data-ttu-id="011ff-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="011ff-124">**Element**</span></span>|<span data-ttu-id="011ff-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="011ff-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="011ff-126">ArrayOfUserResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="011ff-126">ArrayOfUserResponse (SOAP)</span></span>](arrayofuserresponse-soap.md) <br/> |<span data-ttu-id="011ff-127">Contém uma matriz de respostas do usuário.</span><span class="sxs-lookup"><span data-stu-id="011ff-127">Contains an array of user responses.</span></span>  <br/> |
|[<span data-ttu-id="011ff-128">Userresponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="011ff-128">UserResponses (SOAP)</span></span>](userresponses-soap.md) <br/> |<span data-ttu-id="011ff-129">Contém as definições de configuração para cada usuário solicitado.</span><span class="sxs-lookup"><span data-stu-id="011ff-129">Contains the configuration settings for each requested user.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="011ff-130">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="011ff-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="011ff-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="011ff-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="011ff-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="011ff-132">Schema Name</span></span>  <br/> |<span data-ttu-id="011ff-133">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="011ff-133">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="011ff-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="011ff-134">Validation File</span></span>  <br/> |<span data-ttu-id="011ff-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="011ff-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="011ff-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="011ff-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="011ff-137">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="011ff-137">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="011ff-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="011ff-138">See also</span></span>



[<span data-ttu-id="011ff-139">Elementos XML de descoberta automática SOAP para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="011ff-139">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

