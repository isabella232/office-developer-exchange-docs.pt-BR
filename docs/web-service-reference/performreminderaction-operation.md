---
title: Operação PerformReminderAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c597bb0e-13b0-422e-9c23-970463e2a5c3
description: Encontre informações sobre a operação do EWS do PerformReminderAction.
ms.openlocfilehash: 4c069d541e9a42167c447a50c405399958d3608d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462287"
---
# <a name="performreminderaction-operation"></a><span data-ttu-id="190ae-103">Operação PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="190ae-103">PerformReminderAction operation</span></span>

<span data-ttu-id="190ae-104">Encontre informações sobre a operação do EWS do **PerformReminderAction** .</span><span class="sxs-lookup"><span data-stu-id="190ae-104">Find information about the **PerformReminderAction** EWS operation.</span></span> 
  
<span data-ttu-id="190ae-105">A operação do **PerformReminderAction** do serviços Web do Exchange (EWS) inicia uma ação de ignorar ou adiar em um lembrete.</span><span class="sxs-lookup"><span data-stu-id="190ae-105">The **PerformReminderAction** Exchange Web Services (EWS) operation initiates a dismiss or snooze action on a reminder.</span></span> 
  
<span data-ttu-id="190ae-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="190ae-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-performreminderaction-operation"></a><span data-ttu-id="190ae-107">Usando a operação PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="190ae-107">Using the PerformReminderAction operation</span></span>

<span data-ttu-id="190ae-108">Você pode usar a operação **PerformReminderAction** para descartar ou adiar (atrasar) lembretes retornados pela operação [getlembretes](getreminders-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="190ae-108">You can use the **PerformReminderAction** operation to dismiss or snooze (delay) reminders returned by the [GetReminders](getreminders-operation.md) operation.</span></span> <span data-ttu-id="190ae-109">Para adiar um lembrete, defina [ActionType](actiontype-reminderactiontype.md) como **adiar**e defina o valor de [NewReminderTime](newremindertime.md) para uma hora posterior ao [lembrete](remindertime.md)atual, caso contrário, o **NewReminderTime** será ignorado pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="190ae-109">To snooze a reminder, set the [ActionType](actiontype-reminderactiontype.md) to **Snooze**, and set the [NewReminderTime](newremindertime.md) value to a time later than the current [ReminderTime](remindertime.md), otherwise the **NewReminderTime** is ignored by the server.</span></span> <span data-ttu-id="190ae-110">Se o lembrete for para uma ocorrência de uma reunião recorrente, e a ação **adiar** for tomada no lembrete com um **NewReminderTime** que ultrapasse o lembrete da próxima ocorrência, o lembrete será efetivamente ignorado.</span><span class="sxs-lookup"><span data-stu-id="190ae-110">If the reminder is for an occurrence of a recurring meeting, and the **Snooze** action is taken on the reminder with a **NewReminderTime** that is past the reminder of the next occurrence, the reminder is effectively dismissed.</span></span> 
  
<span data-ttu-id="190ae-111">Para descartar um lembrete, defina **ActionType** como **dismiss**.</span><span class="sxs-lookup"><span data-stu-id="190ae-111">To dismiss a reminder, set the **ActionType** to **Dismiss**.</span></span> <span data-ttu-id="190ae-112">Quando o servidor processa a solicitação, o servidor altera o valor [ReminderSet](isreminderset.md) para o item de **true** para **false**.</span><span class="sxs-lookup"><span data-stu-id="190ae-112">When the server processes the request, the server changes the [IsReminderSet](isreminderset.md) value for the item from **True** to **False**.</span></span>
  
### <a name="performreminderaction-operation-soap-headers"></a><span data-ttu-id="190ae-113">Cabeçalhos SOAP de operação PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="190ae-113">PerformReminderAction operation SOAP headers</span></span>

<span data-ttu-id="190ae-114">A operação **PerformReminderAction** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="190ae-114">The **PerformReminderAction** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="190ae-115">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="190ae-115">**Header name**</span></span>|<span data-ttu-id="190ae-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="190ae-116">**Element**</span></span>|<span data-ttu-id="190ae-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="190ae-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="190ae-118">**Representação**</span><span class="sxs-lookup"><span data-stu-id="190ae-118">**Impersonation**</span></span> <br/> |[<span data-ttu-id="190ae-119">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="190ae-119">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="190ae-120">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="190ae-120">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="190ae-121">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="190ae-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="190ae-122">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="190ae-122">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="190ae-123">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="190ae-123">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="190ae-124">Identifica a cultura, conforme definido na RFC 3066, "marcas de identificação de idiomas", a ser usado para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="190ae-124">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="190ae-125">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="190ae-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="190ae-126">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="190ae-126">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="190ae-127">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="190ae-127">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="190ae-128">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="190ae-128">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="190ae-129">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="190ae-129">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="190ae-130">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="190ae-130">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="190ae-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="190ae-131">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="190ae-132">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="190ae-132">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="190ae-133">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="190ae-133">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="performreminderaction-operation-request-example"></a><span data-ttu-id="190ae-134">Exemplo de solicitação de operação PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="190ae-134">PerformReminderAction operation request example</span></span>

<span data-ttu-id="190ae-135">O exemplo a seguir de uma solicitação de operação do **PerformReminderAction** mostra como adiar um lembrete atual e definir um novo horário de lembrete.</span><span class="sxs-lookup"><span data-stu-id="190ae-135">The following example of a **PerformReminderAction** operation request shows how to snooze a current reminder and set a new reminder time.</span></span> <span data-ttu-id="190ae-136">Observe que você precisa incluir o **ChangeKey** para o [ItemId](itemid.md) e o **NewReminderTime** deve ser definido como uma hora depois do **ReminderTime** retornado pela operação [getlembrers](getreminders-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="190ae-136">Note that you need to include the **ChangeKey** for the [ItemId](itemid.md) and the **NewReminderTime** must be set to a time later than the **ReminderTime** returned by the [GetReminders](getreminders-operation.md) operation.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
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
> <span data-ttu-id="190ae-137">O valor de **ItemId** foi reduzido para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="190ae-137">The **ItemId** value has been shortened to preserve readability.</span></span> 
  
<span data-ttu-id="190ae-138">O corpo SOAP de solicitação contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="190ae-138">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="190ae-139">PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="190ae-139">PerformReminderAction</span></span>](performreminderaction.md)
    
- [<span data-ttu-id="190ae-140">ReminderItemActions</span><span class="sxs-lookup"><span data-stu-id="190ae-140">ReminderItemActions</span></span>](reminderitemactions.md)
    
- [<span data-ttu-id="190ae-141">ReminderItemAction</span><span class="sxs-lookup"><span data-stu-id="190ae-141">ReminderItemAction</span></span>](reminderitemaction.md)
    
- [<span data-ttu-id="190ae-142">ActionType</span><span class="sxs-lookup"><span data-stu-id="190ae-142">ActionType</span></span>](actiontype-reminderactiontype.md)
    
- [<span data-ttu-id="190ae-143">ItemId</span><span class="sxs-lookup"><span data-stu-id="190ae-143">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="190ae-144">NewReminderTime</span><span class="sxs-lookup"><span data-stu-id="190ae-144">NewReminderTime</span></span>](newremindertime.md)
    
## <a name="successful-performreminderaction-operation-response"></a><span data-ttu-id="190ae-145">Resposta de operação PerformReminderAction bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="190ae-145">Successful PerformReminderAction operation response</span></span>

<span data-ttu-id="190ae-146">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **PerformReminderAction** .</span><span class="sxs-lookup"><span data-stu-id="190ae-146">The following example shows a successful response to a **PerformReminderAction** operation request.</span></span> <span data-ttu-id="190ae-147">O elemento **UpdatedItemIds** contém os **ItemIds** do item de calendário atualizado.</span><span class="sxs-lookup"><span data-stu-id="190ae-147">The **UpdatedItemIds** element contains the **ItemIds** of the updated calendar item.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="921"
                       MinorBuildNumber="20"
                       Version="V2_10"
                       xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <PerformReminderActionResponse ResponseClass="Success"
                                   xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <UpdatedItemIds>
        <ItemId Id="vwAAAA=="
                ChangeKey="DwAAABYAAAB4to43JyybTYwHLBM1k8MxAAAJKP+S"/>
      </UpdatedItemIds>
    </PerformReminderActionResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="190ae-148">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="190ae-148">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="190ae-149">PerformReminderActionResponse</span><span class="sxs-lookup"><span data-stu-id="190ae-149">PerformReminderActionResponse</span></span>](performreminderactionresponse.md)
    
