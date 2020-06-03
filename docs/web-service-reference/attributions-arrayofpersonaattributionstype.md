---
title: Atribuições (ArrayOfPersonaAttributionsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f61d843c-bca5-4c88-9667-fd03d2a963a1
description: O elemento de atribuições especifica uma matriz de informações de atribuição para um ou mais dos destinatários de contatos ou do Active Directory agregados ao persona associado.
ms.openlocfilehash: a9883e06a8adbd5c9d3bc7e1edd28c62418df653
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460320"
---
# <a name="attributions-arrayofpersonaattributionstype"></a><span data-ttu-id="0cbdc-103">Atribuições (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="0cbdc-103">Attributions (ArrayOfPersonaAttributionsType)</span></span>

<span data-ttu-id="0cbdc-104">O elemento de **atribuições** especifica uma matriz de informações de atribuição para um ou mais dos destinatários de contatos ou do Active Directory agregados ao persona associado.</span><span class="sxs-lookup"><span data-stu-id="0cbdc-104">The **Attributions** element specifies an array of attribution information for one or more of the contacts or Active Directory recipients aggregated into the associated persona.</span></span> 
  
```XML
<Attributions>
    <Attribution></Attribution>
</Attributions>
```

 <span data-ttu-id="0cbdc-105">**ArrayOfPersonaAttributionsType**</span><span class="sxs-lookup"><span data-stu-id="0cbdc-105">**ArrayOfPersonaAttributionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0cbdc-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="0cbdc-106">Attributes and elements</span></span>

<span data-ttu-id="0cbdc-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0cbdc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0cbdc-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0cbdc-108">Attributes</span></span>

<span data-ttu-id="0cbdc-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0cbdc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0cbdc-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0cbdc-110">Child elements</span></span>

|<span data-ttu-id="0cbdc-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0cbdc-111">**Element**</span></span>|<span data-ttu-id="0cbdc-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0cbdc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0cbdc-113">Atribuição (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="0cbdc-113">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md) <br/> |<span data-ttu-id="0cbdc-114">Especifica uma instância em uma matriz de atributos para um elemento **personatype** .</span><span class="sxs-lookup"><span data-stu-id="0cbdc-114">Specifies an instance in an array of attributes for a **PersonaType** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0cbdc-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0cbdc-115">Parent elements</span></span>

|<span data-ttu-id="0cbdc-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0cbdc-116">**Element**</span></span>|<span data-ttu-id="0cbdc-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0cbdc-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0cbdc-118">Pessoal</span><span class="sxs-lookup"><span data-stu-id="0cbdc-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="0cbdc-119">Especifica um conjunto de dados persona retornados por uma solicitação **Getpersona** .</span><span class="sxs-lookup"><span data-stu-id="0cbdc-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0cbdc-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="0cbdc-120">Remarks</span></span>

<span data-ttu-id="0cbdc-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0cbdc-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0cbdc-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0cbdc-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0cbdc-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="0cbdc-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0cbdc-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="0cbdc-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0cbdc-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0cbdc-125">Schema Name</span></span>  <br/> |<span data-ttu-id="0cbdc-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="0cbdc-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="0cbdc-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0cbdc-127">Validation File</span></span>  <br/> |<span data-ttu-id="0cbdc-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="0cbdc-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="0cbdc-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="0cbdc-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="0cbdc-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="0cbdc-130">See also</span></span>

- [<span data-ttu-id="0cbdc-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0cbdc-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

