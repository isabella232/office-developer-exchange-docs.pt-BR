---
title: Operação GetEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetEvents
api_type:
- schema
ms.assetid: f268efe5-9a1a-41a2-b6a6-51fcde7720a1
description: A operação GetEvents é usada por clientes de assinatura pull para solicitar notificações do servidor de acesso para cliente. A resposta da operação GetEvents retorna uma matriz de itens e eventos que ocorreram em uma caixa de correio desde a última notificação.
ms.openlocfilehash: 9258fd003c242911866aa7abbca5eba2b9582223
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462511"
---
# <a name="getevents-operation"></a>Operação GetEvents

A operação **GetEvents** é usada por clientes de assinatura pull para solicitar notificações do servidor de acesso para cliente. A resposta da operação **GetEvents** retorna uma matriz de itens e eventos que ocorreram em uma caixa de correio desde a última notificação. 
  
> [!IMPORTANT]
> A operação **DeleteUserConfiguration** acionará um evento move para o sistema de notificação de eventos. O objeto de configuração do usuário será movido para o dumpster. 
  
## <a name="remarks"></a>Comentários

Alterações nos itens de calendário podem resultar na geração de vários eventos. Esses eventos são o resultado de itens temporários sendo criados na caixa de correio, os itens de armazenamento de dados de disponibilidade estão sendo alterados como parte das operações normais do calendário ou ambos. Eventos de classe de item "IPM. SchedulePlus. FreeBusy. BinaryData "deve ser ignorado por clientes de serviço Web. Esses itens temporários são excluídos após serem criados; Portanto, se for feita uma tentativa de recuperar esses itens, um erro será retornado afirmando que o item não foi encontrado.
  
## <a name="getevents-request-example"></a>Exemplo de solicitação GetEvents

### <a name="description"></a>Descrição

O exemplo a seguir mostra como solicitar os eventos e os itens que estão associados a uma assinatura identificada pelo identificador de assinatura e marca d' água.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetEvents xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</SubscriptionId>
      <Watermark>AAAAAMAGAAAAAAAAAQ==</Watermark>
    </GetEvents>
  </soap:Body>
</soap:Envelope>
```

### <a name="getevents-request-elements"></a>Elementos de solicitação GetEvents

Os seguintes elementos são usados na solicitação:
  
- [GetEvents](getevents.md)
    
- [SubscriptionId (GetEvents)](subscriptionid-getevents.md)
    
- [Marca d'água](watermark.md)
    
## <a name="successful-getevents-response-example"></a>Exemplo de resposta de GetEvents bem-sucedida

### <a name="description"></a>Descrição

O exemplo a seguir de uma resposta mostra uma notificação da existência de duas novas mensagens de email desde que a última solicitação de notificação foi enviada ao servidor.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetEventsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetEventsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Notification>
            <t:SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</t:SubscriptionId>
            <t:PreviousWatermark>AAAAAMAGAAAAAAAAAQ==</t:PreviousWatermark>
            <t:MoreEvents>false</t:MoreEvents>
            <t:NewMailEvent>
              <t:Watermark>AAAAAM4GAAAAAAAAAQ==</t:Watermark>
              <t:TimeStamp>2006-08-22T00:36:29Z</t:TimeStamp>
              <t:ItemId Id="AQApAHR" ChangeKey="CQAAAA==" />
              <t:ParentFolderId Id="AQApAH" ChangeKey="AQAAAA==" />
            </t:NewMailEvent>
            <t:NewMailEvent>
              <t:Watermark>AAAAAOQGAAAAAAAAAQ==</t:Watermark>
              <t:TimeStamp>2006-08-22T01:00:50Z</t:TimeStamp>
              <t:ItemId Id="AQApAHRw" ChangeKey="CQAAAA==" />
              <t:ParentFolderId Id="AQApAH" ChangeKey="AQAAAA==" />
            </t:NewMailEvent>
          </m:Notification>
        </m:GetEventsResponseMessage>
      </m:ResponseMessages>
    </GetEventsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comentários

> [!NOTE]
> Os identificadores de item e de pasta foram reduzidos para preservar a legibilidade. 
  
### <a name="getevents-response-elements"></a>Elementos de resposta de GetEvents

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [GetEventsResponse](geteventsresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetEventsResponseMessage](geteventsresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Notificação](notification-ex15websvcsotherref.md)
    
- [SubscriptionId (GetEvents)](subscriptionid-getevents.md)
    
- [PreviousWatermark](previouswatermark.md)
    
- [MoreEvents](moreevents.md)
    
- [NewMailEvent](newmailevent.md)
    
- [Marca d'água](watermark.md)
    
- [Registra](timestamp.md)
    
- [ItemId](itemid.md)
    
- [ParentFolderId](parentfolderid.md)
    
Para encontrar outras opções para a mensagem de resposta da operação **GetEvents** , explore a hierarquia de esquema. Inicie no elemento [Notification](notification-ex15websvcsotherref.md) . 
  
## <a name="getevents-error-response-example"></a>Exemplo de resposta de erro GetEvents

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta de erro a uma solicitação **GetEvents** . 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetEventsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetEventsResponseMessage ResponseClass="Error">
          <m:MessageText>Access is denied. Only the subscription owner may access the subscription.</m:MessageText>
          <m:ResponseCode>ErrorSubscriptionAccessDenied</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:GetEventsResponseMessage>
      </m:ResponseMessages>
    </GetEventsResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="remarks"></a>Comentários

Durante o processamento de uma solicitação **GetEvents** , o servidor de acesso para cliente realiza as seguintes etapas: 
  
1. A SubscriptionId da solicitação é confirmada como uma assinatura válida hospedada no servidor de acesso para cliente. Se não for, a chamada **GetEvents** falhará. 
    
2. O endereço SMTP do usuário autenticado para a solicitação é comparado com o endereço SMTP do usuário que criou a assinatura. Se eles não corresponderem, a solicitação **GetEvents** falhará. 
    
3. A fila de assinatura é consultada para eventos que estão aguardando para serem enviados para o cliente. Se a fila não estiver vazia, os primeiros eventos 50 da fila são retirados da fila e codificados em uma notificação.
    
4. Se nenhum evento for encontrado na fila, um StatusEvent é gerado e codificado em uma resposta de notificação.
    
5. A resposta de notificação é retornada ao cliente.
    
6. Os eventos incluídos na notificação são removidos da fila de assinatura e o servidor de acesso para cliente última marca d' água local da assinatura é definida como a marca d' água do último evento retornado.
    
7. O temporizador de tempo limite da assinatura é redefinido.
    
## <a name="see-also"></a>Confira também



[Operação Subscribe](subscribe-operation.md)
  
[Cancelar a operação](unsubscribe-operation.md)


[Usando assinaturas pull](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)

