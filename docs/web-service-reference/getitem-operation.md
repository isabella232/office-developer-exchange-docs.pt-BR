---
title: Operação GetItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- GetItem
api_type:
- schema
ms.assetid: e3590b8b-c2a7-4dad-a014-6360197b68e4
description: Encontre informações sobre a operação do EWS do GetItem.
localization_priority: Priority
ms.openlocfilehash: 8871dde183974454fc27dbddda489e6b0a70f3aa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463325"
---
# <a name="getitem-operation"></a><span data-ttu-id="c1c39-103">Operação GetItem</span><span class="sxs-lookup"><span data-stu-id="c1c39-103">GetItem operation</span></span>

<span data-ttu-id="c1c39-104">Encontre informações sobre a operação do EWS do **GetItem** .</span><span class="sxs-lookup"><span data-stu-id="c1c39-104">Find information about the **GetItem** EWS operation.</span></span> 
  
<span data-ttu-id="c1c39-105">A operação **GetItem** Obtém itens do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c1c39-105">The **GetItem** operation gets items from the Exchange store.</span></span> 
  
## <a name="using-the-getitem-operation"></a><span data-ttu-id="c1c39-106">Usando a operação GetItem</span><span class="sxs-lookup"><span data-stu-id="c1c39-106">Using the GetItem operation</span></span>

<span data-ttu-id="c1c39-107">A operação **GetItem** retorna muitas propriedades de item.</span><span class="sxs-lookup"><span data-stu-id="c1c39-107">The **GetItem** operation returns many item properties.</span></span> <span data-ttu-id="c1c39-108">As propriedades que são retornadas em uma resposta **GetItem** variam de acordo com a forma solicitada, as propriedades adicionais solicitadas e o tipo de item retornado.</span><span class="sxs-lookup"><span data-stu-id="c1c39-108">The properties that are returned in a **GetItem** response vary based on the requested shape, requested additional properties, and the type of item returned.</span></span> 
  
