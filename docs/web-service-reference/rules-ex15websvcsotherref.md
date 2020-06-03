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
description: O elemento rules contém uma matriz de regras de proteção.
ms.openlocfilehash: d848abfe0c97d07836f28bc75806f506c5433d44
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464935"
---
# <a name="rules"></a><span data-ttu-id="90bde-103">Regras</span><span class="sxs-lookup"><span data-stu-id="90bde-103">Rules</span></span>

<span data-ttu-id="90bde-104">O elemento **Rules** contém uma matriz de regras de proteção.</span><span class="sxs-lookup"><span data-stu-id="90bde-104">The **Rules** element contains an array of protection rules.</span></span> 
  
```xml
<Rules>   <Rule/></Rules>
```

 <span data-ttu-id="90bde-105">**ArrayOfProtectionRulesType**</span><span class="sxs-lookup"><span data-stu-id="90bde-105">**ArrayOfProtectionRulesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="90bde-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="90bde-106">Attributes and elements</span></span>

<span data-ttu-id="90bde-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="90bde-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="90bde-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="90bde-108">Attributes</span></span>

<span data-ttu-id="90bde-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="90bde-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="90bde-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="90bde-110">Child elements</span></span>

|<span data-ttu-id="90bde-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="90bde-111">**Element**</span></span>|<span data-ttu-id="90bde-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="90bde-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="90bde-113">Rule</span><span class="sxs-lookup"><span data-stu-id="90bde-113">Rule</span></span>](rule.md) <br/> |<span data-ttu-id="90bde-114">Contém uma única regra de proteção.</span><span class="sxs-lookup"><span data-stu-id="90bde-114">Contains a single protection rule.</span></span> <span data-ttu-id="90bde-115">Este elemento pode ocorrer zero ou mais vezes.</span><span class="sxs-lookup"><span data-stu-id="90bde-115">This element can occur zero or more times.</span></span> <span data-ttu-id="90bde-116">Esse elemento ocorre sem nenhuma hora quando nenhuma regra de proteção é definida pela organização.</span><span class="sxs-lookup"><span data-stu-id="90bde-116">This element occurs zero times when no protection rules are defined by the organization.</span></span> <span data-ttu-id="90bde-117">Ela ocorre uma ou mais vezes se pelo menos uma regra for definida pela organização.</span><span class="sxs-lookup"><span data-stu-id="90bde-117">It occurs one or more times if at least one rule is defined by the organization.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="90bde-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="90bde-118">Parent elements</span></span>

|<span data-ttu-id="90bde-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="90bde-119">**Element**</span></span>|<span data-ttu-id="90bde-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="90bde-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="90bde-121">ProtectionRulesConfiguration</span><span class="sxs-lookup"><span data-stu-id="90bde-121">ProtectionRulesConfiguration</span></span>](protectionrulesconfiguration.md) <br/> |<span data-ttu-id="90bde-122">Contém a configuração de serviço para o serviço de regras de proteção.</span><span class="sxs-lookup"><span data-stu-id="90bde-122">Contains service configuration for the protection rules service.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="90bde-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="90bde-123">Remarks</span></span>

<span data-ttu-id="90bde-124">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="90bde-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="90bde-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="90bde-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="90bde-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="90bde-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="90bde-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="90bde-127">Schema Name</span></span>  <br/> |<span data-ttu-id="90bde-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="90bde-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="90bde-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="90bde-129">Validation File</span></span>  <br/> |<span data-ttu-id="90bde-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="90bde-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="90bde-131">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="90bde-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="90bde-132">False</span><span class="sxs-lookup"><span data-stu-id="90bde-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="90bde-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="90bde-133">See also</span></span>



- [<span data-ttu-id="90bde-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="90bde-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

