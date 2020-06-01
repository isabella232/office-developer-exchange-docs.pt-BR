---
title: Atribuição (PersonaAttributionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dc59e17e-baea-4617-8ca1-4382a89de0d7
description: O elemento de atribuição especifica uma instância em uma matriz de atributos para um elemento Personatype.
ms.openlocfilehash: 05b0d41c116f2ed7b8dbb3ac44108bb879256b5c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464172"
---
# <a name="attribution-personaattributiontype"></a><span data-ttu-id="7e962-103">Atribuição (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="7e962-103">Attribution (PersonaAttributionType)</span></span>

<span data-ttu-id="7e962-104">O elemento de **atribuição** especifica uma instância em uma matriz de atributos para um elemento **personatype** .</span><span class="sxs-lookup"><span data-stu-id="7e962-104">The **Attribution** element specifies an instance in an array of attributes for a **PersonaType** element.</span></span> 
  
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

 <span data-ttu-id="7e962-105">**PersonaAttributionType**</span><span class="sxs-lookup"><span data-stu-id="7e962-105">**PersonaAttributionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7e962-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="7e962-106">Attributes and elements</span></span>

<span data-ttu-id="7e962-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7e962-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e962-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="7e962-108">Attributes</span></span>

<span data-ttu-id="7e962-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7e962-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7e962-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7e962-110">Child elements</span></span>

|<span data-ttu-id="7e962-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7e962-111">**Element**</span></span>|<span data-ttu-id="7e962-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7e962-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e962-113">ID (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="7e962-113">ID (String)</span></span>](id-string.md) <br/> |<span data-ttu-id="7e962-114">Especifica uma cadeia de caracteres que identifica exclusivamente um aplicativo ou uma atribuição em uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="7e962-114">Specifies a string that uniquely identifies an app or an attribution in a persona.</span></span>  <br/> |
|[<span data-ttu-id="7e962-115">SourceId</span><span class="sxs-lookup"><span data-stu-id="7e962-115">SourceId</span></span>](sourceid.md) <br/> |<span data-ttu-id="7e962-116">Especifica o identificador do contato ou destinatário do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7e962-116">Specifies the identifier of the contact or Active Directory recipient.</span></span>  <br/> |
|[<span data-ttu-id="7e962-117">DisplayName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="7e962-117">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="7e962-118">Define o nome de exibição de uma pasta, contato, lista de distribuição, usuário delegado ou regra.</span><span class="sxs-lookup"><span data-stu-id="7e962-118">Defines the display name of a folder, contact, distribution list, delegate user, or rule.</span></span>  <br/> |
|[<span data-ttu-id="7e962-119">Iswritable</span><span class="sxs-lookup"><span data-stu-id="7e962-119">IsWritable</span></span>](iswritable.md) <br/> |<span data-ttu-id="7e962-120">Especifica se o contato subjacente ou destinatário do Active Directory pode ser gravado.</span><span class="sxs-lookup"><span data-stu-id="7e962-120">Specifies whether the underlying contact or Active Directory recipient can be written to.</span></span>  <br/> |
|[<span data-ttu-id="7e962-121">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="7e962-121">IsQuickContact</span></span>](isquickcontact.md) <br/> |<span data-ttu-id="7e962-122">Especifica um valor Boolean que indica se o contato subjacente ou o destinatário do Active Directory é um contato rápido.</span><span class="sxs-lookup"><span data-stu-id="7e962-122">Specifies a Boolean value that indicates whether the underlying contact or Active Directory recipient is a quick contact.</span></span>  <br/> |
|[<span data-ttu-id="7e962-123">IsHidden</span><span class="sxs-lookup"><span data-stu-id="7e962-123">IsHidden</span></span>](ishidden.md) <br/> |<span data-ttu-id="7e962-124">Contém um valor booliano que indica se o contato subjacente ou o destinatário do Active Directory deve ser oculto ou exibido como parte do persona.</span><span class="sxs-lookup"><span data-stu-id="7e962-124">Contains a Boolean value that indicates whether the underlying contact or Active Directory recipient should be hidden or displayed as part of the persona.</span></span>  <br/> |
|[<span data-ttu-id="7e962-125">FolderId</span><span class="sxs-lookup"><span data-stu-id="7e962-125">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="7e962-126">Contém o identificador e a chave de alteração de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="7e962-126">Contains the identifier and change key of a folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7e962-127">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7e962-127">Parent elements</span></span>

|<span data-ttu-id="7e962-128">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7e962-128">**Element**</span></span>|<span data-ttu-id="7e962-129">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7e962-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e962-130">Atribuições (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="7e962-130">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md) <br/> |<span data-ttu-id="7e962-131">Especifica uma matriz de informações de atribuição para um ou mais destinatários de contatos ou do Active Directory (AD) agregados no persona associado.</span><span class="sxs-lookup"><span data-stu-id="7e962-131">Specifies an array of attribution information for one or more of the contacts or active directory (AD) recipients aggregated into the associated persona.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7e962-132">Comentários</span><span class="sxs-lookup"><span data-stu-id="7e962-132">Remarks</span></span>

<span data-ttu-id="7e962-133">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7e962-133">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7e962-134">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7e962-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7e962-135">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="7e962-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e962-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="7e962-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7e962-137">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7e962-137">Schema Name</span></span>  <br/> |<span data-ttu-id="7e962-138">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="7e962-138">Type schema</span></span>  <br/> |
|<span data-ttu-id="7e962-139">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7e962-139">Validation File</span></span>  <br/> |<span data-ttu-id="7e962-140">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="7e962-140">types.xsd</span></span>  <br/> |
|<span data-ttu-id="7e962-141">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="7e962-141">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="7e962-142">Também consulte</span><span class="sxs-lookup"><span data-stu-id="7e962-142">See also</span></span>

- [<span data-ttu-id="7e962-143">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7e962-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

