---
title: StatusFrequency
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StatusFrequency
api_type:
- schema
ms.assetid: 917474e2-a426-4166-b825-53783a41dad4
description: O elemento StatusFrequency representa o valor de tempo limite máximo, em minutos, no qual as repetições são tentadas pelo servidor.
ms.openlocfilehash: 402f8978c0ec6b377dfa020f23595c8954509a07
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825589"
---
# <a name="statusfrequency"></a>StatusFrequency

O elemento **StatusFrequency** representa o valor de tempo limite máximo, em minutos, no qual as repetições são tentadas pelo servidor. 
  
[Inscrever-se](subscribe.md)
  
[PushSubscriptionRequest](pushsubscriptionrequest.md)
  
[StatusFrequency](statusfrequency.md)
  
```XML
<StatusFrequency/>
```

 **SubscriptionStatusFrequencyType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |Representa uma assinatura para uma inscrição de notificação de push com base no evento.  <br/> |
   
## <a name="text-value"></a>Text value

Se este elemento for usado, será necessário um valor de texto que representa um número inteiro. Os valores possíveis para esse elemento são de 1 a 1440, inclusive. Esse elemento é opcional. O valor padrão é 30 minutos.
  
## <a name="remarks"></a>Comentários

O valor de **StatusFrequency** é usado pelo servidor para repetir uma notificação de push quando ele não recebe uma resposta a uma notificação de push ou ping de status do cliente. Se o servidor não recebe uma resposta, ele repete enviando a notificação várias vezes, antes de parar enviar a notificação. No EWS, o intervalo de repetição padrão é 30 segundos e tentativas subsequentes são sempre double a hora do último intervalo de repetição. Número de repetições não é exato, pois eles podem ser atrasados devido aos outros carregamentos no servidor. A tabela a seguir mostra como os intervalos de repetição ocorrerem nos 30 minutos alocados pelo valor **StatusFrequency** padrão (supondo que o servidor não o encontrou qualquer atrasos). 
  
|**Retry**|**Segundos**|**Time**|
|:-----|:-----|:-----|
|0  <br/> |0  <br/> |Sincronização inicial  <br/> |
|1  <br/> |30  <br/> |00:30  <br/> |
|2  <br/> |60  <br/> |01:00  <br/> |
|3  <br/> |120  <br/> |02:00  <br/> |
|4  <br/> |240  <br/> |04:00  <br/> |
|5  <br/> |480  <br/> |08:00  <br/> |
|6  <br/> |960  <br/> |16:00  <br/> |
|7  <br/> |1920  <br/> |32:00 - o valor padrão de **StatusFrequency** de 30 excedido, repetir não enviado  <br/> |
   
Se o cliente não receber mensagens de notificação do servidor por um período de tempo que excede o dobro do tempo especificado pela **StatusFrequency**, o cliente deve executar uma ação, como recriar a assinatura. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Inscrever-se a operação](subscribe-operation.md)
  
[Operação GetEvents](getevents-operation.md)
  
[Cancelar a operação](unsubscribe-operation.md)
  
[Marca d'água](watermark.md)

