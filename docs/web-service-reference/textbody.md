---
title: TextBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bd0c0bce-3e7c-47c7-af7f-5ee5f5ad9820
description: O elemento TextBody especifica o corpo do texto.
ms.openlocfilehash: c0002785fb990a251267218f7a5f232e521db41a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459480"
---
# <a name="textbody"></a><span data-ttu-id="d1fda-103">TextBody</span><span class="sxs-lookup"><span data-stu-id="d1fda-103">TextBody</span></span>

<span data-ttu-id="d1fda-104">O elemento **TextBody** especifica o corpo do texto.</span><span class="sxs-lookup"><span data-stu-id="d1fda-104">The **TextBody** element specifies the text body.</span></span> 
  
```XML
<TextBody BodyTypeType=" HTML | Text" IsTruncated=" true | false"></TextBody>
```

 <span data-ttu-id="d1fda-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="d1fda-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d1fda-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d1fda-106">Attributes and elements</span></span>

<span data-ttu-id="d1fda-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d1fda-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d1fda-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d1fda-108">Attributes</span></span>

|<span data-ttu-id="d1fda-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="d1fda-109">**Attribute**</span></span>|<span data-ttu-id="d1fda-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d1fda-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d1fda-111">BodyTypeType</span><span class="sxs-lookup"><span data-stu-id="d1fda-111">BodyTypeType</span></span>  <br/> |<span data-ttu-id="d1fda-112">Indica o tipo de corpo.</span><span class="sxs-lookup"><span data-stu-id="d1fda-112">Indicates the body type.</span></span> <span data-ttu-id="d1fda-113">O valor de **texto** para o atributo **BodyTypeType** indica que o corpo está no formato de texto sem formatação.</span><span class="sxs-lookup"><span data-stu-id="d1fda-113">The value of **Text** for the **BodyTypeType** attribute indicates that the body is in plain text form.</span></span> <span data-ttu-id="d1fda-114">O valor de **HTML** para o atributo **BodyTypeType** indica que o corpo está no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="d1fda-114">The value of **HTML** for the **BodyTypeType** attribute indicates that the body is in HTML form.</span></span> <span data-ttu-id="d1fda-115">O atributo **BodyTypeType** é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1fda-115">The **BodyTypeType** attribute is required.</span></span>  <br/> |
|<span data-ttu-id="d1fda-116">Istruncado</span><span class="sxs-lookup"><span data-stu-id="d1fda-116">IsTruncated</span></span>  <br/> |<span data-ttu-id="d1fda-117">Indica que o conteúdo do corpo foi truncado.</span><span class="sxs-lookup"><span data-stu-id="d1fda-117">Indicates that the body contents have been truncated.</span></span> <span data-ttu-id="d1fda-118">Um valor de texto **false** para o atributo **IsTruncated** indica que o conteúdo do corpo não foi truncado.</span><span class="sxs-lookup"><span data-stu-id="d1fda-118">A text value of **false** for the **IsTruncated** attribute indicates that the body contents have not been truncated.</span></span> <span data-ttu-id="d1fda-119">O corpo normalizado será truncado se o comprimento do corpo do texto for maior do que o valor definido no elemento [MaximumBodySize](maximumbodysize.md) .</span><span class="sxs-lookup"><span data-stu-id="d1fda-119">The normalized body will be truncated if the text body length is longer than the value set in the [MaximumBodySize](maximumbodysize.md) element.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d1fda-120">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d1fda-120">Child elements</span></span>

<span data-ttu-id="d1fda-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d1fda-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d1fda-122">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d1fda-122">Parent elements</span></span>

<span data-ttu-id="d1fda-123">[Item](item.md)  |  [Contato](contact.md)  |  [Mensagem](message-ex15websvcsotherref.md)  |  [DistributionList](distributionlist.md)  |  [CalendarItem](calendaritem.md)  |  [PostItem](postitem.md)  |  [Tarefa](task.md)</span><span class="sxs-lookup"><span data-stu-id="d1fda-123">[Item](item.md) | [Contact](contact.md) | [Message](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="d1fda-124">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="d1fda-124">Text value</span></span>

<span data-ttu-id="d1fda-125">O valor de texto do elemento **TextBody** é o corpo do texto do item.</span><span class="sxs-lookup"><span data-stu-id="d1fda-125">The text value of the **TextBody** element is the text body of the item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d1fda-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="d1fda-126">Remarks</span></span>

<span data-ttu-id="d1fda-127">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d1fda-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d1fda-128">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d1fda-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d1fda-129">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d1fda-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d1fda-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="d1fda-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d1fda-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d1fda-131">Schema name</span></span>  <br/> |<span data-ttu-id="d1fda-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d1fda-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="d1fda-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d1fda-133">Validation file</span></span>  <br/> |<span data-ttu-id="d1fda-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d1fda-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d1fda-135">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="d1fda-135">Can be empty</span></span>  <br/> ||
   

