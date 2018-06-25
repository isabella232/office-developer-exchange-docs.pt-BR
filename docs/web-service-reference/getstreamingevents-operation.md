---
title: Operação GetStreamingEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetStreamingEvents
api_type:
- schema
ms.assetid: 8da95423-72bc-4034-90a8-162eedcd059b
description: Encontre informações sobre o EWS GetStreamingEvents operação.
ms.openlocfilehash: 0e93be7b14cb1ca6a2a9821b016f7bdc0e8d7772
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823673"
---
# <a name="getstreamingevents-operation"></a>Operação GetStreamingEvents

Encontre informações sobre a operação de EWS **GetStreamingEvents** . 
  
A operação **GetStreamingEvents** é usada por clientes de assinatura de streaming para solicitar notificações de servidor acesso para cliente. A resposta **GetStreamingEvents** retorna uma matriz de itens e os eventos que ocorreram em uma caixa de correio desde a última notificação. 
  
## <a name="getstreamingevents-request-example"></a>Exemplo de solicitação de GetStreamingEvents

### <a name="description"></a>Descrição

O exemplo a seguir de uma operação **GetStreamingEvents** mostra como solicitar os eventos e os itens que estão associados uma assinatura que é identificada pelo identificador de inscrição. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
  xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Body>
    <GetStreamingEvents xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</SubscriptionId>
      <ConnectionTimeout>30</ConnectionTimeout>
    </GetStreamingEvents>
  </soap:Body>
</soap:Envelope>
```

### <a name="getstreamingevents-request-elements"></a>Elementos de solicitação de GetStreamingEvents

Os seguintes elementos são usados na solicitação:
  
- [GetStreamingEvents](getstreamingevents.md)
    
- [SubscriptionId (GetStreamingEvents)](subscriptionid-getstreamingevents.md)
    
- [ConnectionTimeout](connectiontimeout.md)
    
## <a name="successful-getstreamingevents-response-example"></a>Exemplo de resposta bem-sucedida GetStreamingEvents

### <a name="description"></a>Descrição

O exemplo a seguir de uma resposta **GetStreamingEvents** mostra as notificações que são enviadas para o cliente quando uma nova mensagem de email é recebida. Ele inclui notificações para os seguintes eventos: CreatedEvent, NewMail e ModifiedEvent. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Header xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <ServerVersionInfo xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="7" Version="V2_4" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" />
</soap:Header>
<soap:Body xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <m:GetStreamingEventsResponse xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
    <m:ResponseMessages>
      <m:GetStreamingEventsResponseMessage ResponseClass="Success">
        <m:ResponseCode>NoError</m:ResponseCode>
        <m:Notifications>
          <m:Notification>
            <t:SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</t:SubscriptionId>
            <t:CreatedEvent>
              <t:TimeStamp>2013-09-16T04:31:29Z</t:TimeStamp>
              <t:ItemId Id="AAMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwBGAAAAAABSSWVKrmGUTJE+MVIvofglBwDZGACZQpSgSpyNkexYe2b7AAAAAAENAADZGACZQpSgSpyNkexYe2b7AAANGFYwAAA=" ChangeKey="CQAAAA==" />
              <t:ParentFolderId Id="AQMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAuAAADUkllSq5hlEyRPjFSL6H4JQEA2RgAmUKUoEqcjZHsWHtm+wAAAgENAAAA" ChangeKey="AQAAAA==" />
            </t:CreatedEvent>
            <t:NewMailEvent>
              <t:TimeStamp>2013-09-16T04:31:29Z</t:TimeStamp>
              <t:ItemId Id="AAMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwBGAAAAAABSSWVKrmGUTJE+MVIvofglBwDZGACZQpSgSpyNkexYe2b7AAAAAAENAADZGACZQpSgSpyNkexYe2b7AAANGFYwAAA=" ChangeKey="CQAAAA==" />
              <t:ParentFolderId Id="AQMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAuAAADUkllSq5hlEyRPjFSL6H4JQEA2RgAmUKUoEqcjZHsWHtm+wAAAgENAAAA" ChangeKey="AQAAAA==" />
            </t:NewMailEvent>
            <t:ModifiedEvent>
              <t:TimeStamp>2013-09-16T04:31:29Z</t:TimeStamp>
              <t:FolderId Id="AQMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAuAAADUkllSq5hlEyRPjFSL6H4JQEA2RgAmUKUoEqcjZHsWHtm+wAAAgENAAAA" ChangeKey="AQAAAA==" />
              <t:ParentFolderId Id="AQMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAuAAADUkllSq5hlEyRPjFSL6H4JQEA2RgAmUKUoEqcjZHsWHtm+wAAAgEJAAAA" ChangeKey="AQAAAA==" />
              <t:UnreadCount>1</t:UnreadCount>
            </t:ModifiedEvent>
          </m:Notification>
        </m:Notifications>
      </m:GetStreamingEventsResponseMessage>
    </m:ResponseMessages>
  </m:GetStreamingEventsResponse>
</soap:Body>
```

