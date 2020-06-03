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
ms.openlocfilehash: e664fba78f170c9f4c59b49b3a08c0dd2e4ed4cd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456719"
---
# <a name="protectionrulesconfiguration"></a><span data-ttu-id="a2edf-103">ProtectionRulesConfiguration</span><span class="sxs-lookup"><span data-stu-id="a2edf-103">ProtectionRulesConfiguration</span></span>

<span data-ttu-id="a2edf-104">O elemento **ProtectionRulesConfiguration** contém informações de configuração de serviço para o serviço de regras de proteção.</span><span class="sxs-lookup"><span data-stu-id="a2edf-104">The **ProtectionRulesConfiguration** element contains service configuration information for the protection rules service.</span></span> 
  
```XML
<ProtectionRulesConfiguration RefreshInterval="">
   <Rules/>
   <InternalDomains/>
</ProtectionRulesConfiguration>
```

 <span data-ttu-id="a2edf-105">**ProtectionRulesServiceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="a2edf-105">**ProtectionRulesServiceConfiguration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a2edf-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a2edf-106">Attributes and elements</span></span>

<span data-ttu-id="a2edf-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a2edf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a2edf-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a2edf-108">Attributes</span></span>

|<span data-ttu-id="a2edf-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="a2edf-109">**Attribute**</span></span>|<span data-ttu-id="a2edf-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a2edf-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a2edf-111">**RefreshInterval**</span><span class="sxs-lookup"><span data-stu-id="a2edf-111">**RefreshInterval**</span></span> <br/> |<span data-ttu-id="a2edf-112">Especifica com que frequência, em horas inteiras, o cliente deve solicitar regras de proteção do servidor.</span><span class="sxs-lookup"><span data-stu-id="a2edf-112">Specifies how often, in whole hours, the client should request protection rules from the server.</span></span> <span data-ttu-id="a2edf-113">Este atributo é obrigatório e seu valor deve ser um inteiro igual ou maior que 1.</span><span class="sxs-lookup"><span data-stu-id="a2edf-113">This attribute is required and its value must be an integer that is equal to or greater than 1.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a2edf-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a2edf-114">Child elements</span></span>

|<span data-ttu-id="a2edf-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a2edf-115">**Element**</span></span>|<span data-ttu-id="a2edf-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a2edf-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2edf-117">Regras</span><span class="sxs-lookup"><span data-stu-id="a2edf-117">Rules </span></span>](rules-ex15websvcsotherref.md) <br/> |<span data-ttu-id="a2edf-118">Uma matriz de regras de proteção.</span><span class="sxs-lookup"><span data-stu-id="a2edf-118">An array of protection rules.</span></span> <span data-ttu-id="a2edf-119">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2edf-119">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="a2edf-120">InternalDomains (SmtpDomainList)</span><span class="sxs-lookup"><span data-stu-id="a2edf-120">InternalDomains (SmtpDomainList)</span></span>](internaldomains-smtpdomainlist.md) <br/> |<span data-ttu-id="a2edf-121">Identifica a lista de domínios SMTP internos da organização.</span><span class="sxs-lookup"><span data-stu-id="a2edf-121">Identifies the list of internal SMTP domains of the organization.</span></span> <span data-ttu-id="a2edf-122">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2edf-122">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a2edf-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a2edf-123">Parent elements</span></span>

|<span data-ttu-id="a2edf-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a2edf-124">**Element**</span></span>|<span data-ttu-id="a2edf-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a2edf-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2edf-126">ServiceConfigurationResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="a2edf-126">ServiceConfigurationResponseMessageType</span></span>](serviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="a2edf-127">Contém definições de configuração de serviço.</span><span class="sxs-lookup"><span data-stu-id="a2edf-127">Contains service configuration settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a2edf-128">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="a2edf-128">Text value</span></span>

<span data-ttu-id="a2edf-129">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a2edf-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a2edf-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="a2edf-130">Remarks</span></span>

<span data-ttu-id="a2edf-131">A configuração do serviço de regras de proteção é composta por uma lista de regras, domínios internos e um intervalo de atualização.</span><span class="sxs-lookup"><span data-stu-id="a2edf-131">The protection rules service configuration is comprised of a list of rules, internal domains, and a refresh interval.</span></span>
  
<span data-ttu-id="a2edf-132">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a2edf-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a2edf-133">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="a2edf-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a2edf-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="a2edf-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a2edf-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a2edf-135">Schema Name</span></span>  <br/> |<span data-ttu-id="a2edf-136">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="a2edf-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a2edf-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a2edf-137">Validation File</span></span>  <br/> |<span data-ttu-id="a2edf-138">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a2edf-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a2edf-139">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a2edf-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="a2edf-140">False</span><span class="sxs-lookup"><span data-stu-id="a2edf-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a2edf-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="a2edf-141">See also</span></span>



- [<span data-ttu-id="a2edf-142">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a2edf-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

