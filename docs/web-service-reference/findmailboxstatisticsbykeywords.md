---
title: FindMailboxStatisticsByKeywords
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cfe0f0ff-5fea-4db8-ac96-a5724c85ed2f
description: O elemento FindMailboxStatisticsByKeywords especifica uma solicitação para pesquisar estatísticas de caixa de correio por palavra-chave.
ms.openlocfilehash: e22c7d8dc849d3fd45d6cb158030cbd82119437e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462525"
---
# <a name="findmailboxstatisticsbykeywords"></a><span data-ttu-id="90c4c-103">FindMailboxStatisticsByKeywords</span><span class="sxs-lookup"><span data-stu-id="90c4c-103">FindMailboxStatisticsByKeywords</span></span>

<span data-ttu-id="90c4c-104">O elemento **FindMailboxStatisticsByKeywords** especifica uma solicitação para pesquisar estatísticas de caixa de correio por palavra-chave.</span><span class="sxs-lookup"><span data-stu-id="90c4c-104">The **FindMailboxStatisticsByKeywords** element specifies a request to search for mailbox statistics by keyword.</span></span> 
  
```XML
<FindMailboxStatisticsByKeywords>
    <Mailboxes/>
    <Keywords/>
    <Language/>
    <Senders/>
    <Recipients/>
    <FromDate/>
    <ToDate/>
    <MessageTypes/>
    <SearchDumpster/>
    <IncludePersonalArchive/>
    <IncludeUnsearchableItems/>
</FindMailboxStatisticsByKeywords>
```

 <span data-ttu-id="90c4c-105">**FindMailboxStatisticsByKeywordsType**</span><span class="sxs-lookup"><span data-stu-id="90c4c-105">**FindMailboxStatisticsByKeywordsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="90c4c-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="90c4c-106">Attributes and elements</span></span>

<span data-ttu-id="90c4c-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="90c4c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="90c4c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="90c4c-108">Attributes</span></span>

<span data-ttu-id="90c4c-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="90c4c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="90c4c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="90c4c-110">Child elements</span></span>

