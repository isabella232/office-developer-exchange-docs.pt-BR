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
description: O elemento user representa a identidade de um único usuário.
ms.openlocfilehash: f151ffa8050a10cdbb4562471d815f8692596cc3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456343"
---
# <a name="user-soap"></a><span data-ttu-id="70d5a-103">Usuário (SOAP)</span><span class="sxs-lookup"><span data-stu-id="70d5a-103">User (SOAP)</span></span>

<span data-ttu-id="70d5a-104">O elemento **User** representa a identidade de um único usuário.</span><span class="sxs-lookup"><span data-stu-id="70d5a-104">The **User** element represents the identity of a single user.</span></span> 
  
```XML
<User>
    <LegacyDN/>
    <Mailbox/>
    <RequestedSettings/>
</User>
```

 <span data-ttu-id="70d5a-105">**Usuário**</span><span class="sxs-lookup"><span data-stu-id="70d5a-105">**User**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="70d5a-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="70d5a-106">Attributes and elements</span></span>

<span data-ttu-id="70d5a-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="70d5a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="70d5a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="70d5a-108">Attributes</span></span>

<span data-ttu-id="70d5a-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="70d5a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="70d5a-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="70d5a-110">Child elements</span></span>

|<span data-ttu-id="70d5a-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="70d5a-111">**Element**</span></span>|<span data-ttu-id="70d5a-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="70d5a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="70d5a-113">LegacyDN (SOAP)</span><span class="sxs-lookup"><span data-stu-id="70d5a-113">LegacyDN (SOAP)</span></span>](legacydn-soap.md) <br/> |<span data-ttu-id="70d5a-114">Representa o nome diferenciado herdado da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="70d5a-114">Represents the alternate mailbox legacy distinguished name.</span></span>  <br/> |
|[<span data-ttu-id="70d5a-115">Caixa de correio (SOAP)</span><span class="sxs-lookup"><span data-stu-id="70d5a-115">Mailbox (SOAP)</span></span>](mailbox-soap.md) <br/> |<span data-ttu-id="70d5a-116">Contém o endereço de email do usuário a ser descoberto.</span><span class="sxs-lookup"><span data-stu-id="70d5a-116">Contains the e-mail address of the user to be discovered.</span></span>  <br/> |
|[<span data-ttu-id="70d5a-117">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="70d5a-117">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="70d5a-118">Contém os nomes das definições de configuração solicitadas.</span><span class="sxs-lookup"><span data-stu-id="70d5a-118">Contains the names of the requested configuration settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="70d5a-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="70d5a-119">Parent elements</span></span>

|<span data-ttu-id="70d5a-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="70d5a-120">**Element**</span></span>|<span data-ttu-id="70d5a-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="70d5a-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="70d5a-122">Usuários (SOAP)</span><span class="sxs-lookup"><span data-stu-id="70d5a-122">Users (SOAP)</span></span>](users-soap.md) <br/> |<span data-ttu-id="70d5a-123">Representa uma coleção de elementos do **usuário** .</span><span class="sxs-lookup"><span data-stu-id="70d5a-123">Represents a collection of **User** elements.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="70d5a-124">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="70d5a-124">Text value</span></span>

<span data-ttu-id="70d5a-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="70d5a-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="70d5a-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="70d5a-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="70d5a-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="70d5a-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="70d5a-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="70d5a-128">Schema Name</span></span>  <br/> |<span data-ttu-id="70d5a-129">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="70d5a-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="70d5a-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="70d5a-130">Validation File</span></span>  <br/> |<span data-ttu-id="70d5a-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="70d5a-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="70d5a-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="70d5a-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="70d5a-133">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="70d5a-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="70d5a-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="70d5a-134">See also</span></span>



[<span data-ttu-id="70d5a-135">Operação GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="70d5a-135">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="70d5a-136">Operação GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="70d5a-136">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="70d5a-137">Operação GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="70d5a-137">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

