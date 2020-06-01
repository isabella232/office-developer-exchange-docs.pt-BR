---
title: RetentionPolicyTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f46679d0-9236-41e2-8624-72300079c67c
description: O elemento RetentionPolicyTag especifica a política de retenção para um item de caixa de correio.
ms.openlocfilehash: 3ece841e14e6cf11ab15e4a4d8b83a778ae32e46
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465174"
---
# <a name="retentionpolicytag"></a><span data-ttu-id="091e8-103">RetentionPolicyTag</span><span class="sxs-lookup"><span data-stu-id="091e8-103">RetentionPolicyTag</span></span>

<span data-ttu-id="091e8-104">O elemento **RetentionPolicyTag** especifica a política de retenção para um item de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="091e8-104">The **RetentionPolicyTag** element specifies the retention policy for a mailbox item.</span></span> 
  
```XML
<RetentionPolicyTag>
   <DisplayName/>
   <RetentionId/>
   <RetentionPeriod/>
   <Type/>
   <RetentionAction/>
   <Description/>
   <IsVisible/>
   <OptedInto/>
   <IsArchive/>
</RetentionPolicyTag>
```

 <span data-ttu-id="091e8-105">**RetentionPolicyTagType**</span><span class="sxs-lookup"><span data-stu-id="091e8-105">**RetentionPolicyTagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="091e8-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="091e8-106">Attributes and elements</span></span>

<span data-ttu-id="091e8-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="091e8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="091e8-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="091e8-108">Attributes</span></span>

<span data-ttu-id="091e8-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="091e8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="091e8-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="091e8-110">Child elements</span></span>

<span data-ttu-id="091e8-111">[DisplayName (cadeia de caracteres)](displayname-string.md)  |  [RetentionId](retentionid.md)  |  [RetentionPeriod](retentionperiod.md)  |  [Tipo (ElcFolderType)](type-elcfoldertype.md)  |  [RetentionAction](retentionaction.md)  |  [Descrição](description.md)  |  [IsVisible](isvisible.md)  |  [OptedInto](optedinto.md)  |  [IsArchive](isarchive.md)</span><span class="sxs-lookup"><span data-stu-id="091e8-111">[DisplayName (string)](displayname-string.md) | [RetentionId](retentionid.md) | [RetentionPeriod](retentionperiod.md) | [Type (ElcFolderType)](type-elcfoldertype.md) | [RetentionAction](retentionaction.md) | [Description](description.md) | [IsVisible](isvisible.md) | [OptedInto](optedinto.md) | [IsArchive](isarchive.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="091e8-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="091e8-112">Parent elements</span></span>

[<span data-ttu-id="091e8-113">RetentionPolicyTags</span><span class="sxs-lookup"><span data-stu-id="091e8-113">RetentionPolicyTags</span></span>](retentionpolicytags.md)
  
## <a name="remarks"></a><span data-ttu-id="091e8-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="091e8-114">Remarks</span></span>

<span data-ttu-id="091e8-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="091e8-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="091e8-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="091e8-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="091e8-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="091e8-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="091e8-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="091e8-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="091e8-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="091e8-119">Schema name</span></span>  <br/> |<span data-ttu-id="091e8-120">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="091e8-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="091e8-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="091e8-121">Validation file</span></span>  <br/> |<span data-ttu-id="091e8-122">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="091e8-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="091e8-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="091e8-123">Can be empty</span></span>  <br/> ||
   

