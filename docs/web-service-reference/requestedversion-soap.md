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
description: O elemento RequestedVersion especifica a versão mínima do serviço que o cliente deseja que a solicitação seja processada.
ms.openlocfilehash: ded276b3eb2c70b6edd39ca12289098de2b3faea
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459164"
---
# <a name="requestedversion-soap"></a><span data-ttu-id="de5f3-103">RequestedVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="de5f3-103">RequestedVersion (SOAP)</span></span>

<span data-ttu-id="de5f3-104">O elemento **RequestedVersion** especifica a versão mínima do serviço que o cliente deseja que a solicitação seja processada.</span><span class="sxs-lookup"><span data-stu-id="de5f3-104">The **RequestedVersion** element specifies the minimum service version that the client wants the request to be processed on.</span></span> 
  
```XML
<RequestedVersion/>
```

 <span data-ttu-id="de5f3-105">**ExchangeVersion**</span><span class="sxs-lookup"><span data-stu-id="de5f3-105">**ExchangeVersion**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="de5f3-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="de5f3-106">Attributes and elements</span></span>

<span data-ttu-id="de5f3-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="de5f3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="de5f3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="de5f3-108">Attributes</span></span>

<span data-ttu-id="de5f3-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="de5f3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="de5f3-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="de5f3-110">Child elements</span></span>

<span data-ttu-id="de5f3-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="de5f3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="de5f3-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="de5f3-112">Parent elements</span></span>

|<span data-ttu-id="de5f3-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="de5f3-113">**Element**</span></span>|<span data-ttu-id="de5f3-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="de5f3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="de5f3-115">Solicitação (SOAP)</span><span class="sxs-lookup"><span data-stu-id="de5f3-115">Request (SOAP)</span></span>](request-soap.md) <br/> |<span data-ttu-id="de5f3-116">Contém as definições de configuração solicitadas e os usuários de destino.</span><span class="sxs-lookup"><span data-stu-id="de5f3-116">Contains the requested configuration settings and the target users.</span></span>  <br/> |
|[<span data-ttu-id="de5f3-117">Solicitação (GetDomainSettings) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="de5f3-117">Request (GetDomainSettings) (SOAP)</span></span>](request-getdomainsettingssoap.md) <br/> |<span data-ttu-id="de5f3-118">Representa uma solicitação para obter as configurações de domínio.</span><span class="sxs-lookup"><span data-stu-id="de5f3-118">Represents a request to get domain settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="de5f3-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="de5f3-119">Text value</span></span>

<span data-ttu-id="de5f3-120">O valor de texto para o elemento **RequestedVersion** pode ser Exchange2010, Exchange2010_SP1, Exchange2010_SP2 ou Exchange2013.</span><span class="sxs-lookup"><span data-stu-id="de5f3-120">The text value for the **RequestedVersion** element can be Exchange2010, Exchange2010_SP1, Exchange2010_SP2, or Exchange2013.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="de5f3-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="de5f3-121">Remarks</span></span>

<span data-ttu-id="de5f3-122">Se esse elemento não estiver presente, será usada a versão mais recente do serviço.</span><span class="sxs-lookup"><span data-stu-id="de5f3-122">If this element is not present, the latest service version is used.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="de5f3-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="de5f3-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="de5f3-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="de5f3-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="de5f3-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="de5f3-125">Schema Name</span></span>  <br/> |<span data-ttu-id="de5f3-126">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="de5f3-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="de5f3-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="de5f3-127">Validation File</span></span>  <br/> |<span data-ttu-id="de5f3-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="de5f3-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="de5f3-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="de5f3-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="de5f3-130">False</span><span class="sxs-lookup"><span data-stu-id="de5f3-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="de5f3-131">Confira também</span><span class="sxs-lookup"><span data-stu-id="de5f3-131">See also</span></span>



[<span data-ttu-id="de5f3-132">Operação GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="de5f3-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="de5f3-133">Operação GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="de5f3-133">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

