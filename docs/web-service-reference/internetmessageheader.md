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
description: O elemento InternetMessageHeader representa o cabeçalho da mensagem da Internet para um determinado cabeçalho dentro da coleção Headers. Para obter a coleção inteira de cabeçalhos de mensagens da Internet, use a propriedade PR_TRANSPORT_MESSAGE_HEADERS. Para obter mais informações sobre os cabeçalhos de mensagem EWS e Internet, Consulteobter cabeçalhos de mensagem da Internet no EWS, MIME e os cabeçalhos de mensagem da Internet ausentes.
ms.openlocfilehash: 7b662617e0b1a1fcdcce3449b729485ba6e0956b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459304"
---
# <a name="internetmessageheader"></a><span data-ttu-id="5276c-105">InternetMessageHeader</span><span class="sxs-lookup"><span data-stu-id="5276c-105">InternetMessageHeader</span></span>

<span data-ttu-id="5276c-106">O elemento **InternetMessageHeader** representa o cabeçalho da mensagem da Internet para um determinado cabeçalho dentro da coleção Headers.</span><span class="sxs-lookup"><span data-stu-id="5276c-106">The **InternetMessageHeader** element represents the Internet message header for a given header within the headers collection.</span></span> <span data-ttu-id="5276c-107">Para obter a coleção inteira de cabeçalhos de mensagens da Internet, use a propriedade **PR_TRANSPORT_MESSAGE_HEADERS** .</span><span class="sxs-lookup"><span data-stu-id="5276c-107">To get the entire collection of Internet message headers, use the **PR_TRANSPORT_MESSAGE_HEADERS** property.</span></span> <span data-ttu-id="5276c-108">Para obter mais informações sobre o EWS e cabeçalhos de mensagens da Internet, consulte "obtendo cabeçalhos de mensagens da Internet em [EWS, MIME e cabeçalhos de mensagem da Internet ausentes](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="5276c-108">For more information about EWS and Internet message headers, see "Getting Internet message headers in [EWS, MIME, and the missing Internet message headers](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx).</span></span>
  
```XML
<InternetMessageHeader HeaderName=""/>
```

 <span data-ttu-id="5276c-109">**InternetHeaderType**</span><span class="sxs-lookup"><span data-stu-id="5276c-109">**InternetHeaderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5276c-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5276c-110">Attributes and elements</span></span>

<span data-ttu-id="5276c-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5276c-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5276c-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="5276c-112">Attributes</span></span>

|<span data-ttu-id="5276c-113">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="5276c-113">**Attribute**</span></span>|<span data-ttu-id="5276c-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5276c-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5276c-115">**HeaderName**</span><span class="sxs-lookup"><span data-stu-id="5276c-115">**HeaderName**</span></span> <br/> |<span data-ttu-id="5276c-116">Identifica o nome do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="5276c-116">Identifies the header name.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="5276c-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5276c-117">Child elements</span></span>

<span data-ttu-id="5276c-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5276c-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5276c-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5276c-119">Parent elements</span></span>

|<span data-ttu-id="5276c-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5276c-120">**Element**</span></span>|<span data-ttu-id="5276c-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5276c-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5276c-122">Propriedadeinternetmessageheaders</span><span class="sxs-lookup"><span data-stu-id="5276c-122">InternetMessageHeaders</span></span>](internetmessageheaders.md) <br/> |<span data-ttu-id="5276c-123">Representa a coleção de todos os cabeçalhos de mensagens da Internet contidos em um item em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="5276c-123">Represents the collection of all Internet message headers that are contained in an item in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5276c-124">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="5276c-124">Text value</span></span>

<span data-ttu-id="5276c-125">O valor de texto representa o valor do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="5276c-125">The text value represents the value for the header.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5276c-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="5276c-126">Remarks</span></span>

<span data-ttu-id="5276c-127">A seguir está a definição da propriedade estendida da API gerenciada do EWS para a propriedade **PR_TRANSPORT_MESSAGE_HEADERS** .</span><span class="sxs-lookup"><span data-stu-id="5276c-127">The following is the EWS Managed API extended property definition for the **PR_TRANSPORT_MESSAGE_HEADERS** property.</span></span> 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

<span data-ttu-id="5276c-128">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5276c-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5276c-129">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="5276c-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5276c-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="5276c-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5276c-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5276c-131">Schema Name</span></span>  <br/> |<span data-ttu-id="5276c-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="5276c-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="5276c-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5276c-133">Validation File</span></span>  <br/> |<span data-ttu-id="5276c-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5276c-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5276c-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5276c-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="5276c-136">False</span><span class="sxs-lookup"><span data-stu-id="5276c-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5276c-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="5276c-137">See also</span></span>



- [<span data-ttu-id="5276c-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5276c-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="5276c-139">EWS, MIME e os cabeçalhos de mensagem da Internet ausentes</span><span class="sxs-lookup"><span data-stu-id="5276c-139">EWS, MIME, and the missing Internet message headers</span></span>](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx)

