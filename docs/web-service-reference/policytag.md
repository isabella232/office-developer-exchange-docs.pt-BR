---
title: PolicyTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fa4b1447-dc7b-47ad-a677-78fcee443dc6
description: O elemento PolicyTag especifica o identificador de retenção em um item ou pasta.
ms.openlocfilehash: ddc4d890d1e514586ba5ea7f6a8b541b2e4786c7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460894"
---
# <a name="policytag"></a><span data-ttu-id="16eea-103">PolicyTag</span><span class="sxs-lookup"><span data-stu-id="16eea-103">PolicyTag</span></span>

<span data-ttu-id="16eea-104">O elemento **PolicyTag** especifica o identificador de retenção em um item ou pasta.</span><span class="sxs-lookup"><span data-stu-id="16eea-104">The **PolicyTag** element specifies the retention identifier on an item or folder.</span></span> 
  
```xml
<PolicyTag IsExplicit="true | false"></PolicyTag>
```

 <span data-ttu-id="16eea-105">**RetentionTagType**</span><span class="sxs-lookup"><span data-stu-id="16eea-105">**RetentionTagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="16eea-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="16eea-106">Attributes and elements</span></span>

<span data-ttu-id="16eea-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="16eea-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="16eea-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="16eea-108">Attributes</span></span>

|<span data-ttu-id="16eea-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="16eea-109">**Attribute**</span></span>|<span data-ttu-id="16eea-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="16eea-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="16eea-111">Isexplicit</span><span class="sxs-lookup"><span data-stu-id="16eea-111">IsExplicit</span></span>  <br/> |<span data-ttu-id="16eea-112">Indica se uma marca de política foi definida explicitamente em um item ou pasta.</span><span class="sxs-lookup"><span data-stu-id="16eea-112">Indicates whether a policy tag was explicitly set on an item or folder.</span></span>  <br/> <span data-ttu-id="16eea-113">Um valor de texto **true** para o atributo **isexplicit** indica que a marca de política foi explicitamente definida no item ou na pasta.</span><span class="sxs-lookup"><span data-stu-id="16eea-113">A text value of **true** for the **IsExplicit** attribute indicates that the policy tag was explicitly set on the item or folder.</span></span> <span data-ttu-id="16eea-114">Um valor de texto **false** indica que a marca de política foi definida implicitamente no item ou na pasta com base na marca de política de pasta pai.</span><span class="sxs-lookup"><span data-stu-id="16eea-114">A text value of **false** indicates that the policy tag was implicitly set on the item or folder based on the parent folder policy tag.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="16eea-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="16eea-115">Child elements</span></span>

<span data-ttu-id="16eea-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="16eea-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="16eea-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="16eea-117">Parent elements</span></span>

<span data-ttu-id="16eea-118">[SearchPreviewItem](searchpreviewitem.md)  |  [Item](item.md)  |  [Contato](contact.md)  |  [Mensagem](message-ex15websvcsotherref.md)  |  [DistributionList](distributionlist.md)  |  [CalendarItem](calendaritem.md)  |  [PostItem](postitem.md)  |  [Tarefa](task.md)</span><span class="sxs-lookup"><span data-stu-id="16eea-118">[SearchPreviewItem](searchpreviewitem.md) | [Item](item.md) | [Contact](contact.md) | [Message](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="16eea-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="16eea-119">Text value</span></span>

<span data-ttu-id="16eea-120">O valor de texto do elemento **PolicyTag** é o identificador de marca de política.</span><span class="sxs-lookup"><span data-stu-id="16eea-120">The text value of the **PolicyTag** element is the policy tag identifier.</span></span> <span data-ttu-id="16eea-121">O identificador da marca de política é um GUID.</span><span class="sxs-lookup"><span data-stu-id="16eea-121">The policy tag identifier is a GUID.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="16eea-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="16eea-122">Remarks</span></span>

<span data-ttu-id="16eea-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="16eea-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="16eea-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="16eea-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="16eea-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="16eea-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="16eea-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="16eea-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="16eea-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="16eea-127">Schema name</span></span>  <br/> |<span data-ttu-id="16eea-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="16eea-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="16eea-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="16eea-129">Validation file</span></span>  <br/> |<span data-ttu-id="16eea-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="16eea-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="16eea-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="16eea-131">Can be empty</span></span>  <br/> ||
   

