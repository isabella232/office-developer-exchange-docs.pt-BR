---
title: RequestedVersion (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 962036c9-9b13-4669-bed2-2502c0f5aabe
description: O elemento RequestedVersion Especifica a versão mínima do serviço que o cliente quer a solicitação a serem processados em.
ms.openlocfilehash: 0d8682c33790d2d26001512ad9e2191ae52074d0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825134"
---
# <a name="requestedversion-soap"></a><span data-ttu-id="cf2b0-103">RequestedVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cf2b0-103">RequestedVersion (SOAP)</span></span>

<span data-ttu-id="cf2b0-104">O elemento **RequestedVersion** Especifica a versão mínima do serviço que o cliente quer a solicitação a serem processados em.</span><span class="sxs-lookup"><span data-stu-id="cf2b0-104">The **RequestedVersion** element specifies the minimum service version that the client wants the request to be processed on.</span></span> 
  
```XML
<RequestedVersion/>
```

 <span data-ttu-id="cf2b0-105">**ExchangeVersion**</span><span class="sxs-lookup"><span data-stu-id="cf2b0-105">**ExchangeVersion**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cf2b0-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="cf2b0-106">Attributes and elements</span></span>

<span data-ttu-id="cf2b0-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="cf2b0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cf2b0-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="cf2b0-108">Attributes</span></span>

<span data-ttu-id="cf2b0-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cf2b0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cf2b0-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="cf2b0-110">Child elements</span></span>

<span data-ttu-id="cf2b0-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cf2b0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cf2b0-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="cf2b0-112">Parent elements</span></span>

|<span data-ttu-id="cf2b0-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cf2b0-113">**Element**</span></span>|<span data-ttu-id="cf2b0-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cf2b0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf2b0-115">Solicitação (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cf2b0-115">Request (SOAP)</span></span>](request-soap.md) <br/> |<span data-ttu-id="cf2b0-116">Contém as definições de configuração solicitado e os usuários de destino.</span><span class="sxs-lookup"><span data-stu-id="cf2b0-116">Contains the requested configuration settings and the target users.</span></span>  <br/> |
|[<span data-ttu-id="cf2b0-117">Solicitação (GetDomainSettings) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cf2b0-117">Request (GetDomainSettings) (SOAP)</span></span>](request-getdomainsettingssoap.md) <br/> |<span data-ttu-id="cf2b0-118">Representa uma solicitação para obter as configurações de domínio.</span><span class="sxs-lookup"><span data-stu-id="cf2b0-118">Represents a request to get domain settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cf2b0-119">Text value</span><span class="sxs-lookup"><span data-stu-id="cf2b0-119">Text value</span></span>

<span data-ttu-id="cf2b0-120">O valor de texto para o elemento **RequestedVersion** pode ser Exchange2010, Exchange2010_SP1, Exchange2010_SP2 ou Exchange2013.</span><span class="sxs-lookup"><span data-stu-id="cf2b0-120">The text value for the **RequestedVersion** element can be Exchange2010, Exchange2010_SP1, Exchange2010_SP2, or Exchange2013.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cf2b0-121">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="cf2b0-121">Remarks</span></span>

<span data-ttu-id="cf2b0-122">Se esse elemento não estiver presente, a versão mais recente do serviço é usada.</span><span class="sxs-lookup"><span data-stu-id="cf2b0-122">If this element is not present, the latest service version is used.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cf2b0-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="cf2b0-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cf2b0-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="cf2b0-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="cf2b0-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="cf2b0-125">Schema Name</span></span>  <br/> |<span data-ttu-id="cf2b0-126">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="cf2b0-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="cf2b0-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="cf2b0-127">Validation File</span></span>  <br/> |<span data-ttu-id="cf2b0-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="cf2b0-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cf2b0-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="cf2b0-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="cf2b0-130">False</span><span class="sxs-lookup"><span data-stu-id="cf2b0-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cf2b0-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="cf2b0-131">See also</span></span>



[<span data-ttu-id="cf2b0-132">Operação de GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cf2b0-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="cf2b0-133">Operação de GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cf2b0-133">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

