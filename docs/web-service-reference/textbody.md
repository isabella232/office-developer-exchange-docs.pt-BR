---
title: TextBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bd0c0bce-3e7c-47c7-af7f-5ee5f5ad9820
description: O elemento TextBody Especifica o corpo de texto.
ms.openlocfilehash: 78b18b27891d571605d2eeeeffb5c252cc790c11
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837712"
---
# <a name="textbody"></a><span data-ttu-id="3b104-103">TextBody</span><span class="sxs-lookup"><span data-stu-id="3b104-103">TextBody</span></span>

<span data-ttu-id="3b104-104">O elemento **TextBody** Especifica o corpo de texto.</span><span class="sxs-lookup"><span data-stu-id="3b104-104">The **TextBody** element specifies the text body.</span></span> 
  
```XML
<TextBody BodyTypeType=" HTML | Text" IsTruncated=" true | false"></TextBody>
```

 <span data-ttu-id="3b104-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="3b104-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3b104-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3b104-106">Attributes and elements</span></span>

<span data-ttu-id="3b104-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3b104-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3b104-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3b104-108">Attributes</span></span>

|<span data-ttu-id="3b104-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="3b104-109">**Attribute**</span></span>|<span data-ttu-id="3b104-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3b104-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3b104-111">BodyTypeType</span><span class="sxs-lookup"><span data-stu-id="3b104-111">BodyTypeType</span></span>  <br/> |<span data-ttu-id="3b104-112">Indica o tipo de corpo.</span><span class="sxs-lookup"><span data-stu-id="3b104-112">Indicates the body type.</span></span> <span data-ttu-id="3b104-113">O valor de **texto** para o atributo **BodyTypeType** indica que o corpo está no formato de texto sem formatação.</span><span class="sxs-lookup"><span data-stu-id="3b104-113">The value of **Text** for the **BodyTypeType** attribute indicates that the body is in plain text form.</span></span> <span data-ttu-id="3b104-114">O valor de **HTML** para o atributo **BodyTypeType** indica que o corpo está no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="3b104-114">The value of **HTML** for the **BodyTypeType** attribute indicates that the body is in HTML form.</span></span> <span data-ttu-id="3b104-115">O atributo **BodyTypeType** é necessário.</span><span class="sxs-lookup"><span data-stu-id="3b104-115">The **BodyTypeType** attribute is required.</span></span>  <br/> |
|<span data-ttu-id="3b104-116">IsTruncated</span><span class="sxs-lookup"><span data-stu-id="3b104-116">IsTruncated</span></span>  <br/> |<span data-ttu-id="3b104-117">Indica que o conteúdo do corpo ter sido truncado.</span><span class="sxs-lookup"><span data-stu-id="3b104-117">Indicates that the body contents have been truncated.</span></span> <span data-ttu-id="3b104-118">Um valor de texto de **false** para o atributo **IsTruncated** indica que o corpo de conteúdo não foi truncado.</span><span class="sxs-lookup"><span data-stu-id="3b104-118">A text value of **false** for the **IsTruncated** attribute indicates that the body contents have not been truncated.</span></span> <span data-ttu-id="3b104-119">O corpo normalizado será truncado se o comprimento do corpo de texto for maior que o valor definido no elemento [MaximumBodySize](maximumbodysize.md) .</span><span class="sxs-lookup"><span data-stu-id="3b104-119">The normalized body will be truncated if the text body length is longer than the value set in the [MaximumBodySize](maximumbodysize.md) element.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="3b104-120">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3b104-120">Child elements</span></span>

<span data-ttu-id="3b104-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3b104-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3b104-122">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3b104-122">Parent elements</span></span>

<span data-ttu-id="3b104-123">[Item](item.md) | [contato](contact.md) | [mensagem](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [tarefa](task.md)</span><span class="sxs-lookup"><span data-stu-id="3b104-123">[Item](item.md) | [Contact](contact.md) | [Message](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="3b104-124">Text value</span><span class="sxs-lookup"><span data-stu-id="3b104-124">Text value</span></span>

<span data-ttu-id="3b104-125">O valor de texto do elemento **TextBody** é o corpo de texto do item.</span><span class="sxs-lookup"><span data-stu-id="3b104-125">The text value of the **TextBody** element is the text body of the item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3b104-126">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="3b104-126">Remarks</span></span>

<span data-ttu-id="3b104-127">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3b104-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3b104-128">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3b104-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3b104-129">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3b104-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3b104-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="3b104-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3b104-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3b104-131">Schema name</span></span>  <br/> |<span data-ttu-id="3b104-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3b104-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="3b104-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3b104-133">Validation file</span></span>  <br/> |<span data-ttu-id="3b104-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3b104-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3b104-135">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="3b104-135">Can be empty</span></span>  <br/> ||
   

