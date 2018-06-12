---
title: PolicyTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fa4b1447-dc7b-47ad-a677-78fcee443dc6
description: O elemento PolicyTag Especifica o identificador de retenção em um item ou pasta.
ms.openlocfilehash: d6cd5aab1145f6006912541c8f8c1d0a91d1e17e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824835"
---
# <a name="policytag"></a><span data-ttu-id="91833-103">PolicyTag</span><span class="sxs-lookup"><span data-stu-id="91833-103">PolicyTag</span></span>

<span data-ttu-id="91833-104">O elemento **PolicyTag** Especifica o identificador de retenção em um item ou pasta.</span><span class="sxs-lookup"><span data-stu-id="91833-104">The **PolicyTag** element specifies the retention identifier on an item or folder.</span></span> 
  
```xml
<PolicyTag IsExplicit="true | false"></PolicyTag>
```

 <span data-ttu-id="91833-105">**RetentionTagType**</span><span class="sxs-lookup"><span data-stu-id="91833-105">**RetentionTagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="91833-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="91833-106">Attributes and elements</span></span>

<span data-ttu-id="91833-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="91833-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="91833-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="91833-108">Attributes</span></span>

|<span data-ttu-id="91833-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="91833-109">**Attribute**</span></span>|<span data-ttu-id="91833-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="91833-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="91833-111">IsExplicit</span><span class="sxs-lookup"><span data-stu-id="91833-111">IsExplicit</span></span>  <br/> |<span data-ttu-id="91833-112">Indica se uma marca de política foi explicitamente definida em um item ou pasta.</span><span class="sxs-lookup"><span data-stu-id="91833-112">Indicates whether a policy tag was explicitly set on an item or folder.</span></span>  <br/> <span data-ttu-id="91833-113">Um valor de texto de **true** para o atributo **IsExplicit** indica que a marca da diretiva foi explicitamente definida no item ou na pasta.</span><span class="sxs-lookup"><span data-stu-id="91833-113">A text value of **true** for the **IsExplicit** attribute indicates that the policy tag was explicitly set on the item or folder.</span></span> <span data-ttu-id="91833-114">Um valor de texto de **false** indica que a marca da diretiva implicitamente foi definida no item ou na pasta com base na marca de política de pasta pai.</span><span class="sxs-lookup"><span data-stu-id="91833-114">A text value of **false** indicates that the policy tag was implicitly set on the item or folder based on the parent folder policy tag.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="91833-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="91833-115">Child elements</span></span>

<span data-ttu-id="91833-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="91833-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="91833-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="91833-117">Parent elements</span></span>

<span data-ttu-id="91833-118">[SearchPreviewItem](searchpreviewitem.md) | [Item](item.md) | [contato](contact.md) | [mensagem](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [tarefa](task.md)</span><span class="sxs-lookup"><span data-stu-id="91833-118">[SearchPreviewItem](searchpreviewitem.md) | [Item](item.md) | [Contact](contact.md) | [Message](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="91833-119">Text value</span><span class="sxs-lookup"><span data-stu-id="91833-119">Text value</span></span>

<span data-ttu-id="91833-120">O valor de texto do elemento **PolicyTag** é o identificador de marca de política.</span><span class="sxs-lookup"><span data-stu-id="91833-120">The text value of the **PolicyTag** element is the policy tag identifier.</span></span> <span data-ttu-id="91833-121">O identificador de marca de política é um GUID.</span><span class="sxs-lookup"><span data-stu-id="91833-121">The policy tag identifier is a GUID.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="91833-122">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="91833-122">Remarks</span></span>

<span data-ttu-id="91833-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="91833-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="91833-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="91833-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="91833-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="91833-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="91833-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="91833-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="91833-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="91833-127">Schema name</span></span>  <br/> |<span data-ttu-id="91833-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="91833-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="91833-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="91833-129">Validation file</span></span>  <br/> |<span data-ttu-id="91833-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="91833-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="91833-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="91833-131">Can be empty</span></span>  <br/> ||
   

