---
title: Operação GetReminders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 1b56f83f-3b87-4b55-8259-fde6692da681
description: Encontre informações sobre a operação GetReminders EWS.
ms.openlocfilehash: e47dbb6ffceac3535bb72f93ee27bbb3f3f259e6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513560"
---
# <a name="getreminders-operation"></a>Operação GetReminders

Encontre informações sobre a **operação GetReminders** EWS. 
  
A **operação GetReminders** Exchange Web Services (EWS) recupera lembretes para itens de calendário e tarefas. 
  
This operation was introduced in Exchange Server 2013.
  
## <a name="using-the-getreminders-operation"></a>Usando a operação GetReminders

A **operação GetReminders** obtém lembretes para os itens de calendário e tarefa atuais e futuros na caixa de correio do usuário, dependendo dos valores de elemento passados na solicitação. A operação pode recuperar todos os itens de calendário atuais e futuros, bem como tarefas que tenham um conjunto de lembretes. Itens de calendário particular são incluídos nas respostas. Tarefas sem lembretes não são incluídas em respostas, nem emails com lembretes ou sinalizadores de acompanhamento. 
  
Para recuperar todos os lembretes atuais, recomendamos definir [ReminderType](remindertype.md) como **Todos** e [EndTime](endtime-remindermessagedatatype.md) para a hora atual. 
  
Se os elementos [BeginTime](begintime.md) e **EndTime** são incluídos na solicitação, a resposta inclui lembretes para qualquer calendário e itens de tarefa que ocorrem entre eles têm um lembrete que ocorre entre **BeginTime** e **EndTime**.
  
A tabela a seguir descreve o comportamento do **elemento ReminderType** quando os **elementos BeginTime** e **EndTime** são incluídos. 
  
|Valor do elemento ReminderType** **|**Descrição**|
|:-----|:-----|
|Todos  <br/> |Lembretes que ocorrem entre **BeginTime** **e EndTime**.  <br/> |
|Atual  <br/> |Lembretes retornados por **All**, mais lembretes anteriores à janela de tempo solicitada se o evento ainda estiver em andamento, além de todos os compromissos, independentemente da idade.  <br/> |
|Antigo  <br/> |Lembretes retornados por **Todos**, menos eventos que ainda não foram concluídos, menos todos os compromissos. Os **elementos BeginTime** **e EndTime** devem ser definidos para usar o **valor** Antigo.  <br/> |
   
### <a name="getreminders-operation-soap-headers"></a>Headers SOAP da operação GetReminders

A **operação GetReminders** pode usar os headers SOAP listados na tabela a seguir. 
  
|**Nome de cabeçalho**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**Representação** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifica o usuário que o aplicativo cliente está representando. Esse header é aplicável a uma solicitação.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifica a cultura, conforme definido na RFC 3066, "Marcas para a Identificação de Idiomas", a ser usada para acessar a caixa de correio. Esse header é aplicável a uma solicitação.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Esse header é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Esse header é aplicável a uma resposta.  <br/> |
   
## <a name="getreminders-operation-request-example"></a>Exemplo de solicitação de operação GetReminders

O exemplo a seguir de uma solicitação de operação **GetReminders** mostra como recuperar os cinco primeiros itens de calendário que ocorrem entre **BeginTime** e **EndTime**.
  
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
    <m:GetReminders>
      <m:EndTime>2014-04-16T21:00:00Z</m:EndTime>
      <m:ReminderType>All</m:ReminderType>
    </m:GetReminders>
  </soap:Body>
</soap:Envelope>
```

O corpo soap de solicitação de exemplo contém os seguintes elementos:
  
- [GetReminders](getreminders.md)
    
- [EndTime](endtime-remindermessagedatatype.md)
    
- [ReminderType](remindertype.md)
    
O corpo SOAP também pode conter os seguintes elementos:
  
- [BeginTime](begintime.md)
    
- [MaxItems](maxitems.md)
    
## <a name="successful-getreminders-operation-response"></a>Resposta bem-sucedida da operação GetReminders

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **GetReminders.** A resposta contém um lembrete para o item de calendário "Reunião de equipe" e um lembrete para a tarefa "Tarefa para enviar anotações de reunião". 
  
> [!NOTE]
> Os identificadores foram reduzidos para preservar a capacidade de leitura. 
  
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
    <GetRemindersResponse ResponseClass="Success"
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <Reminders>
        <Reminder xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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
        <Reminder xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

O corpo SOAP de resposta contém os seguintes elementos:
  
- [GetRemindersResponse](getremindersresponse.md)
    
- [Lembretes](reminders.md)
    
- [Lembrete](reminder.md)
    
- [Assunto](subject.md)
    
- [Location](location-remindermessagedatatype.md)
    
- [ReminderTime](remindertime.md)
    
- [StartDate](startdate.md)
    
- [EndDate](enddate-remindertype.md)
    
- [ItemId](itemid.md)
    
- [RecurringMasterItemId](recurringmasteritemid.md)
    
- [ReminderGroup](remindergroup.md)
    
- [UID](uid-remindertype.md)
    
## <a name="getreminders-operation-error-response-example"></a>Exemplo de resposta de erro de operação GetReminders

O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **GetReminders.** Esta é uma resposta a uma solicitação na qual a data de término era anterior à data de início. 
  
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
    <GetRemindersResponse ResponseClass="Error"
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <MessageText>EndDate is earlier than StartDate</MessageText>
      <ResponseCode>ErrorInvalidOperation</ResponseCode>
      <DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetRemindersResponse>
  </s:Body>
</s:Envelope>
```

O corpo SOAP da resposta de erro contém os seguintes elementos:
  
- [GetRemindersResponse](getremindersresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
Para obter códigos de erro adicionais genéricos para EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>Confira também


- [PerformReminderAction](performreminderaction.md)
    

