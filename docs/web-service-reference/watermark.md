---
title: Watermark
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Watermark
api_type:
- schema
ms.assetid: e1545046-94f9-4ac7-af1c-ea81dfb6822c
description: O elemento Watermark representa um indicador de evento na fila de eventos da caixa de correio.
ms.openlocfilehash: 959ae7369195a164d257b8805a8c985f1fdca53b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524396"
---
# <a name="watermark"></a>Watermark

O **elemento Watermark** representa um indicador de evento na fila de eventos da caixa de correio. 
  
```xml
<Watermark/>
```

 **WatermarkType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[PullSubscriptionRequest](pullsubscriptionrequest.md) <br/> |Representa uma assinatura de uma assinatura de notificação de evento baseada em pull.  <br/> |
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |Representa uma assinatura de uma assinatura de notificação de evento baseada em push.  <br/> |
|[GetEvents](getevents.md) <br/> |Representa a operação usada por clientes pull para solicitar notificações do servidor.  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |Representa um evento em que um item ou pasta é copiado.  <br/> |
|[CreatedEvent](createdevent.md) <br/> |Representa um evento em que um item ou pasta é criado.  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |Representa um evento em que um item ou pasta é excluído.  <br/> |
|[ModifiedEvent](modifiedevent.md) <br/> |Representa um evento em que um item ou pasta é modificado.  <br/> |
|[MovedEvent](movedevent.md) <br/> |Representa um evento em que um item ou pasta é movido de uma pasta pai para outra pasta pai.  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |Representa um evento disparado por um novo item de email em uma caixa de correio.  <br/> |
|[StatusEvent](statusevent.md) <br/> |Representa uma notificação de que nenhuma nova atividade ocorreu na caixa de correio.  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação Descrever.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto pode ser obrigatório ou opcional, dependendo de como esse elemento é usado.
  
## <a name="remarks"></a>Comentários

Se uma solicitação Subscribe contiver uma marca d'água, a assinatura será criada a partir da marca d'água para frente. Se a solicitação Subscribe contiver uma marca d'água que não é encontrada na tabela de eventos de caixa de correio, um erro  `ErrorInvalidWatermark` será retornado ao aplicativo cliente. Isso pode ocorrer se a marca d'água for muito antiga e tiver sido removida da janela de 30 dias da tabela de eventos ou se a marca d'água nunca estiver presente na tabela de eventos. Isso pode acontecer, por exemplo, se uma marca d'água for obtida de uma assinatura diferente para uma caixa de correio em um banco de dados diferente. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação Subscribe](subscribe-operation.md)
  
[Operação GetEvents](getevents-operation.md)
  
[Cancelar a operação](unsubscribe-operation.md)

