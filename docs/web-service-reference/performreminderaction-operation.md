---
title: Operação PerformReminderAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c597bb0e-13b0-422e-9c23-970463e2a5c3
description: Encontre informações sobre o EWS PerformReminderAction operação.
ms.openlocfilehash: 778fbb508413721f58cfcf9143a5296874e6cd1c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824722"
---
# <a name="performreminderaction-operation"></a><span data-ttu-id="b2cb6-103">Operação PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="b2cb6-103">PerformReminderAction operation</span></span>

<span data-ttu-id="b2cb6-104">Encontre informações sobre a operação de EWS **PerformReminderAction** .</span><span class="sxs-lookup"><span data-stu-id="b2cb6-104">Find information about the **PerformReminderAction** EWS operation.</span></span> 
  
<span data-ttu-id="b2cb6-105">A operação de serviços Web do Exchange (EWS) **PerformReminderAction** inicia uma ação dismiss ou adiar sobre um lembrete.</span><span class="sxs-lookup"><span data-stu-id="b2cb6-105">The **PerformReminderAction** Exchange Web Services (EWS) operation initiates a dismiss or snooze action on a reminder.</span></span> 
  
<span data-ttu-id="b2cb6-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b2cb6-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-performreminderaction-operation"></a><span data-ttu-id="b2cb6-107">Usando a operação PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="b2cb6-107">Using the PerformReminderAction operation</span></span>

