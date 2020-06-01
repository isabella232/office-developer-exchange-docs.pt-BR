---
title: GetDomainSettingsRequest (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5ac0ff6d-9e02-4e4c-973d-cd9e076661d5
description: O elemento GetDomainSettingsRequest representa uma solicitação de operação de operação de GetDomainSettings (SOAP).
ms.openlocfilehash: 400016d0817131fb70ec7ff3db7fbfdc1b51f8f9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460957"
---
# <a name="getdomainsettingsrequest-soap"></a><span data-ttu-id="0d707-103">GetDomainSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0d707-103">GetDomainSettingsRequest (SOAP)</span></span>

<span data-ttu-id="0d707-104">O elemento **GetDomainSettingsRequest** representa uma solicitação de operação de operação de [GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="0d707-104">The **GetDomainSettingsRequest** element represents a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) operation request.</span></span> 
  
```XML
<GetDomainSettingsRequest>
   <Domains/>
   <RequestedSettings/>
   <RequestedVersion/>
</GetDomainSettingsRequest>
```

 <span data-ttu-id="0d707-105">**GetDomainSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="0d707-105">**GetDomainSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0d707-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="0d707-106">Attributes and elements</span></span>

<span data-ttu-id="0d707-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0d707-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0d707-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0d707-108">Attributes</span></span>

<span data-ttu-id="0d707-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0d707-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0d707-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0d707-110">Child elements</span></span>

|<span data-ttu-id="0d707-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0d707-111">**Element**</span></span>|<span data-ttu-id="0d707-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0d707-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0d707-113">Domínios (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0d707-113">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="0d707-114">Representa uma coleção de identificadores de domínio.</span><span class="sxs-lookup"><span data-stu-id="0d707-114">Represents a collection of domain identifiers.</span></span>  <br/> |
|[<span data-ttu-id="0d707-115">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0d707-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="0d707-116">Contém os nomes das definições de configuração de domínio solicitadas.</span><span class="sxs-lookup"><span data-stu-id="0d707-116">Contains the names of the requested domain configuration settings.</span></span>  <br/> |
|[<span data-ttu-id="0d707-117">RequestedVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0d707-117">RequestedVersion (SOAP)</span></span>](requestedversion-soap.md) <br/> |<span data-ttu-id="0d707-118">Especifica a versão do servidor que o provedor usará.</span><span class="sxs-lookup"><span data-stu-id="0d707-118">Specifies the server version that the provider will use.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0d707-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0d707-119">Parent elements</span></span>

<span data-ttu-id="0d707-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0d707-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="0d707-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="0d707-121">Text value</span></span>

<span data-ttu-id="0d707-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0d707-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0d707-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="0d707-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0d707-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="0d707-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="0d707-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0d707-125">Schema Name</span></span>  <br/> |<span data-ttu-id="0d707-126">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="0d707-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="0d707-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0d707-127">Validation File</span></span>  <br/> |<span data-ttu-id="0d707-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0d707-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0d707-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0d707-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="0d707-130">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="0d707-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0d707-131">Também consulte</span><span class="sxs-lookup"><span data-stu-id="0d707-131">See also</span></span>



[<span data-ttu-id="0d707-132">Operação GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0d707-132">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

