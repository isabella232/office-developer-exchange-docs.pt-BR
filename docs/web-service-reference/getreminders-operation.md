---
title: Operação getlembretes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1b56f83f-3b87-4b55-8259-fde6692da681
description: Encontre informações sobre a operação do EWS de getlembretes.
ms.openlocfilehash: dcbe20c674d7524a7776d374fa6964899abf472f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458303"
---
# <a name="getreminders-operation"></a>Operação getlembretes

Encontre informações sobre a operação do EWS de **Getlembretes** . 
  
A operação dos serviços Web do Exchange (EWS) do **Getlembretes** recupera lembretes para itens de calendário e tarefa. 
  
This operation was introduced in Exchange Server 2013.
  
## <a name="using-the-getreminders-operation"></a>Usando a operação getlembretes

A operação **Getlembretes** Obtém lembretes para os itens de calendário e de tarefa atuais e futuros na caixa de correio do usuário, dependendo dos valores de elemento passados na solicitação. A operação pode recuperar todos os itens de calendário atuais e futuros, bem como tarefas que tenham um lembrete definido. Os itens de calendário privado estão incluídos nas respostas. Tarefas sem lembretes não estão incluídas em respostas, nem emails com lembretes ou sinalizadores de acompanhamento. 
  
Para recuperar todos os lembretes atuais, recomendamos definir o [lembrete](remindertype.md) como **todos** e a [EndTime](endtime-remindermessagedatatype.md) como a hora atual. 
  
Se os elementos [BeginTime](begintime.md) e **EndTime** forem incluídos na solicitação, a resposta inclui lembretes para qualquer calendário e itens de tarefa que ocorrem entre ter um lembrete que ocorre entre o **BeginTime** e a **EndTime**.
  
A tabela a seguir descreve o comportamento do elemento **Remindertype** quando os elementos **BeginTime** e **EndTime** são incluídos. 
  
|Lembrete * * valor do elemento * *|**Descrição**|
|:-----|:-----|
|Todos  <br/> |Lembretes que ocorrem entre **BeginTime** e **EndTime**.  <br/> |
|Atual  <br/> |Lembretes retornados por **todos**, além de lembretes anteriores à janela de tempo solicitada, se o evento ainda estiver em andamento, além de todos os compromissos, independentemente da idade.  <br/> |
|Antigo  <br/> |Lembretes retornados por **todos**, menos eventos que ainda não foram concluídos, menos todos os compromissos. Os elementos **BeginTime** e **EndTime** devem ser definidos para usar o valor **antigo** .  <br/> |
   
### <a name="getreminders-operation-soap-headers"></a>Cabeçalhos SOAP de operação de islembretes

A operação **Getlembretes** pode usar os cabeçalhos SOAP listados na tabela a seguir. 
  
|**Nome de cabeçalho**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**Representação** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifica o usuário que o aplicativo cliente está representando. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifica a cultura, conforme definido na RFC 3066, "marcas de identificação de idiomas", a ser usado para acessar a caixa de correio. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Este cabeçalho é aplicável a uma resposta.  <br/> |
   
## <a name="getreminders-operation-request-example"></a>Exemplo de solicitação de operação getlembretes

O exemplo a seguir de uma solicitação de operação **Getlembretes** mostra como recuperar os cinco primeiros itens de calendário que ocorrem entre o **BeginTime** e a **EndTime**.
  
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

O corpo SOAP de solicitação de exemplo contém os seguintes elementos:
  
- [Getlembretes](getreminders.md)
    
- [EndTime](endtime-remindermessagedatatype.md)
    
- [Remindertype](remindertype.md)
    
O corpo SOAP também pode conter os seguintes elementos:
  
- [BeginTime](begintime.md)
    
- [MaxItems](maxitems.md)
    
## <a name="successful-getreminders-operation-response"></a>Resposta de operação de getlembretes bem-sucedida

O exemplo a seguir mostra uma resposta bem-sucedida para uma solicitação de operação **Getlembretes** . A resposta contém um lembrete para o item de calendário "reunião de equipe" e um lembrete para a tarefa "tarefa de envio de anotações da reunião". 
  
> [!NOTE]
> Os identificadores foram reduzidos para preservar a legibilidade. 
  
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
    
- [Localização](location-remindermessagedatatype.md)
    
- [ReminderTime](remindertime.md)
    
- [StartDate](startdate.md)
    
- [EndDate](enddate-remindertype.md)
    
- [ItemId](itemid.md)
    
- [RecurringMasterItemId](recurringmasteritemid.md)
    
- [Um dos lembretes](remindergroup.md)
    
- [UID](uid-remindertype.md)
    
## <a name="getreminders-operation-error-response-example"></a>Exemplo de resposta de erro de operação de lembretes

O exemplo a seguir mostra uma resposta de erro para uma solicitação de operação **Getlembretes** . Esta é uma resposta a uma solicitação na qual a data de término era anterior à data de início. 
  
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

O corpo SOAP de resposta de erro contém os seguintes elementos:
  
- [GetRemindersResponse](getremindersresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
Para obter códigos de erro adicionais genéricos para o EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>Confira também


- [PerformReminderAction](performreminderaction.md)
    