<span data-ttu-id="c1c39-109">Os elementos da [mensagem](message-ex15websvcsotherref.md) representam mensagens de email e todos os outros itens que não são digitados com rigidez pelo esquema dos serviços Web do Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="c1c39-109">[Message](message-ex15websvcsotherref.md) elements represent email messages and all other items that are not strongly typed by the Exchange Web Services (EWS) schema.</span></span> <span data-ttu-id="c1c39-110">Itens como IPM. O compartilhamento e o IPM. InfoPath são retornados como elementos de [mensagem](message-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="c1c39-110">Items such as IPM.Sharing and IPM.InfoPath are returned as [Message](message-ex15websvcsotherref.md) elements.</span></span> <span data-ttu-id="c1c39-111">O Exchange não retorna o elemento de [Item](item.md) base em respostas.</span><span class="sxs-lookup"><span data-stu-id="c1c39-111">Exchange does not return the base [Item](item.md) element in responses.</span></span> 
  
<span data-ttu-id="c1c39-112">A operação **GetItem** não retorna anexos.</span><span class="sxs-lookup"><span data-stu-id="c1c39-112">The **GetItem** operation does not return attachments.</span></span> <span data-ttu-id="c1c39-113">Ele retorna metadados sobre um item ou arquivo anexado.</span><span class="sxs-lookup"><span data-stu-id="c1c39-113">It does return metadata about an attached item or file.</span></span> <span data-ttu-id="c1c39-114">Para retornar um anexo, use a [operação GetAttachment](getattachment-operation.md).</span><span class="sxs-lookup"><span data-stu-id="c1c39-114">To return an attachment, use the [GetAttachment operation](getattachment-operation.md).</span></span>
  
## <a name="getitem-operation-soap-headers"></a><span data-ttu-id="c1c39-115">Cabeçalhos SOAP de operação GetItem</span><span class="sxs-lookup"><span data-stu-id="c1c39-115">GetItem operation SOAP headers</span></span>

<span data-ttu-id="c1c39-116">A operação **GetItem** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="c1c39-116">The **GetItem** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="c1c39-117">Header \* \* \* \*</span><span class="sxs-lookup"><span data-stu-id="c1c39-117">\*\*\*\*Header\*\*\*\*</span></span>|<span data-ttu-id="c1c39-118">\*\*\*\*Element\*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="c1c39-118">\*\*\*\*Element\*\*\*\*</span></span>|<span data-ttu-id="c1c39-119">\*\*\*\*Descrição\*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="c1c39-119">\*\*\*\*Description\*\*\*\*</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="c1c39-120">**DateTimePrecision**</span><span class="sxs-lookup"><span data-stu-id="c1c39-120">**DateTimePrecision**</span></span> <br/> |[<span data-ttu-id="c1c39-121">DateTimePrecision</span><span class="sxs-lookup"><span data-stu-id="c1c39-121">DateTimePrecision</span></span>](datetimeprecision.md) <br/> |<span data-ttu-id="c1c39-122">Especifica a resolução de valores de data/hora em respostas do servidor, em segundos ou em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="c1c39-122">Specifies the resolution of data/time values in responses from the server, either in seconds or in milliseconds.</span></span>  <br/> |
|<span data-ttu-id="c1c39-123">**Representação**</span><span class="sxs-lookup"><span data-stu-id="c1c39-123">**Impersonation**</span></span> <br/> |[<span data-ttu-id="c1c39-124">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="c1c39-124">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="c1c39-125">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="c1c39-125">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="c1c39-126">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="c1c39-126">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="c1c39-127">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="c1c39-127">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="c1c39-128">Identifica a cultura, conforme definido na RFC 3066, "marcas de identificação de idiomas", a ser usado para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c1c39-128">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="c1c39-129">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="c1c39-129">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="c1c39-130">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="c1c39-130">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="c1c39-131">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="c1c39-131">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="c1c39-132">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="c1c39-132">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="c1c39-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c1c39-133">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="c1c39-134">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="c1c39-134">Identifies the version of the server that responded to the request.</span></span>  <br/> |
|<span data-ttu-id="c1c39-135">**TimeZoneContext**</span><span class="sxs-lookup"><span data-stu-id="c1c39-135">**TimeZoneContext**</span></span> <br/> |[<span data-ttu-id="c1c39-136">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="c1c39-136">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="c1c39-137">Identifica o fuso horário a ser usado para todas as respostas do servidor.</span><span class="sxs-lookup"><span data-stu-id="c1c39-137">Identifies the time zone to be used for all responses from the server.</span></span>  <br/> |
   
## <a name="in-this-section"></a><span data-ttu-id="c1c39-138">Nesta seção</span><span class="sxs-lookup"><span data-stu-id="c1c39-138">In This Section</span></span>

[<span data-ttu-id="c1c39-139">Operação GetItem (mensagem de email)</span><span class="sxs-lookup"><span data-stu-id="c1c39-139">GetItem operation (email message)</span></span>](getitem-operation-email-message.md)
  
[<span data-ttu-id="c1c39-140">Operação GetItem (item de calendário)</span><span class="sxs-lookup"><span data-stu-id="c1c39-140">GetItem operation (calendar item)</span></span>](getitem-operation-calendar-item.md)
  
[<span data-ttu-id="c1c39-141">Operação GetItem (tarefa)</span><span class="sxs-lookup"><span data-stu-id="c1c39-141">GetItem operation (task)</span></span>](getitem-operation-task.md)
  
[<span data-ttu-id="c1c39-142">Operação GetItem (contato)</span><span class="sxs-lookup"><span data-stu-id="c1c39-142">GetItem operation (contact)</span></span>](getitem-operation-contact.md)
  
## <a name="see-also"></a><span data-ttu-id="c1c39-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="c1c39-143">See also</span></span>



[<span data-ttu-id="c1c39-144">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="c1c39-144">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