|<span data-ttu-id="90c4c-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="90c4c-111">**Element**</span></span>|<span data-ttu-id="90c4c-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="90c4c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="90c4c-113">Caixas de correio (ArrayOfUserMailboxesType)</span><span class="sxs-lookup"><span data-stu-id="90c4c-113">Mailboxes (ArrayOfUserMailboxesType)</span></span>](mailboxes-arrayofusermailboxestype.md) <br/> |<span data-ttu-id="90c4c-114">Contém uma matriz de caixas de correio afetadas pela isenção.</span><span class="sxs-lookup"><span data-stu-id="90c4c-114">Contains an array of mailboxes affected by the hold.</span></span>  <br/> |
|[<span data-ttu-id="90c4c-115">Keywords</span><span class="sxs-lookup"><span data-stu-id="90c4c-115">Keywords</span></span>](keywords-ex15websvcsotherref.md) <br/> |<span data-ttu-id="90c4c-116">Especifica palavras-chave para uma pesquisa.</span><span class="sxs-lookup"><span data-stu-id="90c4c-116">Specifies keywords for a search.</span></span>  <br/> |
|[<span data-ttu-id="90c4c-117">Language</span><span class="sxs-lookup"><span data-stu-id="90c4c-117">Language</span></span>](language.md) <br/> |<span data-ttu-id="90c4c-118">Contém o idioma usado para a consulta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="90c4c-118">Contains the language used for the search query.</span></span>  <br/> |
|[<span data-ttu-id="90c4c-119">Remetentes</span><span class="sxs-lookup"><span data-stu-id="90c4c-119">Senders</span></span>](senders.md) <br/> |<span data-ttu-id="90c4c-120">Especifica uma matriz de endereços SMTP.</span><span class="sxs-lookup"><span data-stu-id="90c4c-120">Specifies an array of SMTP addresses.</span></span>  <br/> |
|[<span data-ttu-id="90c4c-121">Destinatários (ArrayOfSmtpAddressType)</span><span class="sxs-lookup"><span data-stu-id="90c4c-121">Recipients (ArrayOfSmtpAddressType)</span></span>](recipients-arrayofsmtpaddresstype.md) <br/> |<span data-ttu-id="90c4c-122">Especifica uma matriz de destinatários de uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="90c4c-122">Specifies an array of recipients of a message.</span></span>  <br/> |
|[<span data-ttu-id="90c4c-123">FromDate</span><span class="sxs-lookup"><span data-stu-id="90c4c-123">FromDate</span></span>](fromdate.md) <br/> |<span data-ttu-id="90c4c-124">Especifica a data em que a mensagem foi enviada.</span><span class="sxs-lookup"><span data-stu-id="90c4c-124">Specifies the date that the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="90c4c-125">ToDate</span><span class="sxs-lookup"><span data-stu-id="90c4c-125">ToDate</span></span>](todate.md) <br/> |<span data-ttu-id="90c4c-126">Especifica a data em que a mensagem foi recebida.</span><span class="sxs-lookup"><span data-stu-id="90c4c-126">Specifies the date that the message was received.</span></span>  <br/> |
|[<span data-ttu-id="90c4c-127">MessageType</span><span class="sxs-lookup"><span data-stu-id="90c4c-127">MessageTypes</span></span>](messagetypes.md) <br/> |<span data-ttu-id="90c4c-128">Especifica uma matriz de mensagens a serem pesquisadas.</span><span class="sxs-lookup"><span data-stu-id="90c4c-128">Specifies an array of messages to search.</span></span>  <br/> |
|[<span data-ttu-id="90c4c-129">SearchDumpster</span><span class="sxs-lookup"><span data-stu-id="90c4c-129">SearchDumpster</span></span>](searchdumpster.md) <br/> |<span data-ttu-id="90c4c-130">Especifica se pesquisar em itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="90c4c-130">Specifies whether to search in deleted items.</span></span>  <br/> |
|[<span data-ttu-id="90c4c-131">IncludePersonalArchive</span><span class="sxs-lookup"><span data-stu-id="90c4c-131">IncludePersonalArchive</span></span>](includepersonalarchive.md) <br/> |<span data-ttu-id="90c4c-132">Especifica se é para incluir o arquivo morto pessoal na pesquisa.</span><span class="sxs-lookup"><span data-stu-id="90c4c-132">Specifies whether to include the personal archive in the search.</span></span>  <br/> |
|[<span data-ttu-id="90c4c-133">IncludeUnsearchableItems</span><span class="sxs-lookup"><span data-stu-id="90c4c-133">IncludeUnsearchableItems</span></span>](includeunsearchableitems.md) <br/> |<span data-ttu-id="90c4c-134">Especifica se é para incluir itens que não podem ser pesquisados.</span><span class="sxs-lookup"><span data-stu-id="90c4c-134">Specifies whether to include items that cannot be searched.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="90c4c-135">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="90c4c-135">Parent elements</span></span>

<span data-ttu-id="90c4c-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="90c4c-136">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="90c4c-137">Comentários</span><span class="sxs-lookup"><span data-stu-id="90c4c-137">Remarks</span></span>

<span data-ttu-id="90c4c-138">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="90c4c-138">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="90c4c-139">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="90c4c-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="90c4c-140">Namespace</span><span class="sxs-lookup"><span data-stu-id="90c4c-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="90c4c-141">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="90c4c-141">Schema Name</span></span>  <br/> |<span data-ttu-id="90c4c-142">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="90c4c-142">Message schema</span></span>  <br/> |
|<span data-ttu-id="90c4c-143">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="90c4c-143">Validation File</span></span>  <br/> |<span data-ttu-id="90c4c-144">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="90c4c-144">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="90c4c-145">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="90c4c-145">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="90c4c-146">Confira também</span><span class="sxs-lookup"><span data-stu-id="90c4c-146">See also</span></span>



- [<span data-ttu-id="90c4c-147">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="90c4c-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

