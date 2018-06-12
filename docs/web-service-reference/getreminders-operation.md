---
title: Operação GetReminders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1b56f83f-3b87-4b55-8259-fde6692da681
description: Encontre informações sobre o EWS GetReminders operação.
ms.openlocfilehash: 803dabf51b94dbd8fb01f2709a42ff59a597bfd1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752611"
---
# <a name="getreminders-operation"></a><span data-ttu-id="5f55e-103">Operação GetReminders</span><span class="sxs-lookup"><span data-stu-id="5f55e-103">GetReminders operation</span></span>

<span data-ttu-id="5f55e-104">Encontre informações sobre a operação de EWS **GetReminders** .</span><span class="sxs-lookup"><span data-stu-id="5f55e-104">Find information about the **GetReminders** EWS operation.</span></span> 
  
<span data-ttu-id="5f55e-105">A operação de serviços Web do Exchange (EWS) **GetReminders** recupera lembretes para itens de calendário e tarefas.</span><span class="sxs-lookup"><span data-stu-id="5f55e-105">The **GetReminders** Exchange Web Services (EWS) operation retrieves reminders for calendar and task items.</span></span> 
  
<span data-ttu-id="5f55e-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5f55e-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getreminders-operation"></a><span data-ttu-id="5f55e-107">Usando a operação GetReminders</span><span class="sxs-lookup"><span data-stu-id="5f55e-107">Using the GetReminders operation</span></span>

<span data-ttu-id="5f55e-108">A operação **GetReminders** obtém lembretes de calendário atual e futuro e itens de tarefa na caixa de correio do usuário, dependendo dos valores do elemento passado na solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f55e-108">The **GetReminders** operation gets reminders for current and future calendar and task items in the user's mailbox, depending on the element values passed in the request.</span></span> <span data-ttu-id="5f55e-109">A operação pode recuperar todos os itens de calendário atuais e futuros, bem como tarefas que possuem um lembrete definido.</span><span class="sxs-lookup"><span data-stu-id="5f55e-109">The operation can retrieve all current and future calendar items as well as tasks that have a reminder set.</span></span> <span data-ttu-id="5f55e-110">Itens de calendário particular são incluídos nas respostas.</span><span class="sxs-lookup"><span data-stu-id="5f55e-110">Private calendar items are included in responses.</span></span> <span data-ttu-id="5f55e-111">Tarefas sem lembretes não são incluídas nas respostas, nem são emails com lembretes ou sinalizadores de acompanhamento.</span><span class="sxs-lookup"><span data-stu-id="5f55e-111">Tasks without reminders are not included in responses, nor are emails with reminders or follow up flags.</span></span> 
  
<span data-ttu-id="5f55e-112">Para recuperar todos os lembretes atuais, recomendamos a configuração do [ReminderType](remindertype.md) para **todos** e o [EndTime](endtime-remindermessagedatatype.md) para a hora atual.</span><span class="sxs-lookup"><span data-stu-id="5f55e-112">To retrieve all current reminders, we recommend setting the [ReminderType](remindertype.md) to **All** and the [EndTime](endtime-remindermessagedatatype.md) to the current time.</span></span> 
  
<span data-ttu-id="5f55e-113">Se os elementos [BeginTime](begintime.md) e **EndTime** estão incluídos na solicitação, a resposta inclui os lembretes para qualquer calendário e itens de tarefa que ocorrem entre tiverem um lembrete que ocorre entre o **BeginTime** e **EndTime**.</span><span class="sxs-lookup"><span data-stu-id="5f55e-113">If the [BeginTime](begintime.md) and **EndTime** elements are included in the request, the response includes reminders for any calendar and task items that occur between have a reminder that occurs between the **BeginTime** and **EndTime**.</span></span>
  
<span data-ttu-id="5f55e-114">A tabela a seguir descreve o comportamento do elemento **ReminderType** quando os elementos **BeginTime** e **EndTime** são incluídos.</span><span class="sxs-lookup"><span data-stu-id="5f55e-114">The following table describes the behavior of the **ReminderType** element when the **BeginTime** and **EndTime** elements are included.</span></span> 
  
