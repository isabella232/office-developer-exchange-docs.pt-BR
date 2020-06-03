---
title: SubscriptionStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SubscriptionStatus
api_type:
- schema
ms.assetid: 2d64ebb7-f26a-4d02-b7ef-d9d7da75f0c3
description: O elemento SubscriptionStatus descreve o status de uma assinatura push.
ms.openlocfilehash: 195ab229380f4386b39e5c3fd48208cf66e224f0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530941"
---
# <a name="subscriptionstatus"></a>SubscriptionStatus

O elemento **SubscriptionStatus** descreve o status de uma assinatura push. 
  
```xml
<SubscriptionStatus>OK or Unsubscribe</SubscriptionStatus>
```

 **SubscriptionStatusType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SendNotificationResult](sendnotificationresult.md) <br/> |Contém a resposta do aplicativo cliente ' para uma notificação por push.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é obrigatório. Estes são os valores de texto possíveis para este elemento:
  
- OK
    
- Cancelar assinatura
    
## <a name="remarks"></a>Comentários

Este elemento descreve o status da assinatura. O aplicativo cliente de assinatura push envia o status de volta para o computador que está executando o Exchange 2007 que tem a função de servidor de acesso para Cliente instalada após cada notificação por push. Se o valor **SubscriptionStatus** for igual a **unsubscribe**, o servidor de acesso para cliente interromperá o envio de notificações e encerrará a assinatura. Se o valor **SubscriptionStatus** for igual a **OK**, o servidor de acesso para cliente continuará a enviar notificações.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

