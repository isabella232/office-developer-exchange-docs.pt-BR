---
title: PushSubscriptionRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PushSubscriptionRequest
api_type:
- schema
ms.assetid: 70caa0ca-40a1-421f-b4e6-0658f22d0b8e
description: O elemento PushSubscriptionRequest representa uma assinatura para uma inscrição de notificação de push com base no evento.
ms.openlocfilehash: 34717d37b8e5bb50c927e57088299fbcb18a2514
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824929"
---
# <a name="pushsubscriptionrequest"></a>PushSubscriptionRequest

O elemento **PushSubscriptionRequest** representa uma assinatura para uma inscrição de notificação de push com base no evento. 
  
[Inscrever-se](subscribe.md)
  
[PushSubscriptionRequest](pushsubscriptionrequest.md)
  
```XML
<PushSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
   <Watermark/>
   <StatusFrequency/>
   <URL/>
</PushSubscriptionRequest>
```

 **PushSubscriptionRequestType**
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
|[Marca d'água](watermark.md) <br/> |Representa um indicador de evento na tabela de eventos de caixa de correio. Isso é usado para criar uma assinatura começando um evento representado por marca d'água. Se a marca d'água de uma solicitação Subscribe não for encontrada, uma resposta de erro será retornada ao cliente. Isso poderá ocorrer se a marca d'água tem mais de 30 dias ou se a marca d'água nunca estava presente na caixa de correio.  <br/> |
|[StatusFrequency](statusfrequency.md) <br/> |Representa a frequência, especificada em minutos, na qual notificação mensagens serão enviadas para o cliente quando nenhum evento ocorreu.  <br/> |
|[URL](url-ex15websvcsotherref.md) <br/> |Representa o local do cliente do serviço Web para notificações de push.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Inscrever-se](subscribe.md) <br/> |Contém as propriedades usadas para criar inscrições.  <br/> |
   
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



[Inscrever-se a operação](subscribe-operation.md)
  
[Operação GetEvents](getevents-operation.md)
  
[Cancelar a operação](unsubscribe-operation.md)