|<span data-ttu-id="5f55e-115">ReminderType * * elemento valor * *</span><span class="sxs-lookup"><span data-stu-id="5f55e-115">****ReminderType** element value**</span></span>|<span data-ttu-id="5f55e-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5f55e-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5f55e-117">Todos</span><span class="sxs-lookup"><span data-stu-id="5f55e-117">All</span></span>  <br/> |<span data-ttu-id="5f55e-118">Lembretes que ocorrem entre o **BeginTime** e **EndTime**.</span><span class="sxs-lookup"><span data-stu-id="5f55e-118">Reminders that occur between the **BeginTime** and **EndTime**.</span></span>  <br/> |
|<span data-ttu-id="5f55e-119">Atual</span><span class="sxs-lookup"><span data-stu-id="5f55e-119">Current</span></span>  <br/> |<span data-ttu-id="5f55e-120">Lembretes retornados por **todos**, além de lembretes mais antigos que a janela de tempo solicitado se o evento for ainda em andamento, além de todos os compromissos, independentemente da idade.</span><span class="sxs-lookup"><span data-stu-id="5f55e-120">Reminders returned by **All**, plus reminders that are earlier than the requested time window if the event is still ongoing, plus all appointments regardless of age.</span></span>  <br/> |
|<span data-ttu-id="5f55e-121">Antigo</span><span class="sxs-lookup"><span data-stu-id="5f55e-121">Old</span></span>  <br/> |<span data-ttu-id="5f55e-122">Retornado por **todos**, menos os eventos que não tenham sido concluídas ainda, menos todos os compromissos de lembretes.</span><span class="sxs-lookup"><span data-stu-id="5f55e-122">Reminders returned by **All**, minus events that haven't completed yet, minus all appointments.</span></span> <span data-ttu-id="5f55e-123">Os elementos **BeginTime** e **EndTime** devem ser definidos para usar o valor **antigo** .</span><span class="sxs-lookup"><span data-stu-id="5f55e-123">The **BeginTime** and **EndTime** elements must be set to use the **Old** value.</span></span>  <br/> |
   
### <a name="getreminders-operation-soap-headers"></a><span data-ttu-id="5f55e-124">Cabeçalhos SOAP GetReminders operação</span><span class="sxs-lookup"><span data-stu-id="5f55e-124">GetReminders operation SOAP headers</span></span>

