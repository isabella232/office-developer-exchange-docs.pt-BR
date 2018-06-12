---
title: RetentionPolicyTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f46679d0-9236-41e2-8624-72300079c67c
description: O elemento RetentionPolicyTag Especifica a política de retenção para um item de caixa de correio.
ms.openlocfilehash: 2525f6d7a0ca583342d28dd9f4857a69b3a8c05a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825226"
---
# <a name="retentionpolicytag"></a><span data-ttu-id="f1369-103">RetentionPolicyTag</span><span class="sxs-lookup"><span data-stu-id="f1369-103">RetentionPolicyTag</span></span>

<span data-ttu-id="f1369-104">O elemento **RetentionPolicyTag** Especifica a política de retenção para um item de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="f1369-104">The **RetentionPolicyTag** element specifies the retention policy for a mailbox item.</span></span> 
  
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

 <span data-ttu-id="f1369-105">**RetentionPolicyTagType**</span><span class="sxs-lookup"><span data-stu-id="f1369-105">**RetentionPolicyTagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f1369-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f1369-106">Attributes and elements</span></span>

<span data-ttu-id="f1369-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f1369-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f1369-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f1369-108">Attributes</span></span>

<span data-ttu-id="f1369-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f1369-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f1369-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f1369-110">Child elements</span></span>

<span data-ttu-id="f1369-111">[DisplayName (string)](displayname-string.md) | [RetentionId](retentionid.md) | [RetentionPeriod](retentionperiod.md) | [tipo (ElcFolderType)](type-elcfoldertype.md) | [RetentionAction](retentionaction.md) | [Descrição](description.md) | [IsVisible](isvisible.md)  |  [OptedInto](optedinto.md) | [IsArchive](isarchive.md)</span><span class="sxs-lookup"><span data-stu-id="f1369-111">[DisplayName (string)](displayname-string.md) | [RetentionId](retentionid.md) | [RetentionPeriod](retentionperiod.md) | [Type (ElcFolderType)](type-elcfoldertype.md) | [RetentionAction](retentionaction.md) | [Description](description.md) | [IsVisible](isvisible.md) | [OptedInto](optedinto.md) | [IsArchive](isarchive.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f1369-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f1369-112">Parent elements</span></span>

[<span data-ttu-id="f1369-113">RetentionPolicyTags</span><span class="sxs-lookup"><span data-stu-id="f1369-113">RetentionPolicyTags</span></span>](retentionpolicytags.md)
  
## <a name="remarks"></a><span data-ttu-id="f1369-114">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="f1369-114">Remarks</span></span>

<span data-ttu-id="f1369-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f1369-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f1369-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f1369-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f1369-117">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f1369-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f1369-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="f1369-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f1369-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f1369-119">Schema name</span></span>  <br/> |<span data-ttu-id="f1369-120">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f1369-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="f1369-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f1369-121">Validation file</span></span>  <br/> |<span data-ttu-id="f1369-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f1369-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f1369-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="f1369-123">Can be empty</span></span>  <br/> ||
   

