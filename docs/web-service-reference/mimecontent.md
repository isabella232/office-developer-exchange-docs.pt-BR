---
title: MimeContent
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MimeContent
api_type:
- schema
ms.assetid: 4f472a08-5653-4c54-ba65-831dfe32f20f
description: O elemento MimeContent contém o fluxo de MIME ASCII de um objeto que é representado no formato base64Binary e suporta [RFC2045].
ms.openlocfilehash: 60f2d42f09347611559137c494d93036f1192829
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824465"
---
# <a name="mimecontent"></a><span data-ttu-id="781f4-103">MimeContent</span><span class="sxs-lookup"><span data-stu-id="781f4-103">MimeContent</span></span>

<span data-ttu-id="781f4-104">O elemento **MimeContent** contém o fluxo de MIME ASCII de um objeto que é representado no formato base64Binary e suporta [[RFC2045]](http://www.rfc-editor.org/rfc/rfc2045.txt).</span><span class="sxs-lookup"><span data-stu-id="781f4-104">The **MimeContent** element contains the ASCII MIME stream of an object that is represented in base64Binary format and supports [[RFC2045]](http://www.rfc-editor.org/rfc/rfc2045.txt).</span></span>
  
```xml
<MimeContent CharacterSet="" />
```

 <span data-ttu-id="781f4-105">**MimeContentType**</span><span class="sxs-lookup"><span data-stu-id="781f4-105">**MimeContentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="781f4-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="781f4-106">Attributes and elements</span></span>

<span data-ttu-id="781f4-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="781f4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="781f4-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="781f4-108">Attributes</span></span>

|<span data-ttu-id="781f4-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="781f4-109">**Attribute**</span></span>|<span data-ttu-id="781f4-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="781f4-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="781f4-111">**CharacterSet**</span><span class="sxs-lookup"><span data-stu-id="781f4-111">**CharacterSet**</span></span> <br/> |<span data-ttu-id="781f4-112">Se definido, o valor para este atributo é ignorado pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="781f4-112">If set, the value for this attribute is ignored by the server.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="781f4-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="781f4-113">Child elements</span></span>

<span data-ttu-id="781f4-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="781f4-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="781f4-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="781f4-115">Parent elements</span></span>

<span data-ttu-id="781f4-116">[CalendarItem](calendaritem.md) | [contato](contact.md) | [DistributionList](distributionlist.md) | [Item](item.md) | [MeetingCancellation](meetingcancellation.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md)  |  [ MeetingResponse](meetingresponse.md) | [mensagem](message-ex15websvcsotherref.md) | [RemoveItem](removeitem.md) | [tarefa](task.md)</span><span class="sxs-lookup"><span data-stu-id="781f4-116">[CalendarItem](calendaritem.md) | [Contact](contact.md) | [DistributionList](distributionlist.md) | [Item](item.md) | [MeetingCancellation](meetingcancellation.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [Message](message-ex15websvcsotherref.md) | [RemoveItem](removeitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="781f4-117">Text value</span><span class="sxs-lookup"><span data-stu-id="781f4-117">Text value</span></span>

<span data-ttu-id="781f4-118">Se este elemento for usado, será necessário um valor de texto que representa um fluxo MIME base64Binary.</span><span class="sxs-lookup"><span data-stu-id="781f4-118">A text value that represents a base64Binary MIME stream is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="781f4-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="781f4-119">Remarks</span></span>

<span data-ttu-id="781f4-120">O conteúdo da mensagem passa três níveis de codificação antes de ser armazenado no valor de **MimeContent** a seguir:</span><span class="sxs-lookup"><span data-stu-id="781f4-120">The message content goes through the following three levels of encoding before it is stored in the **MimeContent** value:</span></span> 
  
1. <span data-ttu-id="781f4-121">Texto da mensagem — este é o corpo de codificação, como iso-2022-jp para caracteres japonês.</span><span class="sxs-lookup"><span data-stu-id="781f4-121">Message text — This is the body encoding, such as iso-2022-jp for Japanese characters.</span></span>
    
2. <span data-ttu-id="781f4-122">Fluxo de MIME — isto é a codificação ASCII do texto da mensagem para o elemento **MimeContent** ou a codificação UTF8 do texto da mensagem para o elemento [MimeContentUTF8](mimecontentutf8.md) .</span><span class="sxs-lookup"><span data-stu-id="781f4-122">MIME stream — This is the ASCII encoding of the message text for the **MimeContent** element, or the UTF8 encoding of the message text for the [MimeContentUTF8](mimecontentutf8.md) element.</span></span> 
    
3. <span data-ttu-id="781f4-123">Documento XML — será sempre o fluxo de ASCII codificado na base64 do fluxo de MIME, onde caracteres como '\<', que sejam significativas XML, estão ocultos analisadores XML.</span><span class="sxs-lookup"><span data-stu-id="781f4-123">XML document — This is always the base64-encoded ASCII stream of the MIME stream, where characters such as '\<', which are meaningful to XML, are hidden from XML parsers.</span></span>
    
<span data-ttu-id="781f4-124">Cada nível é independente do nível que precede a ele.</span><span class="sxs-lookup"><span data-stu-id="781f4-124">Each level is independent of the level that precedes it.</span></span>
  
<span data-ttu-id="781f4-125">O elemento **MimeContent** deve conter os mesmos dados que contêm outras propriedades que são retornadas com um item.</span><span class="sxs-lookup"><span data-stu-id="781f4-125">The **MimeContent** element might contain the same data that other properties that are returned with an item contain.</span></span> 
  
<span data-ttu-id="781f4-126">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="781f4-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="781f4-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="781f4-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="781f4-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="781f4-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="781f4-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="781f4-129">Schema Name</span></span>  <br/> |<span data-ttu-id="781f4-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="781f4-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="781f4-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="781f4-131">Validation File</span></span>  <br/> |<span data-ttu-id="781f4-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="781f4-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="781f4-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="781f4-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="781f4-134">False</span><span class="sxs-lookup"><span data-stu-id="781f4-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="781f4-135">Ver também</span><span class="sxs-lookup"><span data-stu-id="781f4-135">See also</span></span>



- [<span data-ttu-id="781f4-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="781f4-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