<span data-ttu-id="5f55e-125">A operação **GetReminders** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="5f55e-125">The **GetReminders** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="5f55e-126">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="5f55e-126">**Header name**</span></span>|<span data-ttu-id="5f55e-127">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5f55e-127">**Element**</span></span>|<span data-ttu-id="5f55e-128">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5f55e-128">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="5f55e-129">**Representação**</span><span class="sxs-lookup"><span data-stu-id="5f55e-129">**Impersonation**</span></span> <br/> |[<span data-ttu-id="5f55e-130">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="5f55e-130">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="5f55e-131">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="5f55e-131">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="5f55e-132">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f55e-132">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="5f55e-133">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="5f55e-133">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="5f55e-134">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="5f55e-134">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="5f55e-135">Identifica a cultura, conforme definido no RFC 3066, "Marcas para a identificação de idiomas", que será usada para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="5f55e-135">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="5f55e-136">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f55e-136">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="5f55e-137">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="5f55e-137">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="5f55e-138">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="5f55e-138">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="5f55e-139">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="5f55e-139">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="5f55e-140">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f55e-140">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="5f55e-141">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="5f55e-141">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="5f55e-142">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5f55e-142">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="5f55e-143">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="5f55e-143">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="5f55e-144">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="5f55e-144">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getreminders-operation-request-example"></a><span data-ttu-id="5f55e-145">Exemplo de solicitação de operação GetReminders</span><span class="sxs-lookup"><span data-stu-id="5f55e-145">GetReminders operation request example</span></span>

<span data-ttu-id="5f55e-146">O exemplo a seguir de uma solicitação de operação **GetReminders** mostra como recuperar os itens de calendário de cinco primeiro que ocorrem entre o **BeginTime** e **EndTime**.</span><span class="sxs-lookup"><span data-stu-id="5f55e-146">The following example of a **GetReminders** operation request shows how to retrieve the first five calendar items that occur between the **BeginTime** and **EndTime**.</span></span>
  
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
    <m:GetReminders>
      <m:EndTime>2014-04-16T21:00:00Z</m:EndTime>
      <m:ReminderType>All</m:ReminderType>
    </m:GetReminders>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="5f55e-147">O exemplo de solicitação SOAP body contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="5f55e-147">The example request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5f55e-148">GetReminders</span><span class="sxs-lookup"><span data-stu-id="5f55e-148">GetReminders</span></span>](getreminders.md)
    
- [<span data-ttu-id="5f55e-149">EndTime</span><span class="sxs-lookup"><span data-stu-id="5f55e-149">EndTime</span></span>](endtime-remindermessagedatatype.md)
    
- [<span data-ttu-id="5f55e-150">ReminderType</span><span class="sxs-lookup"><span data-stu-id="5f55e-150">ReminderType</span></span>](remindertype.md)
    
<span data-ttu-id="5f55e-151">O corpo SOAP também pode conter os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="5f55e-151">The SOAP body can also contain the following elements:</span></span>
  
- [<span data-ttu-id="5f55e-152">BeginTime</span><span class="sxs-lookup"><span data-stu-id="5f55e-152">BeginTime</span></span>](begintime.md)
    
- [<span data-ttu-id="5f55e-153">MaxItems</span><span class="sxs-lookup"><span data-stu-id="5f55e-153">MaxItems</span></span>](maxitems.md)
    
## <a name="successful-getreminders-operation-response"></a><span data-ttu-id="5f55e-154">Resposta de operação GetReminders bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="5f55e-154">Successful GetReminders operation response</span></span>

<span data-ttu-id="5f55e-155">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **GetReminders** .</span><span class="sxs-lookup"><span data-stu-id="5f55e-155">The following example shows a successful response to a **GetReminders** operation request.</span></span> <span data-ttu-id="5f55e-156">A resposta conterá um lembrete para o item de calendário "Reunião da equipe" e um lembrete para a tarefa "Tarefa para enviar anotações da reunião".</span><span class="sxs-lookup"><span data-stu-id="5f55e-156">The response contains a reminder for the "Team meeting" calendar item and a reminder for the "Task to send meeting notes" task.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="5f55e-157">Identificadores foram diminuídos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5f55e-157">Identifiers have been shortened to preserve readability.</span></span> 
  
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
    <GetRemindersResponse ResponseClass="Success"
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <Reminders>
        <Reminder xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Subject>Team meeting</Subject>
          <Location />
          <ReminderTime>2014-04-15T21:00:00Z</ReminderTime>
          <StartDate>2014-04-15T21:00:00Z</StartDate>
          <EndDate>2014-04-15T21:30:00Z</EndDate>
          <ItemId Id="vQAAAA=="
                  ChangeKey="DwAAABYAAAB4to43JyybTYwHLBM1k8MxAAACRoV4" />
          <RecurringMasterItemId Id="K7u5AAA=" ChangeKey="DwAAABYAAAB4to43JyybTYwHLBM1k8MxAAACRoV0" />
          <ReminderGroup>Calendar</ReminderGroup>
          <UID>6CF2FA62</UID>
        </Reminder>
        <Reminder xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Subject>Task to send meeting notes</Subject>
          <Location />
          <ReminderTime>2014-04-16T14:00:00Z</ReminderTime>
          <StartDate>0001-01-02T00:00:00Z</StartDate>
          <EndDate>0001-01-02T00:00:00Z</EndDate>
          <ItemId Id="vAAAAA=="
                  ChangeKey="EwAAABQAAACOs0HEMq1WTKpI7sNu5qXNAAAIDg==" />
          <ReminderGroup>Task</ReminderGroup>
          <UID>vAAAAA==</UID>
        </Reminder>
      </Reminders>
    </GetRemindersResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="5f55e-158">A resposta SOAP body contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="5f55e-158">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5f55e-159">GetRemindersResponse</span><span class="sxs-lookup"><span data-stu-id="5f55e-159">GetRemindersResponse</span></span>](getremindersresponse.md)
    
- [<span data-ttu-id="5f55e-160">Reminders</span><span class="sxs-lookup"><span data-stu-id="5f55e-160">Reminders</span></span>](reminders.md)
    
- [<span data-ttu-id="5f55e-161">Lembrete</span><span class="sxs-lookup"><span data-stu-id="5f55e-161">Reminder</span></span>](reminder.md)
    
- [<span data-ttu-id="5f55e-162">Assunto</span><span class="sxs-lookup"><span data-stu-id="5f55e-162">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="5f55e-163">Location</span><span class="sxs-lookup"><span data-stu-id="5f55e-163">Location</span></span>](location-remindermessagedatatype.md)
    
- [<span data-ttu-id="5f55e-164">ReminderTime</span><span class="sxs-lookup"><span data-stu-id="5f55e-164">ReminderTime</span></span>](remindertime.md)
    
- [<span data-ttu-id="5f55e-165">StartDate</span><span class="sxs-lookup"><span data-stu-id="5f55e-165">StartDate</span></span>](startdate.md)
    
- [<span data-ttu-id="5f55e-166">EndDate</span><span class="sxs-lookup"><span data-stu-id="5f55e-166">EndDate</span></span>](enddate-remindertype.md)
    
- [<span data-ttu-id="5f55e-167">ItemId</span><span class="sxs-lookup"><span data-stu-id="5f55e-167">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="5f55e-168">RecurringMasterItemId</span><span class="sxs-lookup"><span data-stu-id="5f55e-168">RecurringMasterItemId</span></span>](recurringmasteritemid.md)
    
- [<span data-ttu-id="5f55e-169">ReminderGroup</span><span class="sxs-lookup"><span data-stu-id="5f55e-169">ReminderGroup</span></span>](remindergroup.md)
    
- [<span data-ttu-id="5f55e-170">UID</span><span class="sxs-lookup"><span data-stu-id="5f55e-170">UID</span></span>](uid-remindertype.md)
    
## <a name="getreminders-operation-error-response-example"></a><span data-ttu-id="5f55e-171">Exemplo de resposta de erro de operação GetReminders</span><span class="sxs-lookup"><span data-stu-id="5f55e-171">GetReminders operation error response example</span></span>

<span data-ttu-id="5f55e-172">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **GetReminders** .</span><span class="sxs-lookup"><span data-stu-id="5f55e-172">The following example shows an error response to a **GetReminders** operation request.</span></span> <span data-ttu-id="5f55e-173">Esta é uma resposta a uma solicitação em que a data final foi anterior à data de início.</span><span class="sxs-lookup"><span data-stu-id="5f55e-173">This is a response to a request in which the end date was earlier than the start date.</span></span> 
  
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
    <GetRemindersResponse ResponseClass="Error"
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <MessageText>EndDate is earlier than StartDate</MessageText>
      <ResponseCode>ErrorInvalidOperation</ResponseCode>
      <DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetRemindersResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="5f55e-174">A resposta de erro corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="5f55e-174">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5f55e-175">GetRemindersResponse</span><span class="sxs-lookup"><span data-stu-id="5f55e-175">GetRemindersResponse</span></span>](getremindersresponse.md)
    
- [<span data-ttu-id="5f55e-176">MessageText</span><span class="sxs-lookup"><span data-stu-id="5f55e-176">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="5f55e-177">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5f55e-177">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="5f55e-178">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="5f55e-178">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="5f55e-179">Para códigos de erro adicionais que são genérica do EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="5f55e-179">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="5f55e-180">Confira também</span><span class="sxs-lookup"><span data-stu-id="5f55e-180">See also</span></span>


- [<span data-ttu-id="5f55e-181">PerformReminderAction</span><span class="sxs-lookup"><span data-stu-id="5f55e-181">PerformReminderAction</span></span>](performreminderaction.md)
    

