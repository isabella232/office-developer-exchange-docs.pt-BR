---
title: EventDescription
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EventDescription
api_type:
- schema
ms.assetid: 7642cb03-71b1-4773-9508-4fbe3a5dcdf4
description: O elemento EventDescription
ms.openlocfilehash: d496e6d2a61b4a72954b25fe3c5362f82aabf143
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752108"
---
# <a name="eventdescription"></a>EventDescription

O elemento **EventDescription** 
  
```xml
<EventDescription/>
```

 **MessageTrackingEventDescriptionType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[RecipientTrackingEvent](recipienttrackingevent.md) <br/> ||
   
## <a name="text-value"></a>Text value

A tabela a seguir lista os valores possíveis para o elemento **EventDescription** . 
  
**Valores de elemento EventDescription**

|**Valor**|**Descrição**|
|:-----|:-----|
|Enviado  <br/> ||
|Resolvido  <br/> ||
|Expandida  <br/> ||
|Entregue  <br/> ||
|MovedToFolderByInboxRule  <br/> ||
|RulesCc  <br/> ||
|FailedGeneral  <br/> ||
|FailedModeration  <br/> ||
|FailedTransportRules  <br/> ||
|SmtpSend  <br/> ||
|SmtpSendCrossSite  <br/> ||
|SmtpSendCrossForest  <br/> ||
|SmtpReceive  <br/> ||
|Encaminhadas  <br/> ||
|Pendente  <br/> ||
|PendingModeration  <br/> ||
|ApprovedModeration  <br/> ||
|QueueRetry  <br/> ||
|QueueRetryNoRetryTime  <br/> ||
|MessageDefer  <br/> ||
|TransferredToForeignOrg  <br/> ||
|TransferredToPartnerOrg  <br/> ||
|TransferredToLegacyExchangeServer  <br/> ||
|DelayedAfterTransferToPartnerOrg  <br/> ||
|Ler  <br/> ||
|NotRead  <br/> ||
   
## <a name="remarks"></a>Coment�rios

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