### <a name="getstreamingevents-response-elements"></a>Elementos de resposta GetStreamingEvents

Os seguintes elementos são usados na resposta:
  
- [GetStreamingEventsResponse](getstreamingeventsresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetStreamingEventsResponseMessage](getstreamingeventsresponsemessage.md)
    
- [NotesFolderPermissionLevel](notesfolderpermissionlevel.md)
    
- [Notificação](notification-ex15websvcsotherref.md)
    
- [SubscriptionId (GetStreamingEvents)](subscriptionid-getstreamingevents.md)
    
Para localizar outras opções para a mensagem de resposta da operação **GetStreamingEvents** , explore a hierarquia de esquema. Inicie o elemento de [notificação](notification-ex15websvcsotherref.md) . 
  
## <a name="getstreamingevents-error-response-example"></a>Exemplo de resposta de erro GetStreamingEvents

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta de erro a uma solicitação **GetStreamingEvents** . 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetStreamingEventsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetStreamingEventsResponseMessage ResponseClass="Error">
        <m:MessageText></m:MessageText>
        <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        <m:ResponseCode>ErrorInvalidSubscription</m:ResponseCode>
        <m:ConnectionStatus>Closed</m:ConnectionStatus>
      </m:ResponseMessages>
    </GetStreamingEventsResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="remarks"></a>Comentários

Ao processar uma solicitação de **GetStreamingEvents** , o servidor de acesso para cliente executa as seguintes etapas: 
  
1. A [SubscriptionId (GetStreamingEvents)](subscriptionid-getstreamingevents.md) da solicitação é confirmada seja uma assinatura válida que está hospedada no servidor de acesso para cliente. Se não for, a chamada de **GetStreamingEvents** falhar. 
    
2. O endereço SMTP do usuário autenticado para a solicitação é validado para ter direitos de representação. Se não tiverem, a solicitação de **GetStreamingEvents** falhará. 
    
3. A fila de inscrição é consultada para eventos que estão em espera a serem enviados para o cliente. Se a fila não está vazia, os 50 primeiros eventos da fila são retirados da fila e codificados em uma notificação.
    
4. Se nenhum evento forem encontrado na fila, um [StatusEvent](statusevent.md) será gerado e codificada em uma resposta de notificação. 
    
5. A resposta de notificação é retornada para o cliente.
    
6. Os eventos que estão incluídos na notificação são removidos da fila de assinatura e acesso para cliente local de servidor última marca d'água para a assinatura é definida como a marca d'água do último evento que é retornado.
    
7. O timer de tempo limite para a assinatura é redefinido.
    
## <a name="see-also"></a>Confira também



[Inscrever-se a operação](subscribe-operation.md)
  
[Cancelar a operação](unsubscribe-operation.md)

