---
title: StreamingSubscriptionRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StreamingSubscriptionRequest
api_type:
- schema
ms.assetid: d18f3b60-ebb6-4133-b895-a6ec8942d039
description: O elemento StreamingSubscriptionRequest representa uma assinatura para uma assinatura de notificação de eventos de streaming.
ms.openlocfilehash: b469ba7598420189c1db0e2fe676a279390eb6bf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468226"
---
# <a name="streamingsubscriptionrequest"></a>StreamingSubscriptionRequest

O elemento **StreamingSubscriptionRequest** representa uma assinatura para uma assinatura de notificação de eventos de streaming. 
  
[Assinar](subscribe.md)
  
[StreamingSubscriptionRequest](streamingsubscriptionrequest.md)
  
```xml
<StreamingSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
</StreamingSubscriptionRequest>
```

 **StreamingSubscriptionRequest**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**SubscribeToAllFolders** <br/> |Indica se o servidor se inscreverá em todas as pastas da caixa de correio do usuário. Um valor **true** indica que o servidor irá se inscrever.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderIds](folderids.md) <br/> |Contém uma matriz de identificadores de pasta que são usados para identificar as pastas a serem monitoradas para notificações de eventos.  <br/> |
|[EventType](eventtypes.md) <br/> |Contém uma coleção de notificações de eventos que são usadas para criar uma assinatura.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Assinar](subscribe.md) <br/> |Contém as propriedades que são usadas para criar assinaturas.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação Subscribe](subscribe-operation.md)
  
[Operação GetEvents](getevents-operation.md)
  
[Operação GetStreamingEvents](getstreamingevents-operation.md)
  
[Cancelar a operação](unsubscribe-operation.md)

