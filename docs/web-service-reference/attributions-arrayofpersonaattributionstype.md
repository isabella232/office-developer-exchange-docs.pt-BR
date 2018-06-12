---
title: Atribuições (ArrayOfPersonaAttributionsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f61d843c-bca5-4c88-9667-fd03d2a963a1
description: O elemento de atribuições Especifica uma matriz de informações de atribuição de um ou mais contatos ou destinatários do Active Directory agregados em que a pessoa associada.
ms.openlocfilehash: 52fecb4e4381d5e9dbbaf7134fa18068ba15f6ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751232"
---
# <a name="attributions-arrayofpersonaattributionstype"></a><span data-ttu-id="2da44-103">Atribuições (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="2da44-103">Attributions (ArrayOfPersonaAttributionsType)</span></span>

<span data-ttu-id="2da44-104">O elemento de **atribuições** Especifica uma matriz de informações de atribuição de um ou mais contatos ou destinatários do Active Directory agregados em que a pessoa associada.</span><span class="sxs-lookup"><span data-stu-id="2da44-104">The **Attributions** element specifies an array of attribution information for one or more of the contacts or Active Directory recipients aggregated into the associated persona.</span></span> 
  
```XML
<Attributions>
    <Attribution></Attribution>
</Attributions>
```

 <span data-ttu-id="2da44-105">**ArrayOfPersonaAttributionsType**</span><span class="sxs-lookup"><span data-stu-id="2da44-105">**ArrayOfPersonaAttributionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2da44-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="2da44-106">Attributes and elements</span></span>

<span data-ttu-id="2da44-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2da44-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2da44-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2da44-108">Attributes</span></span>

<span data-ttu-id="2da44-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2da44-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2da44-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2da44-110">Child elements</span></span>

|<span data-ttu-id="2da44-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2da44-111">**Element**</span></span>|<span data-ttu-id="2da44-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2da44-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2da44-113">Atribuição (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="2da44-113">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md) <br/> |<span data-ttu-id="2da44-114">Especifica uma instância em uma matriz de atributos de um elemento **PersonaType** .</span><span class="sxs-lookup"><span data-stu-id="2da44-114">Specifies an instance in an array of attributes for a **PersonaType** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2da44-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2da44-115">Parent elements</span></span>

|<span data-ttu-id="2da44-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2da44-116">**Element**</span></span>|<span data-ttu-id="2da44-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2da44-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2da44-118">Pessoa</span><span class="sxs-lookup"><span data-stu-id="2da44-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="2da44-119">Especifica um conjunto de dados de pessoa retornados por uma solicitação **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="2da44-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2da44-120">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="2da44-120">Remarks</span></span>

<span data-ttu-id="2da44-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2da44-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2da44-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2da44-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2da44-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="2da44-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2da44-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="2da44-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2da44-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2da44-125">Schema Name</span></span>  <br/> |<span data-ttu-id="2da44-126">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="2da44-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="2da44-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2da44-127">Validation File</span></span>  <br/> |<span data-ttu-id="2da44-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2da44-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="2da44-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="2da44-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="2da44-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="2da44-130">See also</span></span>

- [<span data-ttu-id="2da44-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2da44-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

