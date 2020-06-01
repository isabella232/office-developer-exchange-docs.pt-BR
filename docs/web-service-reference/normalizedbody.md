---
title: NormalizedBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bfb813e4-642d-4f1b-9e91-1fee89dbd083
description: O elemento NormalizedBody especifica uma representação HTML da Propriedade Body de um item como um fragmento que pode ser inserido em outro corpo HTML.
ms.openlocfilehash: fb249794bccfeed198e7a3230ab53c66893dcf96
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462665"
---
# <a name="normalizedbody"></a><span data-ttu-id="b599b-103">NormalizedBody</span><span class="sxs-lookup"><span data-stu-id="b599b-103">NormalizedBody</span></span>

<span data-ttu-id="b599b-104">O elemento **NormalizedBody** especifica uma representação HTML da propriedade **Body** de um item como um fragmento que pode ser inserido em outro corpo HTML.</span><span class="sxs-lookup"><span data-stu-id="b599b-104">The **NormalizedBody** element specifies an HTML representation of the **Body** property of an item as a fragment that can be inserted into another HTML body.</span></span> 
  
```XML
<NormalizedBody BodyType="Text | HTML" IsTruncated="true | false"></NormalizedBody>
```

 <span data-ttu-id="b599b-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="b599b-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b599b-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b599b-106">Attributes and elements</span></span>

<span data-ttu-id="b599b-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b599b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b599b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b599b-108">Attributes</span></span>

|<span data-ttu-id="b599b-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="b599b-109">**Attribute**</span></span>|<span data-ttu-id="b599b-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b599b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b599b-111">BodyType</span><span class="sxs-lookup"><span data-stu-id="b599b-111">BodyType</span></span>  <br/> |<span data-ttu-id="b599b-112">Indica o tipo de corpo.</span><span class="sxs-lookup"><span data-stu-id="b599b-112">Indicates the body type.</span></span> <span data-ttu-id="b599b-113">O valor de **texto** para o atributo **BodyType** indica que o corpo está no formato de texto sem formatação.</span><span class="sxs-lookup"><span data-stu-id="b599b-113">The value of **Text** for the **BodyType** attribute indicates that the body is in plain text form.</span></span> <span data-ttu-id="b599b-114">O valor de **HTML** para o atributo **BodyType** indica que o corpo está no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="b599b-114">The value of **HTML** for the **BodyType** attribute indicates that the body is in HTML form.</span></span> <span data-ttu-id="b599b-115">O atributo **BodyType** é necessário.</span><span class="sxs-lookup"><span data-stu-id="b599b-115">The **BodyType** attribute is required.</span></span>  <br/> |
|<span data-ttu-id="b599b-116">Istruncado</span><span class="sxs-lookup"><span data-stu-id="b599b-116">IsTruncated</span></span>  <br/> |<span data-ttu-id="b599b-117">Indica que o conteúdo do corpo foi truncado.</span><span class="sxs-lookup"><span data-stu-id="b599b-117">Indicates that the body contents have been truncated.</span></span> <span data-ttu-id="b599b-118">Um valor de texto **false** para o atributo **IsTruncated** indica que o conteúdo do corpo não foi truncado.</span><span class="sxs-lookup"><span data-stu-id="b599b-118">A text value of **false** for the **IsTruncated** attribute indicates that the body contents have not been truncated.</span></span> <span data-ttu-id="b599b-119">O corpo normalizado será truncado se o tamanho do corpo normalizado for maior do que o valor definido no elemento [MaximumBodySize](maximumbodysize.md) .</span><span class="sxs-lookup"><span data-stu-id="b599b-119">The normalized body will be truncated if the normalized body length is longer than the value set in the [MaximumBodySize](maximumbodysize.md) element.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b599b-120">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b599b-120">Child elements</span></span>

<span data-ttu-id="b599b-121">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b599b-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b599b-122">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b599b-122">Parent elements</span></span>

<span data-ttu-id="b599b-123">[Item](item.md)  |  [Mensagem](message-ex15websvcsotherref.md)  |  [MeetingMessage](meetingmessage.md)  |  [MeetingRequest](meetingrequest.md)  |  [MeetingResponse](meetingresponse.md)  |  [MeetingCancellation](meetingcancellation.md)  |  [Tarefa](task.md)  |  [PostItem](postitem.md)  |  [CalendarItem](calendaritem.md)  |  [Contato](contact.md)  |  [DistributionList](distributionlist.md)</span><span class="sxs-lookup"><span data-stu-id="b599b-123">[Item](item.md) | [Message](message-ex15websvcsotherref.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [Task](task.md) | [PostItem](postitem.md) | [CalendarItem](calendaritem.md) | [Contact](contact.md) | [DistributionList](distributionlist.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="b599b-124">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="b599b-124">Text value</span></span>

<span data-ttu-id="b599b-125">O valor de texto do elemento **NormalizedBody** é o corpo normalizado do item.</span><span class="sxs-lookup"><span data-stu-id="b599b-125">The text value of the **NormalizedBody** element is the normalized body of the item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b599b-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="b599b-126">Remarks</span></span>

<span data-ttu-id="b599b-127">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b599b-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b599b-128">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b599b-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b599b-129">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="b599b-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b599b-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="b599b-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b599b-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b599b-131">Schema name</span></span>  <br/> |<span data-ttu-id="b599b-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b599b-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="b599b-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b599b-133">Validation file</span></span>  <br/> |<span data-ttu-id="b599b-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b599b-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b599b-135">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="b599b-135">Can be empty</span></span>  <br/> ||
   

