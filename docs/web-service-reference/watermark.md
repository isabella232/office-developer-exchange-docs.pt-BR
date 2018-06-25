---
title: Marca d'água
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Watermark
api_type:
- schema
ms.assetid: e1545046-94f9-4ac7-af1c-ea81dfb6822c
description: O elemento de marca d'água representa um indicador de evento na fila de eventos de caixa de correio.
ms.openlocfilehash: 1867aa781bc24f5eb3bdb4648fa494a2a7ea396a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838047"
---
# <a name="watermark"></a>Marca d'água

O elemento de **marca d'água** representa um indicador de evento na fila de eventos de caixa de correio. 
  
```xml
<Watermark/>
```

 **WatermarkType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[PullSubscriptionRequest](pullsubscriptionrequest.md) <br/> |Representa uma assinatura para uma inscrição de notificação de evento baseado em extração.  <br/> |
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |Representa uma assinatura para uma inscrição de notificação de push com base no evento.  <br/> |
|[GetEvents](getevents.md) <br/> |Representa a operação usada pelos clientes de recepção para notificações de solicitação do servidor.  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |Representa um evento onde uma pasta ou um item é copiada.  <br/> |
|[CreatedEvent](createdevent.md) <br/> |Representa um evento onde uma pasta ou um item é criada.  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |Representa um evento onde uma pasta ou um item é excluída.  <br/> |
|[ModifiedEvent](modifiedevent.md) <br/> |Representa um evento onde um item ou pasta é modificada.  <br/> |
|[MovedEvent](movedevent.md) <br/> |Representa um evento onde uma pasta ou um item é movida da pasta pai de um para outra pasta pai.  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |Representa um evento disparado por um novo item de email em uma caixa de correio.  <br/> |
|[StatusEvent](statusevent.md) <br/> |Representa uma notificação que nenhuma nova atividade ocorreu na caixa de correio.  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação Subscribe.  <br/> |
   
## <a name="text-value"></a>Text value

Um valor de texto pode ser obrigatórias ou opcionais, dependendo de como esse elemento é usado.
  
## <a name="remarks"></a>Comentários

Se uma solicitação Subscribe contiver uma marca d'água, a assinatura é criada a partir de encaminhar a marca d'água. Se a solicitação Subscribe contiver uma marca d'água que não foi encontrada na tabela de eventos de caixa de correio, uma `ErrorInvalidWatermark` erro será retornado para o aplicativo cliente. Isso pode ocorrer se a marca d'água é muito antiga e foi removida da janela de 30 dias de tabela eventos ou se a marca d'água não estava nunca presentes na tabela eventos. Isso pode acontecer, por exemplo, se uma marca d'água é obtida de uma assinatura diferente para uma caixa de correio em um banco de dados diferente. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Inscrever-se a operação](subscribe-operation.md)
  
[Operação GetEvents](getevents-operation.md)
  
[Cancelar a operação](unsubscribe-operation.md)

