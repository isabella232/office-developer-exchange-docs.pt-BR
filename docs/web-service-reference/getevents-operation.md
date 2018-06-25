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
description: A operação GetEvents é usada pelos clientes de inscrição de recepção para notificações de solicitação do servidor de acesso para cliente. A resposta de operação GetEvents retorna uma matriz de itens e os eventos que ocorreram em uma caixa de correio desde a última notificação.
ms.openlocfilehash: 1a23a9d570a4554e54becb7927f25dff89888c74
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752473"
---
# <a name="getevents-operation"></a>Operação GetEvents

A operação **GetEvents** é usada pelos clientes de inscrição de recepção para notificações de solicitação do servidor de acesso para cliente. A resposta de operação **GetEvents** retorna uma matriz de itens e os eventos que ocorreram em uma caixa de correio desde a última notificação. 
  
> [!IMPORTANT]
> A operação **DeleteUserConfiguration** irá disparar um evento de movimentação para o sistema de notificação de evento. O objeto de configuração do usuário será movido para o dumpster. 
  
## <a name="remarks"></a>Comentários

Alterações nos itens de calendário podem resultar na geração de vários eventos. Esses eventos são o resultado de itens temporários que está sendo criada na caixa de correio, itens de armazenamento de dados de livre/ocupado sendo alteradas como parte das operações normais do calendário, ou ambos. Classe de eventos para o item "IPM. SchedulePlus.FreeBusy.BinaryData"devem ser ignorados pelo clientes de serviço Web. Esses itens temporários são excluídos depois que eles são criados; Portanto, se for feita uma tentativa para recuperar esses itens, um erro será retornado que afirma que o item não foi encontrado.
  
## <a name="getevents-request-example"></a>Exemplo de solicitação GetEvents

### <a name="description"></a>Descrição

O exemplo a seguir mostra como solicitar os eventos e os itens que estão associados uma assinatura que é identificada pela marca d'água e do identificador de inscrição.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetEvents xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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
    
## <a name="successful-getevents-response-example"></a>Exemplo de resposta bem-sucedida GetEvents

### <a name="description"></a>Descrição

O exemplo de uma resposta a seguir mostra uma notificação da existência de duas novas mensagens de email desde a última solicitação de notificação foi enviada para o servidor.
  
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
    <GetEventsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a>Comments

> [!NOTE]
> Os identificadores de item e pasta foram diminuídos para preservar a legibilidade. 
  
### <a name="getevents-response-elements"></a>Elementos de resposta GetEvents

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
    
- [Carimbo de hora](timestamp.md)
    
- [ItemId](itemid.md)
    
- [ParentFolderId](parentfolderid.md)
    
Para localizar outras opções para a mensagem de resposta da operação **GetEvents** , explore a hierarquia de esquema. Inicie o elemento de [notificação](notification-ex15websvcsotherref.md) . 
  
## <a name="getevents-error-response-example"></a>Exemplo de resposta de erro GetEvents

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta de erro a uma solicitação de **GetEvents** . 
  
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
    <GetEventsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

Ao processar uma solicitação de **GetEvents** , o servidor de acesso para cliente executa as seguintes etapas: 
  
1. A SubscriptionID da solicitação for confirmada seja uma assinatura válida que está hospedada no servidor de acesso para cliente. Se não for, a chamada **GetEvents** falha. 
    
2. O endereço SMTP do usuário autenticado para a solicitação é comparado com o endereço SMTP do usuário que criou a assinatura. Se eles não coincidirem, a solicitação de **GetEvents** falhará. 
    
3. A fila de inscrição é consultada para eventos que estão em espera a serem enviados para o cliente. Se a fila não está vazia, os 50 primeiros eventos da fila são retirados da fila e codificados em uma notificação.
    
4. Se nenhum evento forem encontrado na fila, um StatusEvent será gerado e codificado em uma resposta de notificação.
    
5. A resposta de notificação é retornada para o cliente.
    
6. Os eventos que estão incluídos na notificação são removidos da fila de inscrição e a acesso para cliente local última marca d'água server para a assinatura é definida como a marca d'água do último evento que é retornado.
    
7. O timer de tempo limite para a assinatura é redefinido.
    
## <a name="see-also"></a>Confira também



[Inscrever-se a operação](subscribe-operation.md)
  
[Cancelar a operação](unsubscribe-operation.md)


[Usando inscrições de recepção](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)