- [<span data-ttu-id="190ae-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="190ae-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="190ae-151">UpdatedItemIds</span><span class="sxs-lookup"><span data-stu-id="190ae-151">UpdatedItemIds</span></span>](updateditemids.md)
    
- [<span data-ttu-id="190ae-152">ItemId</span><span class="sxs-lookup"><span data-stu-id="190ae-152">ItemId</span></span>](itemid.md)
    
## <a name="performreminderaction-operation-error-response-example"></a><span data-ttu-id="190ae-153">Exemplo de resposta de erro de operação PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="190ae-153">PerformReminderAction operation error response example</span></span>

<span data-ttu-id="190ae-154">O exemplo a seguir mostra uma resposta a uma solicitação de operação **PerformReminderAction** quando nenhuma alteração foi feita no servidor.</span><span class="sxs-lookup"><span data-stu-id="190ae-154">The following example shows a response to a **PerformReminderAction** operation request when no change was made on the server.</span></span> <span data-ttu-id="190ae-155">Esta é uma resposta na qual uma solicitação foi enviada, mas nenhum **UpdatedItemIds** foi retornado, o que significa que nenhum lembrete foi alterado.</span><span class="sxs-lookup"><span data-stu-id="190ae-155">This is a response in which a request was sent, but no **UpdatedItemIds** were returned, meaning no reminders were changed.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="7"
                       Version="V2_10"
                       xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <PerformReminderActionResponse ResponseClass="Success"
                                   xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <UpdatedItemIds />
    </PerformReminderActionResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="190ae-156">O corpo SOAP de resposta de erro contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="190ae-156">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="190ae-157">PerformReminderActionResponse</span><span class="sxs-lookup"><span data-stu-id="190ae-157">PerformReminderActionResponse</span></span>](performreminderactionresponse.md)
    
- [<span data-ttu-id="190ae-158">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="190ae-158">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="190ae-159">UpdatedItemIds</span><span class="sxs-lookup"><span data-stu-id="190ae-159">UpdatedItemIds</span></span>](updateditemids.md)
    
<span data-ttu-id="190ae-160">Para obter códigos de erro adicionais genéricos para o EWS, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="190ae-160">For additional error codes that are generic to EWS, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="190ae-161">Também consulte</span><span class="sxs-lookup"><span data-stu-id="190ae-161">See also</span></span>


- [<span data-ttu-id="190ae-162">Operação getlembretes</span><span class="sxs-lookup"><span data-stu-id="190ae-162">GetReminders operation</span></span>](getreminders-operation.md)
    

