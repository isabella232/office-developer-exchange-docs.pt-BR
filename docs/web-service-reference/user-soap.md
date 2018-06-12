---
title: Usuário (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: c6bc0031-bc1d-41bd-84e4-9074a5b77012
description: O elemento de usuário representa a identidade de um único usuário.
ms.openlocfilehash: a8dcb22f5c74a9622f978f34e48146115351fe82
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837971"
---
# <a name="user-soap"></a><span data-ttu-id="0c473-103">Usuário (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0c473-103">User (SOAP)</span></span>

<span data-ttu-id="0c473-104">O elemento de **usuário** representa a identidade de um único usuário.</span><span class="sxs-lookup"><span data-stu-id="0c473-104">The **User** element represents the identity of a single user.</span></span> 
  
```XML
<User>
    <LegacyDN/>
    <Mailbox/>
    <RequestedSettings/>
</User>
```

 <span data-ttu-id="0c473-105">**User**</span><span class="sxs-lookup"><span data-stu-id="0c473-105">**User**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0c473-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="0c473-106">Attributes and elements</span></span>

<span data-ttu-id="0c473-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0c473-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0c473-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0c473-108">Attributes</span></span>

<span data-ttu-id="0c473-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0c473-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0c473-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0c473-110">Child elements</span></span>

|<span data-ttu-id="0c473-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0c473-111">**Element**</span></span>|<span data-ttu-id="0c473-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0c473-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0c473-113">LegacyDN (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0c473-113">LegacyDN (SOAP)</span></span>](legacydn-soap.md) <br/> |<span data-ttu-id="0c473-114">Representa o nome distinto herdado de caixa de correio alternativo.</span><span class="sxs-lookup"><span data-stu-id="0c473-114">Represents the alternate mailbox legacy distinguished name.</span></span>  <br/> |
|[<span data-ttu-id="0c473-115">Caixa de correio (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0c473-115">Mailbox (SOAP)</span></span>](mailbox-soap.md) <br/> |<span data-ttu-id="0c473-116">Contém o endereço de email do usuário a ser descoberto.</span><span class="sxs-lookup"><span data-stu-id="0c473-116">Contains the e-mail address of the user to be discovered.</span></span>  <br/> |
|[<span data-ttu-id="0c473-117">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0c473-117">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="0c473-118">Contém os nomes das definições de configuração solicitada.</span><span class="sxs-lookup"><span data-stu-id="0c473-118">Contains the names of the requested configuration settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0c473-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0c473-119">Parent elements</span></span>

|<span data-ttu-id="0c473-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0c473-120">**Element**</span></span>|<span data-ttu-id="0c473-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0c473-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0c473-122">Usuários (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0c473-122">Users (SOAP)</span></span>](users-soap.md) <br/> |<span data-ttu-id="0c473-123">Representa uma coleção de elementos do **usuário** .</span><span class="sxs-lookup"><span data-stu-id="0c473-123">Represents a collection of **User** elements.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0c473-124">Text value</span><span class="sxs-lookup"><span data-stu-id="0c473-124">Text value</span></span>

<span data-ttu-id="0c473-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0c473-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0c473-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="0c473-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0c473-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="0c473-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="0c473-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0c473-128">Schema Name</span></span>  <br/> |<span data-ttu-id="0c473-129">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="0c473-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="0c473-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0c473-130">Validation File</span></span>  <br/> |<span data-ttu-id="0c473-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0c473-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0c473-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0c473-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="0c473-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="0c473-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0c473-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="0c473-134">See also</span></span>



[<span data-ttu-id="0c473-135">Operação de GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0c473-135">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="0c473-136">Operação de GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0c473-136">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="0c473-137">Operação de GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0c473-137">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

