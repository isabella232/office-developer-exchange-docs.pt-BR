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
description: O elemento Watermark representa um indicador de evento na fila de eventos de caixa de correio.
ms.openlocfilehash: a717196101fea698b0b8c66f92a3d420fda9a421
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459760"
---
# <a name="watermark"></a>Marca d'água

O elemento **Watermark** representa um indicador de evento na fila de eventos de caixa de correio. 
  
```xml
<Watermark/>
```

 **Marca d' água**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[PullSubscriptionRequest](pullsubscriptionrequest.md) <br/> |Representa uma assinatura para uma assinatura de notificação de eventos baseada em pull.  <br/> |
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |Representa uma assinatura para uma assinatura de notificação de eventos baseada em push.  <br/> |
|[GetEvents](getevents.md) <br/> |Representa a operação usada por clientes de recebimento para solicitar notificações do servidor.  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |Representa um evento em que um item ou pasta é copiado.  <br/> |
|[CreatedEvent](createdevent.md) <br/> |Representa um evento em que um item ou pasta é criado.  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |Representa um evento em que um item ou pasta é excluído.  <br/> |
|[ModifiedEvent](modifiedevent.md) <br/> |Representa um evento em que um item ou pasta é modificado.  <br/> |
|[MovedEvent](movedevent.md) <br/> |Representa um evento em que um item ou pasta é movido de uma pasta pai para outra pasta pai.  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |Representa um evento disparado por um novo item de email em uma caixa de correio.  <br/> |
|[StatusEvent](statusevent.md) <br/> |Representa uma notificação de que nenhuma atividade nova ocorreu na caixa de correio.  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação de assinatura.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto pode ser obrigatório ou opcional, dependendo de como esse elemento é usado.
  
## <a name="remarks"></a>Comentários

Se uma solicitação de assinatura contiver uma marca d' água, a assinatura será criada a partir da marca d' água para frente. Se a solicitação de assinatura contiver uma marca d' água que não seja encontrada na tabela de eventos de caixa de correio, um `ErrorInvalidWatermark` erro será retornado para o aplicativo cliente. Isso pode ocorrer se a marca d' água for muito antiga e tiver sido removida da janela de 30 dias da tabela de eventos ou se a marca d' água ainda não estiver presente na tabela de eventos. Isso pode acontecer, por exemplo, se uma marca d' água for Obtida de uma assinatura diferente para uma caixa de correio em um banco de dados diferente. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação Subscribe](subscribe-operation.md)
  
[Operação GetEvents](getevents-operation.md)
  
[Cancelar a operação](unsubscribe-operation.md)

