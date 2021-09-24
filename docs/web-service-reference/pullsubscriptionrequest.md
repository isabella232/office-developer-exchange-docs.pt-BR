---
title: PullSubscriptionRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PullSubscriptionRequest
api_type:
- schema
ms.assetid: 145c5cc7-a894-4f0b-a6ea-358cddfb5c33
description: O elemento PullSubscriptionRequest representa uma assinatura de uma assinatura de notificação de evento baseada em pull.
ms.openlocfilehash: f1a527dff0c81262cac01a905293af1155acbf1c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540598"
---
# <a name="pullsubscriptionrequest"></a>PullSubscriptionRequest

O **elemento PullSubscriptionRequest** representa uma assinatura de uma assinatura de notificação de evento baseada em pull. 
  
[Subscribe](subscribe.md)
  
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
|**SubscribeToAllFolders** <br/> |Indica se você deve se inscrever em todas as pastas disponíveis. Esse atributo é opcional.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderIds](folderids.md) <br/> |Contém uma matriz de identificadores de pasta que são usados para identificar pastas para monitorar notificações de eventos.  <br/> |
|[EventTypes](eventtypes.md) <br/> |Contém uma coleção de notificações de eventos usadas para criar uma assinatura.  <br/> |
|[Watermark](watermark.md) <br/> |Representa um indicador de evento na tabela de eventos de caixa de correio. Isso é usado para criar uma assinatura que começa em um evento representado pela marca d'água. Se a marca d'água de uma solicitação Subscribe não for encontrada, uma resposta de erro será retornada ao cliente. Esse erro pode ocorrer se a marca d'água tiver mais de 30 dias ou se a marca d'água nunca estiver presente na caixa de correio.  <br/> |
|[Timeout](timeout.md) <br/> |Representa a duração, em minutos, de que a assinatura pode permanecer ociosa sem uma solicitação GetEvents do cliente.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Subscribe](subscribe.md) <br/> |Contém as propriedades usadas para criar assinaturas.  <br/> |
   
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

