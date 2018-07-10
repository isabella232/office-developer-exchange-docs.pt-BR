---
title: InternetMessageHeader
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InternetMessageHeader
api_type:
- schema
ms.assetid: c70675f8-6feb-4c89-ba48-bce0479b308b
description: O elemento InternetMessageHeader representa o cabeçalho da mensagem para um determinado cabeçalho dentro da coleção de cabeçalhos da Internet. Para obter toda a coleção de cabeçalhos de mensagem da Internet, use a propriedade PR_TRANSPORT_MESSAGE_HEADERS. Para obter mais informações sobre os cabeçalhos de mensagem do EWS e a Internet, seeGetting cabeçalhos de mensagens da Internet no EWS, MIME e os cabeçalhos das mensagens de Internet ausentes.
ms.openlocfilehash: 9457cdabe99c0adcb8183cbc039cc86db881fec7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823952"
---
# <a name="internetmessageheader"></a><span data-ttu-id="a427f-105">InternetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="a427f-105">InternetMessageHeader</span></span>

<span data-ttu-id="a427f-106">O elemento **InternetMessageHeader** representa o cabeçalho da mensagem para um determinado cabeçalho dentro da coleção de cabeçalhos da Internet.</span><span class="sxs-lookup"><span data-stu-id="a427f-106">The **InternetMessageHeader** element represents the Internet message header for a given header within the headers collection.</span></span> <span data-ttu-id="a427f-107">Para obter toda a coleção de cabeçalhos de mensagem da Internet, use a propriedade **PR_TRANSPORT_MESSAGE_HEADERS** .</span><span class="sxs-lookup"><span data-stu-id="a427f-107">To get the entire collection of Internet message headers, use the **PR_TRANSPORT_MESSAGE_HEADERS** property.</span></span> <span data-ttu-id="a427f-108">Para obter mais informações sobre cabeçalhos de mensagem do EWS e a Internet, consulte "Getting Internet cabeçalhos das mensagens no [EWS, MIME e os cabeçalhos das mensagens de Internet ausentes](http://msdn.microsoft.com/pt-br/library/exchange/hh545614%28v=exchg.140%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="a427f-108">For more information about EWS and Internet message headers, see "Getting Internet message headers in [EWS, MIME, and the missing Internet message headers](http://msdn.microsoft.com/pt-br/library/exchange/hh545614%28v=exchg.140%29.aspx).</span></span>
  
```XML
<InternetMessageHeader HeaderName=""/>
```

 <span data-ttu-id="a427f-109">**InternetHeaderType**</span><span class="sxs-lookup"><span data-stu-id="a427f-109">**InternetHeaderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a427f-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a427f-110">Attributes and elements</span></span>

<span data-ttu-id="a427f-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a427f-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a427f-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="a427f-112">Attributes</span></span>

|<span data-ttu-id="a427f-113">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="a427f-113">**Attribute**</span></span>|<span data-ttu-id="a427f-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a427f-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a427f-115">**HeaderName**</span><span class="sxs-lookup"><span data-stu-id="a427f-115">**HeaderName**</span></span> <br/> |<span data-ttu-id="a427f-116">Identifica o nome de cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="a427f-116">Identifies the header name.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a427f-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a427f-117">Child elements</span></span>

<span data-ttu-id="a427f-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a427f-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a427f-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a427f-119">Parent elements</span></span>

|<span data-ttu-id="a427f-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a427f-120">**Element**</span></span>|<span data-ttu-id="a427f-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a427f-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a427f-122">InternetMessageHeaders</span><span class="sxs-lookup"><span data-stu-id="a427f-122">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="a427f-123">Representa a coleção de todos os cabeçalhos de mensagem da Internet que estão contidos em um item em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="a427f-123">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a427f-124">Text value</span><span class="sxs-lookup"><span data-stu-id="a427f-124">Text value</span></span>

<span data-ttu-id="a427f-125">O valor de texto representa o valor para o cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="a427f-125">The text value represents the value for the header.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a427f-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="a427f-126">Remarks</span></span>

<span data-ttu-id="a427f-127">Apresentamos a seguir o EWS Managed API estendido a definição de propriedade para a propriedade **PR_TRANSPORT_MESSAGE_HEADERS** .</span><span class="sxs-lookup"><span data-stu-id="a427f-127">The following is the EWS Managed API extended property definition for the **PR_TRANSPORT_MESSAGE_HEADERS** property.</span></span> 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

<span data-ttu-id="a427f-128">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a427f-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a427f-129">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a427f-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a427f-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="a427f-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a427f-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a427f-131">Schema Name</span></span>  <br/> |<span data-ttu-id="a427f-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a427f-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="a427f-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a427f-133">Validation File</span></span>  <br/> |<span data-ttu-id="a427f-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a427f-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a427f-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a427f-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="a427f-136">False</span><span class="sxs-lookup"><span data-stu-id="a427f-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a427f-137">Ver também</span><span class="sxs-lookup"><span data-stu-id="a427f-137">See also</span></span>



- [<span data-ttu-id="a427f-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a427f-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="a427f-139">EWS, MIME e os cabeçalhos das mensagens de Internet ausentes</span><span class="sxs-lookup"><span data-stu-id="a427f-139">EWS, MIME, and the missing Internet message headers</span></span>](http://msdn.microsoft.com/pt-br/library/exchange/hh545614%28v=exchg.140%29.aspx)

