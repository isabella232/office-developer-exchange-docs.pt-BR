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
description: O elemento PullSubscriptionRequest representa uma assinatura para uma inscrição de notificação de evento baseado em extração.
ms.openlocfilehash: 5f757bf1f79f7e2a00fb886db50e6ea0eaed1a4a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824932"
---
# <a name="pullsubscriptionrequest"></a>PullSubscriptionRequest

O elemento **PullSubscriptionRequest** representa uma assinatura para uma inscrição de notificação de evento baseado em extração. 
  
[Inscrever-se](subscribe.md)
  
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
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**SubscribeToAllFolders** <br/> |Indica se deve se inscrever para todas as pastas disponíveis. Este atributo é opcional.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderIds](folderids.md) <br/> |Contém uma matriz de identificadores de pasta que são usados para identificar pastas para monitorar as notificações de eventos.  <br/> |
|[EventTypes](eventtypes.md) <br/> |Contém uma coleção de notificações de eventos que são usados para criar uma assinatura.  <br/> |
|[Marca d'água](watermark.md) <br/> |Representa um indicador de evento na tabela de eventos de caixa de correio. Isso é usado para criar uma assinatura que inicia em um evento que é representado por marca d'água. Se a marca d'água de uma solicitação Subscribe não for encontrada, uma resposta de erro será retornada ao cliente. Esse erro pode ocorrer se a marca d'água tem mais de 30 dias ou se a marca d'água nunca estava presente na caixa de correio.  <br/> |
|[Timeout](timeout.md) <br/> |Representa a duração em minutos, que a assinatura pode permanecer inativa sem uma solicitação GetEvents do cliente.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Inscrever-se](subscribe.md) <br/> |Contém as propriedades que são usadas para criar assinaturas.  <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[PushSubscriptionRequest](pushsubscriptionrequest.md)
  
[Inscrever-se a operação](subscribe-operation.md)
  
[Operação GetEvents](getevents-operation.md)
  
[Cancelar a operação](unsubscribe-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

