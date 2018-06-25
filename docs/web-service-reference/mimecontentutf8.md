---
title: MimeContentUTF8
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 31544c95-5231-4b57-958c-2a689464d29b
description: O elemento MimeContentUTF8 contém o fluxo de MIME de codificação UTF-8 de um objeto que é representado no formato base64Binary e suporta internacionalização de endereço de email e [RFC6530].
ms.openlocfilehash: 47599b6634738fd488e5b020f69e36d5fcf550a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824466"
---
# <a name="mimecontentutf8"></a><span data-ttu-id="5caa0-103">MimeContentUTF8</span><span class="sxs-lookup"><span data-stu-id="5caa0-103">MimeContentUTF8</span></span>

<span data-ttu-id="5caa0-104">O elemento **MimeContentUTF8** contém o fluxo de MIME de codificação UTF-8 de um objeto que é representado no formato base64Binary e suporta internacionalização de endereço de email e [[RFC6530]](http://www.rfc-editor.org/rfc/rfc6530.txt).</span><span class="sxs-lookup"><span data-stu-id="5caa0-104">The **MimeContentUTF8** element contains the UTF-8 MIME stream of an object that is represented in base64Binary format and supports email address internationalization and [[RFC6530]](http://www.rfc-editor.org/rfc/rfc6530.txt).</span></span>
  
```XML
<MimeContentUTF8 CharacterSet="" />
```

 <span data-ttu-id="5caa0-105">**MimeContentType**</span><span class="sxs-lookup"><span data-stu-id="5caa0-105">**MimeContentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5caa0-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="5caa0-106">Attributes and elements</span></span>

<span data-ttu-id="5caa0-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5caa0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5caa0-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5caa0-108">Attributes</span></span>

|<span data-ttu-id="5caa0-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="5caa0-109">**Attribute**</span></span>|<span data-ttu-id="5caa0-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5caa0-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5caa0-111">**CharacterSet**</span><span class="sxs-lookup"><span data-stu-id="5caa0-111">**CharacterSet**</span></span> <br/> |<span data-ttu-id="5caa0-112">Se definido, o valor para este atributo é ignorado pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="5caa0-112">If set, the value for this attribute is ignored by the server.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="5caa0-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5caa0-113">Child elements</span></span>

<span data-ttu-id="5caa0-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5caa0-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5caa0-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5caa0-115">Parent elements</span></span>

<span data-ttu-id="5caa0-116">[CalendarItem](calendaritem.md) | [contato](contact.md) | [DistributionList](distributionlist.md) | [Item](item.md) | [MeetingCancellation](meetingcancellation.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md)  |  [ MeetingResponse](meetingresponse.md) | [mensagem](message-ex15websvcsotherref.md) | [RemoveItem](removeitem.md) | [tarefa](task.md)</span><span class="sxs-lookup"><span data-stu-id="5caa0-116">[CalendarItem](calendaritem.md) | [Contact](contact.md) | [DistributionList](distributionlist.md) | [Item](item.md) | [MeetingCancellation](meetingcancellation.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [Message](message-ex15websvcsotherref.md) | [RemoveItem](removeitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="5caa0-117">Text value</span><span class="sxs-lookup"><span data-stu-id="5caa0-117">Text value</span></span>

<span data-ttu-id="5caa0-118">Se este elemento for usado, será necessário um valor de texto que representa um fluxo MIME base64binary.</span><span class="sxs-lookup"><span data-stu-id="5caa0-118">A text value that represents a base64binary MIME stream is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5caa0-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="5caa0-119">Remarks</span></span>

<span data-ttu-id="5caa0-120">O conteúdo da mensagem passa três níveis de codificação antes de ser armazenado no valor de **MimeContentUTF8** a seguir:</span><span class="sxs-lookup"><span data-stu-id="5caa0-120">The message content goes through the following three levels of encoding before it is stored in the **MimeContentUTF8** value:</span></span> 
  
1. <span data-ttu-id="5caa0-121">Texto da mensagem — este é o corpo de codificação, como iso-2022-jp para caracteres japonês.</span><span class="sxs-lookup"><span data-stu-id="5caa0-121">Message text — This is the body encoding, such as iso-2022-jp for Japanese characters.</span></span>
    
2. <span data-ttu-id="5caa0-122">Fluxo de MIME — isto é a codificação UTF8 do texto da mensagem para o elemento **MimeContentUTF8** ou a codificação ASCII do texto da mensagem para o elemento [MimeContent](mimecontent.md) .</span><span class="sxs-lookup"><span data-stu-id="5caa0-122">MIME stream — This is the UTF8 encoding of the message text for the **MimeContentUTF8** element, or the ASCII encoding of the message text for the [MimeContent](mimecontent.md) element.</span></span> 
    
3. <span data-ttu-id="5caa0-123">Documento XML — será sempre o fluxo de ASCII codificado na base64 do fluxo de MIME, onde caracteres como '\<', que sejam significativas XML, estão ocultos analisadores XML.</span><span class="sxs-lookup"><span data-stu-id="5caa0-123">XML document — This is always the base64-encoded ASCII stream of the MIME stream, where characters such as '\<', which are meaningful to XML, are hidden from XML parsers.</span></span>
    
<span data-ttu-id="5caa0-124">Cada nível é independente do nível que precede a ele.</span><span class="sxs-lookup"><span data-stu-id="5caa0-124">Each level is independent of the level that precedes it.</span></span>
  
<span data-ttu-id="5caa0-125">O elemento **MimeContentUTF8** deve conter os mesmos dados que contêm outras propriedades que são retornadas com um item.</span><span class="sxs-lookup"><span data-stu-id="5caa0-125">The **MimeContentUTF8** element might contain the same data that other properties that are returned with an item contain.</span></span> 
  
<span data-ttu-id="5caa0-126">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5caa0-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="5caa0-127">Diferenças de versão</span><span class="sxs-lookup"><span data-stu-id="5caa0-127">Version differences</span></span>

<span data-ttu-id="5caa0-128">Este elemento está disponível nas versões do Exchange, começando com compilação 15.00.0986.00.</span><span class="sxs-lookup"><span data-stu-id="5caa0-128">This element is available in versions of Exchange starting with build 15.00.0986.00.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5caa0-129">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="5caa0-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5caa0-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="5caa0-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5caa0-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5caa0-131">Schema Name</span></span>  <br/> |<span data-ttu-id="5caa0-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="5caa0-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="5caa0-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5caa0-133">Validation File</span></span>  <br/> |<span data-ttu-id="5caa0-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5caa0-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5caa0-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5caa0-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="5caa0-136">False</span><span class="sxs-lookup"><span data-stu-id="5caa0-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5caa0-137">Ver também</span><span class="sxs-lookup"><span data-stu-id="5caa0-137">See also</span></span>



- [<span data-ttu-id="5caa0-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5caa0-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

