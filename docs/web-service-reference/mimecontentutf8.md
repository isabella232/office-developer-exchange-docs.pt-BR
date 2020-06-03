---
title: MimeContentUTF8
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 31544c95-5231-4b57-958c-2a689464d29b
description: O elemento MimeContentUTF8 contém o fluxo de MIME UTF-8 de um objeto que é representado no formato base64Binary e oferece suporte à internacionalização de endereços de email e [RFC6530].
ms.openlocfilehash: a9214bda876c1aadac5b026b3adf38faea8ef17a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530426"
---
# <a name="mimecontentutf8"></a><span data-ttu-id="be702-103">MimeContentUTF8</span><span class="sxs-lookup"><span data-stu-id="be702-103">MimeContentUTF8</span></span>

<span data-ttu-id="be702-104">O elemento **MimeContentUTF8** contém o fluxo de MIME UTF-8 de um objeto que é representado no formato base64Binary e oferece suporte à internacionalização de endereços de email e [[RFC6530]](http://www.rfc-editor.org/rfc/rfc6530.txt).</span><span class="sxs-lookup"><span data-stu-id="be702-104">The **MimeContentUTF8** element contains the UTF-8 MIME stream of an object that is represented in base64Binary format and supports email address internationalization and [[RFC6530]](http://www.rfc-editor.org/rfc/rfc6530.txt).</span></span>
  
```XML
<MimeContentUTF8 CharacterSet="" />
```

 <span data-ttu-id="be702-105">**MimeContentType**</span><span class="sxs-lookup"><span data-stu-id="be702-105">**MimeContentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="be702-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="be702-106">Attributes and elements</span></span>

<span data-ttu-id="be702-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="be702-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="be702-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="be702-108">Attributes</span></span>

|<span data-ttu-id="be702-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="be702-109">**Attribute**</span></span>|<span data-ttu-id="be702-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="be702-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="be702-111">**CharacterSet**</span><span class="sxs-lookup"><span data-stu-id="be702-111">**CharacterSet**</span></span> <br/> |<span data-ttu-id="be702-112">Se definido, o valor desse atributo será ignorado pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="be702-112">If set, the value for this attribute is ignored by the server.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="be702-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="be702-113">Child elements</span></span>

<span data-ttu-id="be702-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="be702-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="be702-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="be702-115">Parent elements</span></span>

<span data-ttu-id="be702-116">[CalendarItem](calendaritem.md)  |  [Contato](contact.md)  |  [DistributionList](distributionlist.md)  |  [Item](item.md)  |  [MeetingCancellation](meetingcancellation.md)  |  [MeetingMessage](meetingmessage.md)  |  [MeetingRequest](meetingrequest.md)  |  [MeetingResponse](meetingresponse.md)  |  [Mensagem](message-ex15websvcsotherref.md)  |  [RemoveItem](removeitem.md)  |  [Tarefa](task.md)</span><span class="sxs-lookup"><span data-stu-id="be702-116">[CalendarItem](calendaritem.md) | [Contact](contact.md) | [DistributionList](distributionlist.md) | [Item](item.md) | [MeetingCancellation](meetingcancellation.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [Message](message-ex15websvcsotherref.md) | [RemoveItem](removeitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="be702-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="be702-117">Text value</span></span>

<span data-ttu-id="be702-118">Um valor de texto que representa um fluxo MIME base64Binary será necessário se esse elemento for usado.</span><span class="sxs-lookup"><span data-stu-id="be702-118">A text value that represents a base64binary MIME stream is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="be702-119">Comentários</span><span class="sxs-lookup"><span data-stu-id="be702-119">Remarks</span></span>

<span data-ttu-id="be702-120">O conteúdo da mensagem passa pelos três níveis de codificação a seguir antes de ser armazenado no valor **MimeContentUTF8** :</span><span class="sxs-lookup"><span data-stu-id="be702-120">The message content goes through the following three levels of encoding before it is stored in the **MimeContentUTF8** value:</span></span> 
  
1. <span data-ttu-id="be702-121">Texto da mensagem – esta é a codificação do corpo, como ISO-2022-JP para caracteres japoneses.</span><span class="sxs-lookup"><span data-stu-id="be702-121">Message text — This is the body encoding, such as iso-2022-jp for Japanese characters.</span></span>
    
2. <span data-ttu-id="be702-122">Fluxo MIME — essa é a codificação UTF8 do texto da mensagem para o elemento **MimeContentUTF8** ou a codificação ASCII do texto da mensagem para o elemento [MimeContent](mimecontent.md) .</span><span class="sxs-lookup"><span data-stu-id="be702-122">MIME stream — This is the UTF8 encoding of the message text for the **MimeContentUTF8** element, or the ASCII encoding of the message text for the [MimeContent](mimecontent.md) element.</span></span> 
    
3. <span data-ttu-id="be702-123">Documento XML — este é sempre o fluxo ASCII codificado em base64 do fluxo MIME, onde caracteres como ' \< ', que são significativos para XML, estão ocultos de analisadores XML.</span><span class="sxs-lookup"><span data-stu-id="be702-123">XML document — This is always the base64-encoded ASCII stream of the MIME stream, where characters such as '\<', which are meaningful to XML, are hidden from XML parsers.</span></span>
    
<span data-ttu-id="be702-124">Cada nível é independente do nível que o precede.</span><span class="sxs-lookup"><span data-stu-id="be702-124">Each level is independent of the level that precedes it.</span></span>
  
<span data-ttu-id="be702-125">O elemento **MimeContentUTF8** pode conter os mesmos dados que outras propriedades retornadas com um item contêm.</span><span class="sxs-lookup"><span data-stu-id="be702-125">The **MimeContentUTF8** element might contain the same data that other properties that are returned with an item contain.</span></span> 
  
<span data-ttu-id="be702-126">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="be702-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="be702-127">Diferenças de versão</span><span class="sxs-lookup"><span data-stu-id="be702-127">Version differences</span></span>

<span data-ttu-id="be702-128">Este elemento está disponível em versões do Exchange a partir do Build 15.00.0986.00.</span><span class="sxs-lookup"><span data-stu-id="be702-128">This element is available in versions of Exchange starting with build 15.00.0986.00.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="be702-129">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="be702-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="be702-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="be702-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="be702-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="be702-131">Schema Name</span></span>  <br/> |<span data-ttu-id="be702-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="be702-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="be702-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="be702-133">Validation File</span></span>  <br/> |<span data-ttu-id="be702-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="be702-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="be702-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="be702-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="be702-136">False</span><span class="sxs-lookup"><span data-stu-id="be702-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="be702-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="be702-137">See also</span></span>



- [<span data-ttu-id="be702-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="be702-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

