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
description: O elemento PushSubscriptionRequest representa uma assinatura para uma assinatura de notificação de eventos baseada em push.
ms.openlocfilehash: dcdb767ed175468aa4ec940f3147c164e4707e40
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465510"
---
# <a name="pushsubscriptionrequest"></a>PushSubscriptionRequest

O elemento **PushSubscriptionRequest** representa uma assinatura para uma assinatura de notificação de eventos baseada em push. 
  
[Assinar](subscribe.md)
  
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
|[Marca d'água](watermark.md) <br/> |Representa um indicador de evento na tabela de eventos de caixa de correio. Isso é usado para criar uma assinatura começando em um evento representado pela marca d' água. Se a marca d' água de uma solicitação de assinatura não for encontrada, uma resposta de erro será retornada ao cliente. Isso pode ocorrer se a marca d' água for mais antiga que 30 dias ou se a marca d' água nunca estiver presente na caixa de correio.  <br/> |
|[StatusFrequency](statusfrequency.md) <br/> |Representa a frequência, especificada em minutos, em que as mensagens de notificação serão enviadas ao cliente quando nenhum evento tiver ocorrido.  <br/> |
|[Endereço](url-ex15websvcsotherref.md) <br/> |Representa o local do serviço Web cliente para notificações por push.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Assinar](subscribe.md) <br/> |Contém as propriedades usadas para criar assinaturas.  <br/> |
   
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



[Operação Subscribe](subscribe-operation.md)
  
[Operação GetEvents](getevents-operation.md)
  
[Cancelar a operação](unsubscribe-operation.md)

