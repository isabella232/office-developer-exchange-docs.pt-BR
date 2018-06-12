---
title: Operação GetItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItem
api_type:
- schema
ms.assetid: e3590b8b-c2a7-4dad-a014-6360197b68e4
description: Encontre informações sobre o EWS GetItem operação.
ms.openlocfilehash: 9b63032b2eaa3bf26027a42e38bfa06bedcbac86
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752544"
---
# <a name="getitem-operation"></a><span data-ttu-id="0d885-103">Operação GetItem</span><span class="sxs-lookup"><span data-stu-id="0d885-103">GetItem operation</span></span>

<span data-ttu-id="0d885-104">Encontre informações sobre a operação de EWS **GetItem** .</span><span class="sxs-lookup"><span data-stu-id="0d885-104">Find information about the **GetItem** EWS operation.</span></span> 
  
<span data-ttu-id="0d885-105">A operação **GetItem** obtém os itens do armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0d885-105">The **GetItem** operation gets items from the Exchange store.</span></span> 
  
## <a name="using-the-getitem-operation"></a><span data-ttu-id="0d885-106">Usando a operação GetItem</span><span class="sxs-lookup"><span data-stu-id="0d885-106">Using the GetItem operation</span></span>

<span data-ttu-id="0d885-107">A operação de **GetItem** retorna propriedades de item de muitos.</span><span class="sxs-lookup"><span data-stu-id="0d885-107">The **GetItem** operation returns many item properties.</span></span> <span data-ttu-id="0d885-108">As propriedades que são retornadas em uma resposta **GetItem** variam com base na forma solicitada, propriedades adicionais solicitadas e o tipo de item os dados retornados.</span><span class="sxs-lookup"><span data-stu-id="0d885-108">The properties that are returned in a **GetItem** response vary based on the requested shape, requested additional properties, and the type of item returned.</span></span> 
  
<span data-ttu-id="0d885-109">Elementos de [mensagem](message-ex15websvcsotherref.md) representam as mensagens de email e outros itens que não são fortemente tipados pelo esquema dos serviços Web do Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="0d885-109">[Message](message-ex15websvcsotherref.md) elements represent email messages and all other items that are not strongly typed by the Exchange Web Services (EWS) schema.</span></span> <span data-ttu-id="0d885-110">Itens como IPM. Compartilhamento e IPM.InfoPath são retornados como elementos da [mensagem](message-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="0d885-110">Items such as IPM.Sharing and IPM.InfoPath are returned as [Message](message-ex15websvcsotherref.md) elements.</span></span> <span data-ttu-id="0d885-111">Exchange não retorna o elemento do [Item](item.md) base nas respostas.</span><span class="sxs-lookup"><span data-stu-id="0d885-111">Exchange does not return the base [Item](item.md) element in responses.</span></span> 
  
<span data-ttu-id="0d885-112">A operação **GetItem** não retorna anexos.</span><span class="sxs-lookup"><span data-stu-id="0d885-112">The **GetItem** operation does not return attachments.</span></span> <span data-ttu-id="0d885-113">Ela retornar metadados sobre um item anexado ou o arquivo.</span><span class="sxs-lookup"><span data-stu-id="0d885-113">It does return metadata about an attached item or file.</span></span> <span data-ttu-id="0d885-114">Para retornar um anexo, use a [operação GetAttachment](getattachment-operation.md).</span><span class="sxs-lookup"><span data-stu-id="0d885-114">To return an attachment, use the [GetAttachment operation](getattachment-operation.md).</span></span>
  
## <a name="getitem-operation-soap-headers"></a><span data-ttu-id="0d885-115">Cabeçalhos SOAP GetItem operação</span><span class="sxs-lookup"><span data-stu-id="0d885-115">GetItem operation SOAP headers</span></span>

<span data-ttu-id="0d885-116">A operação **GetItem** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="0d885-116">The **GetItem** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="0d885-117">Cabeçalho \* \* \*</span><span class="sxs-lookup"><span data-stu-id="0d885-117">****Header****</span></span>|<span data-ttu-id="0d885-118">****Element****</span><span class="sxs-lookup"><span data-stu-id="0d885-118">****Element****</span></span>|<span data-ttu-id="0d885-119">****Descrição****</span><span class="sxs-lookup"><span data-stu-id="0d885-119">****Description****</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="0d885-120">**DateTimePrecision**</span><span class="sxs-lookup"><span data-stu-id="0d885-120">**DateTimePrecision**</span></span> <br/> |[<span data-ttu-id="0d885-121">DateTimePrecision</span><span class="sxs-lookup"><span data-stu-id="0d885-121">DateTimePrecision</span></span>](datetimeprecision.md) <br/> |<span data-ttu-id="0d885-122">Especifica a resolução dos valores de data/hora nas respostas do servidor, em segundos ou em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="0d885-122">Specifies the resolution of data/time values in responses from the server, either in seconds or in milliseconds.</span></span>  <br/> |
|<span data-ttu-id="0d885-123">**Representação**</span><span class="sxs-lookup"><span data-stu-id="0d885-123">**Impersonation**</span></span> <br/> |[<span data-ttu-id="0d885-124">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="0d885-124">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="0d885-125">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="0d885-125">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="0d885-126">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="0d885-126">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="0d885-127">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="0d885-127">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="0d885-128">Identifica a cultura, conforme definido no RFC 3066, "Marcas para a identificação de idiomas", que será usada para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="0d885-128">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="0d885-129">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="0d885-129">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="0d885-130">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="0d885-130">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="0d885-131">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="0d885-131">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="0d885-132">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="0d885-132">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="0d885-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="0d885-133">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="0d885-134">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="0d885-134">Identifies the version of the server that responded to the request.</span></span>  <br/> |
|<span data-ttu-id="0d885-135">**TimeZoneContext**</span><span class="sxs-lookup"><span data-stu-id="0d885-135">**TimeZoneContext**</span></span> <br/> |[<span data-ttu-id="0d885-136">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="0d885-136">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="0d885-137">Identifica o fuso horário a ser usado para todas as respostas do servidor.</span><span class="sxs-lookup"><span data-stu-id="0d885-137">Identifies the time zone to be used for all responses from the server.</span></span>  <br/> |
   
## <a name="in-this-section"></a><span data-ttu-id="0d885-138">Nesta Seção</span><span class="sxs-lookup"><span data-stu-id="0d885-138">In This Section</span></span>

[<span data-ttu-id="0d885-139">Operação GetItem (mensagem de email)</span><span class="sxs-lookup"><span data-stu-id="0d885-139">GetItem operation (email message)</span></span>](getitem-operation-email-message.md)
  
[<span data-ttu-id="0d885-140">Operação GetItem (item de calendário)</span><span class="sxs-lookup"><span data-stu-id="0d885-140">GetItem operation (calendar item)</span></span>](getitem-operation-calendar-item.md)
  
[<span data-ttu-id="0d885-141">Operação GetItem (tarefa)</span><span class="sxs-lookup"><span data-stu-id="0d885-141">GetItem operation (task)</span></span>](getitem-operation-task.md)
  
[<span data-ttu-id="0d885-142">Operação GetItem (contato)</span><span class="sxs-lookup"><span data-stu-id="0d885-142">GetItem operation (contact)</span></span>](getitem-operation-contact.md)
  
## <a name="see-also"></a><span data-ttu-id="0d885-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="0d885-143">See also</span></span>



[<span data-ttu-id="0d885-144">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="0d885-144">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

