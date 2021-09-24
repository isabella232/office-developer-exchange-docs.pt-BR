---
title: PushSubscriptionRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PushSubscriptionRequest
api_type:
- schema
ms.assetid: 70caa0ca-40a1-421f-b4e6-0658f22d0b8e
description: O elemento PushSubscriptionRequest representa uma assinatura de uma assinatura de notificação de evento baseada em push.
ms.openlocfilehash: 6eb76bba92e78e048ae97dbec5fc6c4d698a815f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523724"
---
# <a name="pushsubscriptionrequest"></a>PushSubscriptionRequest

O **elemento PushSubscriptionRequest** representa uma assinatura de uma assinatura de notificação de evento baseada em push. 
  
[Subscribe](subscribe.md)
  
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
|**SubscribeToAllFolders** <br/> |Indica se você deve se inscrever em todas as pastas disponíveis. Esse atributo é opcional.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderIds](folderids.md) <br/> |Contém uma matriz de identificadores de pasta que são usados para identificar pastas para monitorar notificações de eventos.  <br/> |
|[EventTypes](eventtypes.md) <br/> |Contém uma coleção de notificações de eventos usadas para criar uma assinatura.  <br/> |
|[Watermark](watermark.md) <br/> |Representa um indicador de evento na tabela de eventos de caixa de correio. Isso é usado para criar uma assinatura a partir de um evento representado pela marca d'água. Se a marca d'água de uma solicitação Subscribe não for encontrada, uma resposta de erro será retornada ao cliente. Isso pode ocorrer se a marca d'água tiver mais de 30 dias ou se a marca d'água nunca estiver presente na caixa de correio.  <br/> |
|[StatusFrequency](statusfrequency.md) <br/> |Representa a frequência, especificada em minutos, na qual as mensagens de notificação serão enviadas ao cliente quando nenhum evento tiver ocorrido.  <br/> |
|[Url ](url-ex15websvcsotherref.md) <br/> |Representa o local do serviço Web do cliente para notificações por push.  <br/> |
   
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



[Operação Subscribe](subscribe-operation.md)
  
[Operação GetEvents](getevents-operation.md)
  
[Cancelar a operação](unsubscribe-operation.md)

