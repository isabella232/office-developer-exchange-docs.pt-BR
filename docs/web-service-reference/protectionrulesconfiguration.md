---
title: ProtectionRulesConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ProtectionRulesConfiguration
api_type:
- schema
ms.assetid: e5b4699a-476e-4053-bb52-873eb921c046
description: O elemento ProtectionRulesConfiguration contém informações de configuração de serviço para o serviço de regras de proteção.
ms.openlocfilehash: 9c286fcf9752d591d53323f45a264f4bdd078c1c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824912"
---
# <a name="protectionrulesconfiguration"></a><span data-ttu-id="70ab9-103">ProtectionRulesConfiguration</span><span class="sxs-lookup"><span data-stu-id="70ab9-103">ProtectionRulesConfiguration</span></span>

<span data-ttu-id="70ab9-104">O elemento **ProtectionRulesConfiguration** contém informações de configuração de serviço para o serviço de regras de proteção.</span><span class="sxs-lookup"><span data-stu-id="70ab9-104">The **ProtectionRulesConfiguration** element contains service configuration information for the protection rules service.</span></span> 
  
```XML
<ProtectionRulesConfiguration RefreshInterval="">
   <Rules/>
   <InternalDomains/>
</ProtectionRulesConfiguration>
```

 <span data-ttu-id="70ab9-105">**ProtectionRulesServiceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="70ab9-105">**ProtectionRulesServiceConfiguration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="70ab9-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="70ab9-106">Attributes and elements</span></span>

<span data-ttu-id="70ab9-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="70ab9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="70ab9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="70ab9-108">Attributes</span></span>

|<span data-ttu-id="70ab9-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="70ab9-109">**Attribute**</span></span>|<span data-ttu-id="70ab9-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="70ab9-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="70ab9-111">**RefreshInterval**</span><span class="sxs-lookup"><span data-stu-id="70ab9-111">**RefreshInterval**</span></span> <br/> |<span data-ttu-id="70ab9-112">Especifica a frequência, em horas inteiras, o cliente deve solicitar as regras de proteção do servidor.</span><span class="sxs-lookup"><span data-stu-id="70ab9-112">Specifies how often, in whole hours, the client should request protection rules from the server.</span></span> <span data-ttu-id="70ab9-113">Este atributo é necessário e seu valor deve ser um inteiro que é igual ou maior que 1.</span><span class="sxs-lookup"><span data-stu-id="70ab9-113">This attribute is required and its value must be an integer that is equal to or greater than 1.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="70ab9-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="70ab9-114">Child elements</span></span>

|<span data-ttu-id="70ab9-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="70ab9-115">**Element**</span></span>|<span data-ttu-id="70ab9-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="70ab9-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="70ab9-117">Regras</span><span class="sxs-lookup"><span data-stu-id="70ab9-117">Rules </span></span>](rules-ex15websvcsotherref.md) <br/> |<span data-ttu-id="70ab9-118">Uma matriz de regras de proteção.</span><span class="sxs-lookup"><span data-stu-id="70ab9-118">An array of protection rules.</span></span> <span data-ttu-id="70ab9-119">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70ab9-119">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="70ab9-120">InternalDomains (SmtpDomainList)</span><span class="sxs-lookup"><span data-stu-id="70ab9-120">InternalDomains (SmtpDomainList)</span></span>](internaldomains-smtpdomainlist.md) <br/> |<span data-ttu-id="70ab9-121">Identifica a lista de domínios de SMTP internos da organização.</span><span class="sxs-lookup"><span data-stu-id="70ab9-121">Identifies the list of internal SMTP domains of the organization.</span></span> <span data-ttu-id="70ab9-122">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="70ab9-122">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="70ab9-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="70ab9-123">Parent elements</span></span>

|<span data-ttu-id="70ab9-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="70ab9-124">**Element**</span></span>|<span data-ttu-id="70ab9-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="70ab9-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="70ab9-126">ServiceConfigurationResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="70ab9-126">ServiceConfigurationResponseMessageType</span></span>](serviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="70ab9-127">Contém as definições de configuração de serviço.</span><span class="sxs-lookup"><span data-stu-id="70ab9-127">Contains service configuration settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="70ab9-128">Text value</span><span class="sxs-lookup"><span data-stu-id="70ab9-128">Text value</span></span>

<span data-ttu-id="70ab9-129">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="70ab9-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="70ab9-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="70ab9-130">Remarks</span></span>

<span data-ttu-id="70ab9-131">A configuração de serviço de regras de proteção é composta por uma lista de regras, domínios internos e um intervalo de atualização.</span><span class="sxs-lookup"><span data-stu-id="70ab9-131">The protection rules service configuration is comprised of a list of rules, internal domains, and a refresh interval.</span></span>
  
<span data-ttu-id="70ab9-132">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="70ab9-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="70ab9-133">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="70ab9-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="70ab9-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="70ab9-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="70ab9-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="70ab9-135">Schema Name</span></span>  <br/> |<span data-ttu-id="70ab9-136">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="70ab9-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="70ab9-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="70ab9-137">Validation File</span></span>  <br/> |<span data-ttu-id="70ab9-138">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="70ab9-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="70ab9-139">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="70ab9-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="70ab9-140">False</span><span class="sxs-lookup"><span data-stu-id="70ab9-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="70ab9-141">Ver também</span><span class="sxs-lookup"><span data-stu-id="70ab9-141">See also</span></span>



- [<span data-ttu-id="70ab9-142">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="70ab9-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

