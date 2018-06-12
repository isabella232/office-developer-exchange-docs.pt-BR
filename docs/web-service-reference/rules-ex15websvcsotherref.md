---
title: Regras
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Rules
api_type:
- schema
ms.assetid: 53f59054-8f68-4eaa-be9c-ccfc9383bcf2
description: O elemento de regras contém uma matriz de regras de proteção.
ms.openlocfilehash: 5d511f977f3eb3273dc43f56356a059985b2a929
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825269"
---
# <a name="rules"></a><span data-ttu-id="5c51d-103">Regras</span><span class="sxs-lookup"><span data-stu-id="5c51d-103">Rules</span></span>

<span data-ttu-id="5c51d-104">O elemento de **regras** contém uma matriz de regras de proteção.</span><span class="sxs-lookup"><span data-stu-id="5c51d-104">The **Rules** element contains an array of protection rules.</span></span> 
  
```xml
<Rules>   <Rule/></Rules>
```

 <span data-ttu-id="5c51d-105">**ArrayOfProtectionRulesType**</span><span class="sxs-lookup"><span data-stu-id="5c51d-105">**ArrayOfProtectionRulesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5c51d-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="5c51d-106">Attributes and elements</span></span>

<span data-ttu-id="5c51d-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5c51d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5c51d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5c51d-108">Attributes</span></span>

<span data-ttu-id="5c51d-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5c51d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5c51d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5c51d-110">Child elements</span></span>

|<span data-ttu-id="5c51d-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5c51d-111">**Element**</span></span>|<span data-ttu-id="5c51d-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5c51d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c51d-113">Rule</span><span class="sxs-lookup"><span data-stu-id="5c51d-113">Rule</span></span>](rule.md) <br/> |<span data-ttu-id="5c51d-114">Contém uma regra de proteção do único.</span><span class="sxs-lookup"><span data-stu-id="5c51d-114">Contains a single protection rule.</span></span> <span data-ttu-id="5c51d-115">Esse elemento pode ocorrer zero ou mais vezes.</span><span class="sxs-lookup"><span data-stu-id="5c51d-115">This element can occur zero or more times.</span></span> <span data-ttu-id="5c51d-116">Esse elemento ocorre zero vezes quando não há regras de proteção são definidas pela organização.</span><span class="sxs-lookup"><span data-stu-id="5c51d-116">This element occurs zero times when no protection rules are defined by the organization.</span></span> <span data-ttu-id="5c51d-117">Uma ou mais vezes ocorre se não houver pelo menos uma regra definida pela organização.</span><span class="sxs-lookup"><span data-stu-id="5c51d-117">It occurs one or more times if at least one rule is defined by the organization.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5c51d-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5c51d-118">Parent elements</span></span>

|<span data-ttu-id="5c51d-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5c51d-119">**Element**</span></span>|<span data-ttu-id="5c51d-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5c51d-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c51d-121">ProtectionRulesConfiguration</span><span class="sxs-lookup"><span data-stu-id="5c51d-121">ProtectionRulesConfiguration</span></span>](protectionrulesconfiguration.md) <br/> |<span data-ttu-id="5c51d-122">Contém a configuração do serviço para o serviço de regras de proteção.</span><span class="sxs-lookup"><span data-stu-id="5c51d-122">Contains service configuration for the protection rules service.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5c51d-123">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="5c51d-123">Remarks</span></span>

<span data-ttu-id="5c51d-124">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="5c51d-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5c51d-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="5c51d-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5c51d-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="5c51d-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5c51d-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5c51d-127">Schema Name</span></span>  <br/> |<span data-ttu-id="5c51d-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="5c51d-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="5c51d-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5c51d-129">Validation File</span></span>  <br/> |<span data-ttu-id="5c51d-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5c51d-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5c51d-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5c51d-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="5c51d-132">False</span><span class="sxs-lookup"><span data-stu-id="5c51d-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5c51d-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="5c51d-133">See also</span></span>



- [<span data-ttu-id="5c51d-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5c51d-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