<span data-ttu-id="b2cb6-108">Você pode usar a operação **PerformReminderAction** para descartar ou snooze lembretes (atraso) retornados pela operação de [GetReminders](getreminders-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="b2cb6-108">You can use the **PerformReminderAction** operation to dismiss or snooze (delay) reminders returned by the [GetReminders](getreminders-operation.md) operation.</span></span> <span data-ttu-id="b2cb6-109">Para adiar um lembrete, defina o [ActionType](actiontype-reminderactiontype.md) como **Snooze**e definir o valor de [NewReminderTime](newremindertime.md) até um momento posterior à atual [ReminderTime](remindertime.md), caso contrário, o **NewReminderTime** será ignorado pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="b2cb6-109">To snooze a reminder, set the [ActionType](actiontype-reminderactiontype.md) to **Snooze**, and set the [NewReminderTime](newremindertime.md) value to a time later than the current [ReminderTime](remindertime.md), otherwise the **NewReminderTime** is ignored by the server.</span></span> <span data-ttu-id="b2cb6-110">Se o lembrete for para uma ocorrência de uma reunião recorrente, e a ação de **Snooze** será executada o lembrete com **NewReminderTime** passar o lembrete da próxima ocorrência, o lembrete efetivamente é descartado.</span><span class="sxs-lookup"><span data-stu-id="b2cb6-110">If the reminder is for an occurrence of a recurring meeting, and the **Snooze** action is taken on the reminder with a **NewReminderTime** that is past the reminder of the next occurrence, the reminder is effectively dismissed.</span></span> 
  
<span data-ttu-id="b2cb6-111">Para descartar um lembrete, defina o **ActionType** como **Dismiss**.</span><span class="sxs-lookup"><span data-stu-id="b2cb6-111">To dismiss a reminder, set the **ActionType** to **Dismiss**.</span></span> <span data-ttu-id="b2cb6-112">Quando o servidor processa a solicitação, o servidor altera o valor de [IsReminderSet](isreminderset.md) para o item de **True** para **False**.</span><span class="sxs-lookup"><span data-stu-id="b2cb6-112">When the server processes the request, the server changes the [IsReminderSet](isreminderset.md) value for the item from **True** to **False**.</span></span>
  
### <a name="performreminderaction-operation-soap-headers"></a><span data-ttu-id="b2cb6-113">Cabeçalhos SOAP PerformReminderAction operação</span><span class="sxs-lookup"><span data-stu-id="b2cb6-113">PerformReminderAction operation SOAP headers</span></span>

<span data-ttu-id="b2cb6-114">A operação **PerformReminderAction** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="b2cb6-114">The **PerformReminderAction** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="b2cb6-115">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="b2cb6-115">**Header name**</span></span>|<span data-ttu-id="b2cb6-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b2cb6-116">**Element**</span></span>|<span data-ttu-id="b2cb6-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b2cb6-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b2cb6-118">**Representação**</span><span class="sxs-lookup"><span data-stu-id="b2cb6-118">**Impersonation**</span></span> <br/> |[<span data-ttu-id="b2cb6-119">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="b2cb6-119">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="b2cb6-120">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="b2cb6-120">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="b2cb6-121">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2cb6-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="b2cb6-122">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="b2cb6-122">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="b2cb6-123">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="b2cb6-123">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="b2cb6-124">Identifica a cultura, conforme definido no RFC 3066, "Marcas para a identificação de idiomas", que será usada para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b2cb6-124">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="b2cb6-125">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2cb6-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="b2cb6-126">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="b2cb6-126">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="b2cb6-127">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="b2cb6-127">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="b2cb6-128">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="b2cb6-128">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="b2cb6-129">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2cb6-129">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="b2cb6-130">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="b2cb6-130">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="b2cb6-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="b2cb6-131">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="b2cb6-132">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="b2cb6-132">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="b2cb6-133">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="b2cb6-133">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="performreminderaction-operation-request-example"></a><span data-ttu-id="b2cb6-134">Exemplo de solicitação de operação PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="b2cb6-134">PerformReminderAction operation request example</span></span>

<span data-ttu-id="b2cb6-135">O exemplo a seguir de uma solicitação de operação **PerformReminderAction** mostra como snooze um lembrete atual e definir um novo horário do lembrete.</span><span class="sxs-lookup"><span data-stu-id="b2cb6-135">The following example of a **PerformReminderAction** operation request shows how to snooze a current reminder and set a new reminder time.</span></span> <span data-ttu-id="b2cb6-136">Observe que você precisa incluir o **ChangeKey** para o [ItemId](itemid.md) e o **NewReminderTime** deve ser definida para um horário mais recente do que o **ReminderTime** retornados pela operação de [GetReminders](getreminders-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="b2cb6-136">Note that you need to include the **ChangeKey** for the [ItemId](itemid.md) and the **NewReminderTime** must be set to a time later than the **ReminderTime** returned by the [GetReminders](getreminders-operation.md) operation.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:PerformReminderAction>
      <m:ReminderItemActions>
        <t:ReminderItemAction>
          <t:ActionType>Snooze</t:ActionType>
          <t:ItemId Id="vwAAAA=="
           ChangeKey="DwAAABQAAACOs0HEMq1WTKpI7sNu5qXNAAAUDA=="/>
          <t:NewReminderTime>2014-04-16T17:00:00Z</t:NewReminderTime>
        </t:ReminderItemAction>
      </m:ReminderItemActions>
    </m:PerformReminderAction>
  </soap:Body>
</soap:Envelope>
```

> [!NOTE]
> <span data-ttu-id="b2cb6-137">O valor de **ItemId** foi reduzido para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b2cb6-137">The **ItemId** value has been shortened to preserve readability.</span></span> 
  
<span data-ttu-id="b2cb6-138">A solicitação de corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="b2cb6-138">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="b2cb6-139">PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="b2cb6-139">PerformReminderAction</span></span>](performreminderaction.md)
    
- [<span data-ttu-id="b2cb6-140">ReminderItemActions</span><span class="sxs-lookup"><span data-stu-id="b2cb6-140">ReminderItemActions</span></span>](reminderitemactions.md)
    
- [<span data-ttu-id="b2cb6-141">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="b2cb6-141">ReminderItemAction</span></span>](reminderitemaction.md)
    
- [<span data-ttu-id="b2cb6-142">ActionType</span><span class="sxs-lookup"><span data-stu-id="b2cb6-142">ActionType</span></span>](actiontype-reminderactiontype.md)
    
- [<span data-ttu-id="b2cb6-143">ItemId</span><span class="sxs-lookup"><span data-stu-id="b2cb6-143">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="b2cb6-144">NewReminderTime</span><span class="sxs-lookup"><span data-stu-id="b2cb6-144">NewReminderTime</span></span>](newremindertime.md)
    
## <a name="successful-performreminderaction-operation-response"></a><span data-ttu-id="b2cb6-145">Resposta de operação PerformReminderAction bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="b2cb6-145">Successful PerformReminderAction operation response</span></span>

<span data-ttu-id="b2cb6-146">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **PerformReminderAction** .</span><span class="sxs-lookup"><span data-stu-id="b2cb6-146">The following example shows a successful response to a **PerformReminderAction** operation request.</span></span> <span data-ttu-id="b2cb6-147">O elemento **UpdatedItemIds** contém o **ItemIds** do item de calendário atualizados.</span><span class="sxs-lookup"><span data-stu-id="b2cb6-147">The **UpdatedItemIds** element contains the **ItemIds** of the updated calendar item.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="921"
                       MinorBuildNumber="20"
                       Version="V2_10"
                       xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <PerformReminderActionResponse ResponseClass="Success"
                                   xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <UpdatedItemIds>
        <ItemId Id="vwAAAA=="
                ChangeKey="DwAAABYAAAB4to43JyybTYwHLBM1k8MxAAAJKP+S"/>
      </UpdatedItemIds>
    </PerformReminderActionResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="b2cb6-148">A resposta SOAP body contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="b2cb6-148">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="b2cb6-149">PerformReminderActionResponse</span><span class="sxs-lookup"><span data-stu-id="b2cb6-149">PerformReminderActionResponse</span></span>](performreminderactionresponse.md)
    
- [<span data-ttu-id="b2cb6-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b2cb6-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b2cb6-151">UpdatedItemIds</span><span class="sxs-lookup"><span data-stu-id="b2cb6-151">UpdatedItemIds</span></span>](updateditemids.md)
    
- [<span data-ttu-id="b2cb6-152">ItemId</span><span class="sxs-lookup"><span data-stu-id="b2cb6-152">ItemId</span></span>](itemid.md)
    
## <a name="performreminderaction-operation-error-response-example"></a><span data-ttu-id="b2cb6-153">Exemplo de resposta de erro de operação PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="b2cb6-153">PerformReminderAction operation error response example</span></span>

<span data-ttu-id="b2cb6-154">O exemplo a seguir mostra uma resposta a uma solicitação de operação **PerformReminderAction** quando nenhuma alteração foi feita no servidor.</span><span class="sxs-lookup"><span data-stu-id="b2cb6-154">The following example shows a response to a **PerformReminderAction** operation request when no change was made on the server.</span></span> <span data-ttu-id="b2cb6-155">Esta é uma resposta na qual uma solicitação foi enviada, mas nenhum **UpdatedItemIds** foram retornados, que significa que nenhum lembretes foram alteradas.</span><span class="sxs-lookup"><span data-stu-id="b2cb6-155">This is a response in which a request was sent, but no **UpdatedItemIds** were returned, meaning no reminders were changed.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="7"
                       Version="V2_10"
                       xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <PerformReminderActionResponse ResponseClass="Success"
                                   xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <UpdatedItemIds />
    </PerformReminderActionResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="b2cb6-156">A resposta de erro corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="b2cb6-156">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="b2cb6-157">PerformReminderActionResponse</span><span class="sxs-lookup"><span data-stu-id="b2cb6-157">PerformReminderActionResponse</span></span>](performreminderactionresponse.md)
    
- [<span data-ttu-id="b2cb6-158">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b2cb6-158">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b2cb6-159">UpdatedItemIds</span><span class="sxs-lookup"><span data-stu-id="b2cb6-159">UpdatedItemIds</span></span>](updateditemids.md)
    
<span data-ttu-id="b2cb6-160">Para códigos de erro adicionais que são genéricos para o EWS, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="b2cb6-160">For additional error codes that are generic to EWS, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="b2cb6-161">Confira também</span><span class="sxs-lookup"><span data-stu-id="b2cb6-161">See also</span></span>


- [<span data-ttu-id="b2cb6-162">Operação GetReminders</span><span class="sxs-lookup"><span data-stu-id="b2cb6-162">GetReminders operation</span></span>](getreminders-operation.md)
    

