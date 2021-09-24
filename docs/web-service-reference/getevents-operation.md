---
title: Operação GetEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetEvents
api_type:
- schema
ms.assetid: f268efe5-9a1a-41a2-b6a6-51fcde7720a1
description: A operação GetEvents é usada por clientes de assinatura pull para solicitar notificações do servidor de Acesso para Cliente. A resposta da operação GetEvents retorna uma matriz de itens e eventos que ocorreram em uma caixa de correio desde a última notificação.
ms.openlocfilehash: 72d99a654921794115d56d28327a39a21c9ea378
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511597"
---
# <a name="getevents-operation"></a>Operação GetEvents

A **operação GetEvents** é usada por clientes de assinatura pull para solicitar notificações do servidor de Acesso para Cliente. A **resposta da operação GetEvents** retorna uma matriz de itens e eventos que ocorreram em uma caixa de correio desde a última notificação. 
  
> [!IMPORTANT]
> A **operação DeleteUserConfiguration** disparará um evento de movimentação para o sistema de notificação de eventos. O objeto de configuração do usuário será movido para a lixeira. 
  
## <a name="notes"></a>Observações

Alterações nos itens calendário podem resultar na geração de vários eventos. Esses eventos são o resultado de itens temporários que estão sendo criados na caixa de correio, itens de armazenamento de dados de livre/ocupado sendo alterados como parte das operações normais do Calendário ou ambos. Eventos da classe de item "IPM. SchedulePlus.FreeBusy.BinaryData" deve ser ignorado pelos clientes de serviço Web. Esses itens temporários são excluídos após a criação; portanto, se uma tentativa for feita para recuperar esses itens, um erro será retornado informando que o item não foi encontrado.
  
## <a name="getevents-request-example"></a>Exemplo de solicitação GetEvents

### <a name="description"></a>Descrição

O exemplo a seguir mostra como solicitar os eventos e itens associados a uma assinatura identificada pelo identificador de assinatura e marca d'água.
  
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
    
- [Watermark](watermark.md)
    
## <a name="successful-getevents-response-example"></a>Exemplo de resposta GetEvents bem-sucedida

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
> Os identificadores de item e pasta foram reduzidos para preservar a capacidade de leitura. 
  
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
    
- [Watermark](watermark.md)
    
- [TimeStamp](timestamp.md)
    
- [ItemId](itemid.md)
    
- [ParentFolderId](parentfolderid.md)
    
Para encontrar outras opções para a mensagem de resposta da **operação GetEvents,** explore a hierarquia de esquema. Comece no [elemento Notification.](notification-ex15websvcsotherref.md) 
  
## <a name="getevents-error-response-example"></a>Exemplo de resposta de erro GetEvents

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta de erro a uma **solicitação GetEvents.** 
  
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

Ao processar uma **solicitação GetEvents,** o servidor de Acesso para Cliente executa as seguintes etapas: 
  
1. O SubscriptionID da solicitação é confirmado como uma assinatura válida hospedada no servidor de Acesso para Cliente. Se não estiver, a **chamada GetEvents** falhará. 
    
2. O endereço SMTP do usuário autenticado para a solicitação é comparado ao endereço SMTP do usuário que criou a assinatura. Se eles não corresponderem, a **solicitação GetEvents** falhará. 
    
3. A fila de assinaturas é consultada para eventos que estão aguardando serem enviados para o cliente. Se a fila não estiver vazia, os primeiros 50 eventos da fila serão retirados da fila e codificados em uma notificação.
    
4. Se nenhum evento for encontrado na fila, um StatusEvent será gerado e codificado em uma resposta de notificação.
    
5. A resposta de notificação é retornada ao cliente.
    
6. Os eventos incluídos na notificação são removidos da fila de assinatura e a última marca d'água local do servidor de Acesso para Cliente para a assinatura é definida como a marca d'água do último evento retornado.
    
7. O temporizador de tempo de tempo para a assinatura é redefinido.
    
## <a name="see-also"></a>Confira também



[Operação Subscribe](subscribe-operation.md)
  
[Operação de cancelamento de assinatura](unsubscribe-operation.md)


[Usando Assinaturas Pull](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)

