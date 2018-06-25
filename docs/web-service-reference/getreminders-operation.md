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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752611"
---
# <a name="getreminders-operation"></a>Operação GetReminders

Encontre informações sobre a operação de EWS **GetReminders** . 
  
A operação de serviços Web do Exchange (EWS) **GetReminders** recupera lembretes para itens de calendário e tarefas. 
  
This operation was introduced in Exchange Server 2013.
  
## <a name="using-the-getreminders-operation"></a>Usando a operação GetReminders

A operação **GetReminders** obtém lembretes de calendário atual e futuro e itens de tarefa na caixa de correio do usuário, dependendo dos valores do elemento passado na solicitação. A operação pode recuperar todos os itens de calendário atuais e futuros, bem como tarefas que possuem um lembrete definido. Itens de calendário particular são incluídos nas respostas. Tarefas sem lembretes não são incluídas nas respostas, nem são emails com lembretes ou sinalizadores de acompanhamento. 
  
Para recuperar todos os lembretes atuais, recomendamos a configuração do [ReminderType](remindertype.md) para **todos** e o [EndTime](endtime-remindermessagedatatype.md) para a hora atual. 
  
Se os elementos [BeginTime](begintime.md) e **EndTime** estão incluídos na solicitação, a resposta inclui os lembretes para qualquer calendário e itens de tarefa que ocorrem entre tiverem um lembrete que ocorre entre o **BeginTime** e **EndTime**.
  
A tabela a seguir descreve o comportamento do elemento **ReminderType** quando os elementos **BeginTime** e **EndTime** são incluídos. 
  
|ReminderType * * elemento valor * *|**Descrição**|
|:-----|:-----|
|Todos  <br/> |Lembretes que ocorrem entre o **BeginTime** e **EndTime**.  <br/> |
|Atual  <br/> |Lembretes retornados por **todos**, além de lembretes mais antigos que a janela de tempo solicitado se o evento for ainda em andamento, além de todos os compromissos, independentemente da idade.  <br/> |
|Antigo  <br/> |Retornado por **todos**, menos os eventos que não tenham sido concluídas ainda, menos todos os compromissos de lembretes. Os elementos **BeginTime** e **EndTime** devem ser definidos para usar o valor **antigo** .  <br/> |
   
### <a name="getreminders-operation-soap-headers"></a>Cabeçalhos SOAP GetReminders operação

A operação **GetReminders** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir. 
  
|**Nome de cabeçalho**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**Representação** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifica o usuário que o aplicativo cliente está representando. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifica a cultura, conforme definido no RFC 3066, "Marcas para a identificação de idiomas", que será usada para acessar a caixa de correio. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Este cabeçalho é aplicável a uma resposta.  <br/> |
   
## <a name="getreminders-operation-request-example"></a>Exemplo de solicitação de operação GetReminders

O exemplo a seguir de uma solicitação de operação **GetReminders** mostra como recuperar os itens de calendário de cinco primeiro que ocorrem entre o **BeginTime** e **EndTime**.
  
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

O exemplo de solicitação SOAP body contém os seguintes elementos:
  
- [GetReminders](getreminders.md)
    
- [EndTime](endtime-remindermessagedatatype.md)
    
- [ReminderType](remindertype.md)
    
O corpo SOAP também pode conter os seguintes elementos:
  
- [BeginTime](begintime.md)
    
- [MaxItems](maxitems.md)
    
## <a name="successful-getreminders-operation-response"></a>Resposta de operação GetReminders bem-sucedida

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **GetReminders** . A resposta conterá um lembrete para o item de calendário "Reunião da equipe" e um lembrete para a tarefa "Tarefa para enviar anotações da reunião". 
  
> [!NOTE]
> Identificadores foram diminuídos para preservar a legibilidade. 
  
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

A resposta SOAP body contém os seguintes elementos:
  
- [GetRemindersResponse](getremindersresponse.md)
    
- [Reminders](reminders.md)
    
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

O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **GetReminders** . Esta é uma resposta a uma solicitação em que a data final foi anterior à data de início. 
  
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

A resposta de erro corpo SOAP contém os seguintes elementos:
  
- [GetRemindersResponse](getremindersresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
Para códigos de erro adicionais que são genérica do EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>Confira também


- [PerformReminderAction](performreminderaction.md)
    

