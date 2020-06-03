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
ms.openlocfilehash: 5f61a4eea945193d672afbcd2c693502ccf3e4e1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530632"
---
# <a name="eventdescription"></a>EventDescription

O elemento **EventDescription** 
  
```xml
<EventDescription/>
```

 **MessageTrackingEventDescriptionType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[RecipientTrackingEvent](recipienttrackingevent.md) <br/> ||
   
## <a name="text-value"></a>Valor de texto

A tabela a seguir lista os valores possíveis para o elemento **EventDescription** . 
  
**Valores do elemento EventDescription**

|**Valor**|**Descrição**|
|:-----|:-----|
|Submitted  <br/> ||
|Resolvido  <br/> ||
|Expandido  <br/> ||
|Gerados  <br/> ||
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
|Pending  <br/> ||
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
|Não lido  <br/> ||
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

