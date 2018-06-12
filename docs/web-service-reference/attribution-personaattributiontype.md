---
title: Atribuição (PersonaAttributionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dc59e17e-baea-4617-8ca1-4382a89de0d7
description: O elemento de atribuição Especifica uma instância em uma matriz de atributos de um elemento PersonaType.
ms.openlocfilehash: 0e800c92c75bf0c475d4bffd33d6ab49f9ad9a9a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751233"
---
# <a name="attribution-personaattributiontype"></a><span data-ttu-id="31ff4-103">Atribuição (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="31ff4-103">Attribution (PersonaAttributionType)</span></span>

<span data-ttu-id="31ff4-104">O elemento de **atribuição** Especifica uma instância em uma matriz de atributos de um elemento **PersonaType** .</span><span class="sxs-lookup"><span data-stu-id="31ff4-104">The **Attribution** element specifies an instance in an array of attributes for a **PersonaType** element.</span></span> 
  
```XML
<Attribution>
    <Id></Id>
    <SourceId></SourceId>
    <DisplayName></DisplayName>
    <IsWritable></IsWritable>
    <IsQuickContact></IsQuickContact>
    <IsHidden></IsHidden>
    <FolderId></FolderId>
</Attribution>
```

 <span data-ttu-id="31ff4-105">**PersonaAttributionType**</span><span class="sxs-lookup"><span data-stu-id="31ff4-105">**PersonaAttributionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="31ff4-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="31ff4-106">Attributes and elements</span></span>

<span data-ttu-id="31ff4-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="31ff4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="31ff4-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="31ff4-108">Attributes</span></span>

<span data-ttu-id="31ff4-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="31ff4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="31ff4-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="31ff4-110">Child elements</span></span>

|<span data-ttu-id="31ff4-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="31ff4-111">**Element**</span></span>|<span data-ttu-id="31ff4-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="31ff4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="31ff4-113">ID (String)</span><span class="sxs-lookup"><span data-stu-id="31ff4-113">ID (String)</span></span>](id-string.md) <br/> |<span data-ttu-id="31ff4-114">Especifica uma cadeia de caracteres que identifica exclusivamente uma atribuição de uma pessoa ou de um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="31ff4-114">Specifies a string that uniquely identifies an app or an attribution in a persona.</span></span>  <br/> |
|[<span data-ttu-id="31ff4-115">SourceId</span><span class="sxs-lookup"><span data-stu-id="31ff4-115">SourceId</span></span>](sourceid.md) <br/> |<span data-ttu-id="31ff4-116">Especifica o identificador do contato ou destinatário do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="31ff4-116">Specifies the identifier of the contact or Active Directory recipient.</span></span>  <br/> |
|[<span data-ttu-id="31ff4-117">DisplayName (string)</span><span class="sxs-lookup"><span data-stu-id="31ff4-117">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="31ff4-118">Define o nome de exibição de uma pasta, o contato, a lista de distribuição, o usuário delegado ou a regra.</span><span class="sxs-lookup"><span data-stu-id="31ff4-118">Defines the display name of a folder, contact, distribution list, delegate user, or rule.</span></span>  <br/> |
|[<span data-ttu-id="31ff4-119">IsWritable</span><span class="sxs-lookup"><span data-stu-id="31ff4-119">IsWritable</span></span>](iswritable.md) <br/> |<span data-ttu-id="31ff4-120">Especifica se o contato subjacente ou o destinatário do Active Directory pode ser gravado em.</span><span class="sxs-lookup"><span data-stu-id="31ff4-120">Specifies whether the underlying contact or Active Directory recipient can be written to.</span></span>  <br/> |
|[<span data-ttu-id="31ff4-121">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="31ff4-121">IsQuickContact</span></span>](isquickcontact.md) <br/> |<span data-ttu-id="31ff4-122">Especifica um valor Boolean que indica se o contato subjacente ou o destinatário do Active Directory é um contato rápido.</span><span class="sxs-lookup"><span data-stu-id="31ff4-122">Specifies a Boolean value that indicates whether the underlying contact or Active Directory recipient is a quick contact.</span></span>  <br/> |
|[<span data-ttu-id="31ff4-123">IsHidden</span><span class="sxs-lookup"><span data-stu-id="31ff4-123">IsHidden</span></span>](ishidden.md) <br/> |<span data-ttu-id="31ff4-124">Contém um valor Boolean que indica se o destinatário do Active Directory ou o contato subjacente deve ser oculto ou exibido como parte da pessoa.</span><span class="sxs-lookup"><span data-stu-id="31ff4-124">Contains a Boolean value that indicates whether the underlying contact or Active Directory recipient should be hidden or displayed as part of the persona.</span></span>  <br/> |
|[<span data-ttu-id="31ff4-125">FolderId</span><span class="sxs-lookup"><span data-stu-id="31ff4-125">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="31ff4-126">Contém o identificador e alterar a chave de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="31ff4-126">Contains the identifier and change key of a folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="31ff4-127">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="31ff4-127">Parent elements</span></span>

|<span data-ttu-id="31ff4-128">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="31ff4-128">**Element**</span></span>|<span data-ttu-id="31ff4-129">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="31ff4-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="31ff4-130">Atribuições (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="31ff4-130">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md) <br/> |<span data-ttu-id="31ff4-131">Especifica uma matriz das informações de atribuição para uma ou mais contatos ou destinatários do active directory (AD) agregados em que a pessoa associada.</span><span class="sxs-lookup"><span data-stu-id="31ff4-131">Specifies an array of attribution information for one or more of the contacts or active directory (AD) recipients aggregated into the associated persona.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="31ff4-132">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="31ff4-132">Remarks</span></span>

<span data-ttu-id="31ff4-133">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="31ff4-133">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="31ff4-134">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="31ff4-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="31ff4-135">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="31ff4-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="31ff4-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="31ff4-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="31ff4-137">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="31ff4-137">Schema Name</span></span>  <br/> |<span data-ttu-id="31ff4-138">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="31ff4-138">Type schema</span></span>  <br/> |
|<span data-ttu-id="31ff4-139">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="31ff4-139">Validation File</span></span>  <br/> |<span data-ttu-id="31ff4-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="31ff4-140">types.xsd</span></span>  <br/> |
|<span data-ttu-id="31ff4-141">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="31ff4-141">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="31ff4-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="31ff4-142">See also</span></span>

- [<span data-ttu-id="31ff4-143">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="31ff4-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

