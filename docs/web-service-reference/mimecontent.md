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
description: O elemento MimeContent contém o fluxo MIME ASCII de um objeto que é representado no formato base64Binary e suporta [RFC2045].
ms.openlocfilehash: 039ef1245d48e4cf13141970921dd210f4bd7d06
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530433"
---
# <a name="mimecontent"></a><span data-ttu-id="24d4d-103">MimeContent</span><span class="sxs-lookup"><span data-stu-id="24d4d-103">MimeContent</span></span>

<span data-ttu-id="24d4d-104">O elemento **MimeContent** contém o fluxo MIME ASCII de um objeto que é representado no formato base64Binary e suporta [[rfc2045]](http://www.rfc-editor.org/rfc/rfc2045.txt).</span><span class="sxs-lookup"><span data-stu-id="24d4d-104">The **MimeContent** element contains the ASCII MIME stream of an object that is represented in base64Binary format and supports [[RFC2045]](http://www.rfc-editor.org/rfc/rfc2045.txt).</span></span>
  
```xml
<MimeContent CharacterSet="" />
```

 <span data-ttu-id="24d4d-105">**MimeContentType**</span><span class="sxs-lookup"><span data-stu-id="24d4d-105">**MimeContentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="24d4d-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="24d4d-106">Attributes and elements</span></span>

<span data-ttu-id="24d4d-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="24d4d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="24d4d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="24d4d-108">Attributes</span></span>

|<span data-ttu-id="24d4d-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="24d4d-109">**Attribute**</span></span>|<span data-ttu-id="24d4d-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="24d4d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="24d4d-111">**CharacterSet**</span><span class="sxs-lookup"><span data-stu-id="24d4d-111">**CharacterSet**</span></span> <br/> |<span data-ttu-id="24d4d-112">Se definido, o valor desse atributo será ignorado pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="24d4d-112">If set, the value for this attribute is ignored by the server.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="24d4d-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="24d4d-113">Child elements</span></span>

<span data-ttu-id="24d4d-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="24d4d-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="24d4d-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="24d4d-115">Parent elements</span></span>

<span data-ttu-id="24d4d-116">[CalendarItem](calendaritem.md)  |  [Contato](contact.md)  |  [DistributionList](distributionlist.md)  |  [Item](item.md)  |  [MeetingCancellation](meetingcancellation.md)  |  [MeetingMessage](meetingmessage.md)  |  [MeetingRequest](meetingrequest.md)  |  [MeetingResponse](meetingresponse.md)  |  [Mensagem](message-ex15websvcsotherref.md)  |  [RemoveItem](removeitem.md)  |  [Tarefa](task.md)</span><span class="sxs-lookup"><span data-stu-id="24d4d-116">[CalendarItem](calendaritem.md) | [Contact](contact.md) | [DistributionList](distributionlist.md) | [Item](item.md) | [MeetingCancellation](meetingcancellation.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [Message](message-ex15websvcsotherref.md) | [RemoveItem](removeitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="24d4d-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="24d4d-117">Text value</span></span>

<span data-ttu-id="24d4d-118">Um valor de texto que representa um fluxo MIME base64Binary será necessário se esse elemento for usado.</span><span class="sxs-lookup"><span data-stu-id="24d4d-118">A text value that represents a base64Binary MIME stream is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="24d4d-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="24d4d-119">Remarks</span></span>

<span data-ttu-id="24d4d-120">O conteúdo da mensagem passa pelos três níveis de codificação a seguir antes de ser armazenado no valor **MimeContent** :</span><span class="sxs-lookup"><span data-stu-id="24d4d-120">The message content goes through the following three levels of encoding before it is stored in the **MimeContent** value:</span></span> 
  
1. <span data-ttu-id="24d4d-121">Texto da mensagem – esta é a codificação do corpo, como ISO-2022-JP para caracteres japoneses.</span><span class="sxs-lookup"><span data-stu-id="24d4d-121">Message text — This is the body encoding, such as iso-2022-jp for Japanese characters.</span></span>
    
2. <span data-ttu-id="24d4d-122">Fluxo MIME — esta é a codificação ASCII do texto da mensagem para o elemento **MimeContent** ou a codificação UTF8 do texto da mensagem para o elemento [MimeContentUTF8](mimecontentutf8.md) .</span><span class="sxs-lookup"><span data-stu-id="24d4d-122">MIME stream — This is the ASCII encoding of the message text for the **MimeContent** element, or the UTF8 encoding of the message text for the [MimeContentUTF8](mimecontentutf8.md) element.</span></span> 
    
3. <span data-ttu-id="24d4d-123">Documento XML — este é sempre o fluxo ASCII codificado em base64 do fluxo MIME, onde caracteres como ' \< ', que são significativos para XML, estão ocultos de analisadores XML.</span><span class="sxs-lookup"><span data-stu-id="24d4d-123">XML document — This is always the base64-encoded ASCII stream of the MIME stream, where characters such as '\<', which are meaningful to XML, are hidden from XML parsers.</span></span>
    
<span data-ttu-id="24d4d-124">Cada nível é independente do nível que o precede.</span><span class="sxs-lookup"><span data-stu-id="24d4d-124">Each level is independent of the level that precedes it.</span></span>
  
<span data-ttu-id="24d4d-125">O elemento **MimeContent** pode conter os mesmos dados que outras propriedades retornadas com um item contêm.</span><span class="sxs-lookup"><span data-stu-id="24d4d-125">The **MimeContent** element might contain the same data that other properties that are returned with an item contain.</span></span> 
  
<span data-ttu-id="24d4d-126">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="24d4d-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="24d4d-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="24d4d-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="24d4d-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="24d4d-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="24d4d-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="24d4d-129">Schema Name</span></span>  <br/> |<span data-ttu-id="24d4d-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="24d4d-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="24d4d-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="24d4d-131">Validation File</span></span>  <br/> |<span data-ttu-id="24d4d-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="24d4d-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="24d4d-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="24d4d-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="24d4d-134">False</span><span class="sxs-lookup"><span data-stu-id="24d4d-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="24d4d-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="24d4d-135">See also</span></span>



- [<span data-ttu-id="24d4d-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="24d4d-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

