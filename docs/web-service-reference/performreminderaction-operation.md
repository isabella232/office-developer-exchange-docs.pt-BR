---
title: Operação PerformReminderAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: c597bb0e-13b0-422e-9c23-970463e2a5c3
description: Encontre informações sobre a operação PerformReminderAction EWS.
ms.openlocfilehash: ca547c401100afdfd9d846ca3bfddf710efd2797
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515303"
---
# <a name="performreminderaction-operation"></a>Operação PerformReminderAction

Encontre informações sobre a **operação PerformReminderAction** EWS. 
  
A **operação PerformReminderAction** Exchange Web Services (EWS) inicia uma ação de demissão ou snooze em um lembrete. 
  
This operation was introduced in Exchange Server 2013.
  
## <a name="using-the-performreminderaction-operation"></a>Usando a operação PerformReminderAction

Você pode usar a **operação PerformReminderAction** para descartar ou esnocar lembretes (atraso) retornados pela [operação GetReminders.](getreminders-operation.md) Para esnocar um lembrete, de definir [o ActionType](actiontype-reminderactiontype.md) como **Snooze** e definir o valor [NewReminderTime](newremindertime.md) como um tempo posterior ao [ReminderTime](remindertime.md)atual , caso **contrário, NewReminderTime** será ignorado pelo servidor. Se o lembrete for para uma ocorrência de uma reunião recorrente e a ação **Snooze** for tomada no lembrete com um **NewReminderTime** que está além do lembrete da próxima ocorrência, o lembrete será efetivamente ignorado. 
  
Para descartar um lembrete, de definir **ActionType** como **Dismiss**. Quando o servidor processa a solicitação, o servidor altera o [valor IsReminderSet](isreminderset.md) do item de **True** para **False**.
  
### <a name="performreminderaction-operation-soap-headers"></a>Headers SOAP da operação PerformReminderAction

A **operação PerformReminderAction** pode usar os headers SOAP listados na tabela a seguir. 
  
|**Nome de cabeçalho**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**Representação** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifica o usuário que o aplicativo cliente está representando. Esse header é aplicável a uma solicitação.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifica a cultura, conforme definido na RFC 3066, "Marcas para a Identificação de Idiomas", a ser usada para acessar a caixa de correio. Esse header é aplicável a uma solicitação.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Esse header é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Esse header é aplicável a uma resposta.  <br/> |
   
## <a name="performreminderaction-operation-request-example"></a>Exemplo de solicitação de operação PerformReminderAction

O exemplo a seguir de uma solicitação de operação **PerformReminderAction** mostra como esnocar um lembrete atual e definir um novo horário de lembrete. Observe que você precisa incluir **o ChangeKey** para [ItemId](itemid.md) e **NewReminderTime** deve ser definido para um horário posterior ao **reminderTime** retornado pela [operação GetReminders.](getreminders-operation.md) 
  
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
> O **valor ItemId** foi reduzido para preservar a capacidade de leitura. 
  
O corpo SOAP de solicitação contém os seguintes elementos:
  
- [PerformReminderAction](performreminderaction.md)
    
- [ReminderItemActions](reminderitemactions.md)
    
- [ReminderItemAction](reminderitemaction.md)
    
- [ActionType](actiontype-reminderactiontype.md)
    
- [ItemId](itemid.md)
    
- [NewReminderTime](newremindertime.md)
    
## <a name="successful-performreminderaction-operation-response"></a>Resposta bem-sucedida da operação PerformReminderAction

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **PerformReminderAction.** O **elemento UpdatedItemIds** contém **os ItemIds** do item de calendário atualizado. 
  
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

O corpo SOAP de resposta contém os seguintes elementos:
  
- [PerformReminderActionResponse](performreminderactionresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [UpdatedItemIds](updateditemids.md)
    
- [ItemId](itemid.md)
    
## <a name="performreminderaction-operation-error-response-example"></a>Exemplo de resposta de erro da operação PerformReminderAction

O exemplo a seguir mostra uma resposta a uma solicitação de operação **PerformReminderAction** quando nenhuma alteração foi feita no servidor. Esta é uma resposta na qual uma solicitação foi enviada, mas **nenhuma UpdatedItemIds** foi retornada, o que significa que nenhum lembrete foi alterado. 
  
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

O corpo SOAP da resposta de erro contém os seguintes elementos:
  
- [PerformReminderActionResponse](performreminderactionresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [UpdatedItemIds](updateditemids.md)
    
Para obter códigos de erro adicionais genéricos para EWS, consulte [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>Confira também


- [Operação GetReminders](getreminders-operation.md)
    

