---
title: PullSubscriptionRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PullSubscriptionRequest
api_type:
- schema
ms.assetid: 145c5cc7-a894-4f0b-a6ea-358cddfb5c33
description: O elemento PullSubscriptionRequest representa uma assinatura para uma assinatura de notificação de eventos baseada em pull.
ms.openlocfilehash: fb9712c9e1481678c2821ee344052783d5c25bf9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468863"
---
# <a name="pullsubscriptionrequest"></a>PullSubscriptionRequest

O elemento **PullSubscriptionRequest** representa uma assinatura para uma assinatura de notificação de eventos baseada em pull. 
  
[Assinar](subscribe.md)
  
[PullSubscriptionRequest](pullsubscriptionrequest.md)
  
```XML
<PullSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
   <Watermark/>
   <Timeout/>
</PullSubscriptionRequest>
```

 **PullSubscriptionRequestType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**SubscribeToAllFolders** <br/> |Indica se é para se inscrever em todas as pastas disponíveis. Esse atributo é opcional.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderIds](folderids.md) <br/> |Contém uma matriz de identificadores de pasta que são usados para identificar as pastas a serem monitoradas para notificações de eventos.  <br/> |
|[EventType](eventtypes.md) <br/> |Contém uma coleção de notificações de eventos que são usadas para criar uma assinatura.  <br/> |
|[Marca d'água](watermark.md) <br/> |Representa um indicador de evento na tabela de eventos de caixa de correio. Isso é usado para criar uma assinatura que começa em um evento que é representado pela marca d' água. Se a marca d' água de uma solicitação de assinatura não for encontrada, uma resposta de erro será retornada ao cliente. Esse erro pode ocorrer se a marca d' água for mais antiga que 30 dias ou se a marca d' água nunca estiver presente na caixa de correio.  <br/> |
|[Timeout](timeout.md) <br/> |Representa a duração, em minutos, que a assinatura pode permanecer ociosa sem uma solicitação de GetEvents do cliente.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Assinar](subscribe.md) <br/> |Contém as propriedades que são usadas para criar assinaturas.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[PushSubscriptionRequest](pushsubscriptionrequest.md)
  
[Operação Subscribe](subscribe-operation.md)
  
[Operação GetEvents](getevents-operation.md)
  
[Cancelar a operação](unsubscribe-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

