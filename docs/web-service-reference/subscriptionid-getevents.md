---
title: SubscriptionId (GetEvents)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SubscriptionId
api_type:
- schema
ms.assetid: 77c0abab-69e8-428e-8c20-22258e4ef71b
description: O elemento SubscriptionId representa o identificador de uma assinatura.
ms.openlocfilehash: 8867b7da7c75cfd9d41f708c0481627d5186cc14
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825622"
---
# <a name="subscriptionid-getevents"></a>SubscriptionId (GetEvents)

O elemento **SubscriptionId** representa o identificador de uma assinatura. 
  
```xml
<SubscriptionId/>
```

 **SubscriptionIdType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetEvents](getevents.md) <br/> |Representa a operação usada pelos clientes de recepção para notificações de solicitação do servidor.  <br/> |
|[Notificação](notification-ex15websvcsotherref.md) <br/> |Contém informações sobre a inscrição e os eventos que ocorreram desde a última notificação.  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Contém o status e o resultado de uma solicitação Subscribe.  <br/> |
|[Cancelar assinatura](unsubscribe.md) <br/> |Contém as propriedades usadas para cancelar a assinatura de uma assinatura.  <br/> |
   
## <a name="text-value"></a>Text value

É necessário um valor de texto. O valor de texto é um GUID.
  
## <a name="remarks"></a>Coment�rios

O GUID que representa o identificador de inscrição é gerado pelo servidor de acesso para cliente quando a assinatura é criada.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |messages.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Inscrever-se a operação](subscribe-operation.md)
  
[Operação GetEvents](getevents-operation.md)
  
[Cancelar a operação](unsubscribe-operation.md)

