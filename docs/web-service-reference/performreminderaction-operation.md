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
# <a name="performreminderaction-operation"></a>Operação PerformReminderAction

Encontre informações sobre a operação de EWS **PerformReminderAction** . 
  
A operação de serviços Web do Exchange (EWS) **PerformReminderAction** inicia uma ação dismiss ou adiar sobre um lembrete. 
  
This operation was introduced in Exchange Server 2013.
  
## <a name="using-the-performreminderaction-operation"></a>Usando a operação PerformReminderAction

Você pode usar a operação **PerformReminderAction** para descartar ou snooze lembretes (atraso) retornados pela operação de [GetReminders](getreminders-operation.md) . Para adiar um lembrete, defina o [ActionType](actiontype-reminderactiontype.md) como **Snooze**e definir o valor de [NewReminderTime](newremindertime.md) até um momento posterior à atual [ReminderTime](remindertime.md), caso contrário, o **NewReminderTime** será ignorado pelo servidor. Se o lembrete for para uma ocorrência de uma reunião recorrente, e a ação de **Snooze** será executada o lembrete com **NewReminderTime** passar o lembrete da próxima ocorrência, o lembrete efetivamente é descartado. 
  
Para descartar um lembrete, defina o **ActionType** como **Dismiss**. Quando o servidor processa a solicitação, o servidor altera o valor de [IsReminderSet](isreminderset.md) para o item de **True** para **False**.
  
### <a name="performreminderaction-operation-soap-headers"></a>Cabeçalhos SOAP PerformReminderAction operação

A operação **PerformReminderAction** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir. 
  
|**Nome de cabeçalho**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**Representação** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifica o usuário que o aplicativo cliente está representando. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifica a cultura, conforme definido no RFC 3066, "Marcas para a identificação de idiomas", que será usada para acessar a caixa de correio. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Este cabeçalho é aplicável a uma resposta.  <br/> |
   
## <a name="performreminderaction-operation-request-example"></a>Exemplo de solicitação de operação PerformReminderAction

O exemplo a seguir de uma solicitação de operação **PerformReminderAction** mostra como snooze um lembrete atual e definir um novo horário do lembrete. Observe que você precisa incluir o **ChangeKey** para o [ItemId](itemid.md) e o **NewReminderTime** deve ser definida para um horário mais recente do que o **ReminderTime** retornados pela operação de [GetReminders](getreminders-operation.md) . 
  
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
> O valor de **ItemId** foi reduzido para preservar a legibilidade. 
  
A solicitação de corpo SOAP contém os seguintes elementos:
  
- [PerformReminderAction](performreminderaction.md)
    
- [ReminderItemActions](reminderitemactions.md)
    
- [ReminderItemAction](reminderitemaction.md)
    
- [ActionType](actiontype-reminderactiontype.md)
    
- [ItemId](itemid.md)
    
- [NewReminderTime](newremindertime.md)
    
## <a name="successful-performreminderaction-operation-response"></a>Resposta de operação PerformReminderAction bem-sucedida

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **PerformReminderAction** . O elemento **UpdatedItemIds** contém o **ItemIds** do item de calendário atualizados. 
  
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

A resposta SOAP body contém os seguintes elementos:
  
- [PerformReminderActionResponse](performreminderactionresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [UpdatedItemIds](updateditemids.md)
    
- [ItemId](itemid.md)
    
## <a name="performreminderaction-operation-error-response-example"></a>Exemplo de resposta de erro de operação PerformReminderAction

O exemplo a seguir mostra uma resposta a uma solicitação de operação **PerformReminderAction** quando nenhuma alteração foi feita no servidor. Esta é uma resposta na qual uma solicitação foi enviada, mas nenhum **UpdatedItemIds** foram retornados, que significa que nenhum lembretes foram alteradas. 
  
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

A resposta de erro corpo SOAP contém os seguintes elementos:
  
- [PerformReminderActionResponse](performreminderactionresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [UpdatedItemIds](updateditemids.md)
    
Para códigos de erro adicionais que são genéricos para o EWS, consulte [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>Confira também


- [Operação GetReminders](getreminders-operation.md)
    

