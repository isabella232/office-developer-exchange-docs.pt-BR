---
title: StreamingSubscriptionRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- StreamingSubscriptionRequest
api_type:
- schema
ms.assetid: d18f3b60-ebb6-4133-b895-a6ec8942d039
description: O elemento StreamingSubscriptionRequest representa uma assinatura de uma assinatura de notificação de evento de streaming.
ms.openlocfilehash: 9789329f3f59cb543861dca0232207669f0711b8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544546"
---
# <a name="streamingsubscriptionrequest"></a>StreamingSubscriptionRequest

O **elemento StreamingSubscriptionRequest** representa uma assinatura de uma assinatura de notificação de evento de streaming. 
  
[Subscribe](subscribe.md)
  
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
|**SubscribeToAllFolders** <br/> |Indica se o servidor assinará todas as pastas na caixa de correio do usuário. Um valor **true** indica que o servidor assinará.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderIds](folderids.md) <br/> |Contém uma matriz de identificadores de pasta que são usados para identificar pastas para monitorar notificações de eventos.  <br/> |
|[EventTypes](eventtypes.md) <br/> |Contém uma coleção de notificações de eventos usadas para criar uma assinatura.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Subscribe](subscribe.md) <br/> |Contém as propriedades usadas para criar assinaturas.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services. Esse elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
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

