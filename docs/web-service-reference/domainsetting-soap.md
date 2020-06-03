---
title: DomainSetting (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: bad5399c-0762-4979-9c15-58cf4b7b6278
description: O elemento DomainSetting contém configurações de domínio retornadas pela solicitação de operação de operação de GetDomainSettings (SOAP).
ms.openlocfilehash: 54441dd7cfcf7372807a1e6bfd8ea5d26805bffc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526295"
---
# <a name="domainsetting-soap"></a><span data-ttu-id="c368e-103">DomainSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c368e-103">DomainSetting (SOAP)</span></span>

<span data-ttu-id="c368e-104">O elemento **DomainSetting** contém configurações de domínio retornadas pela solicitação de operação de operação de [GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="c368e-104">The **DomainSetting** element contains domain settings that are returned by the [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) operation request.</span></span> 
  
```XML
<DomainSetting>
   <Name/>
</DomainSetting>
```

 <span data-ttu-id="c368e-105">**DomainSetting**</span><span class="sxs-lookup"><span data-stu-id="c368e-105">**DomainSetting**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c368e-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c368e-106">Attributes and elements</span></span>

<span data-ttu-id="c368e-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c368e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c368e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c368e-108">Attributes</span></span>

<span data-ttu-id="c368e-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c368e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c368e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c368e-110">Child elements</span></span>

|<span data-ttu-id="c368e-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c368e-111">**Element**</span></span>|<span data-ttu-id="c368e-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c368e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c368e-113">Nome (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c368e-113">Name (SOAP)</span></span>](name-soap.md) <br/> |<span data-ttu-id="c368e-114">Representa o nome de uma configuração.</span><span class="sxs-lookup"><span data-stu-id="c368e-114">Represents the name of a setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c368e-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c368e-115">Parent elements</span></span>

|<span data-ttu-id="c368e-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c368e-116">**Element**</span></span>|<span data-ttu-id="c368e-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c368e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c368e-118">DomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c368e-118">DomainSettings (SOAP)</span></span>](domainsettings-soap.md) <br/> |<span data-ttu-id="c368e-119">Representa as configurações de domínio que foram enviadas em uma solicitação de descoberta automática ou retornadas por uma resposta de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="c368e-119">Represents the domain settings that were submitted in an Autodiscover request or returned by an Autodiscover response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c368e-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="c368e-120">Text value</span></span>

<span data-ttu-id="c368e-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c368e-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c368e-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c368e-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c368e-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="c368e-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="c368e-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c368e-124">Schema Name</span></span>  <br/> |<span data-ttu-id="c368e-125">Esquema de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="c368e-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="c368e-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c368e-126">Validation File</span></span>  <br/> |<span data-ttu-id="c368e-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c368e-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c368e-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c368e-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="c368e-129">Verdadeiro</span><span class="sxs-lookup"><span data-stu-id="c368e-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c368e-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="c368e-130">See also</span></span>

- [<span data-ttu-id="c368e-131">Operação GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c368e-131">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

