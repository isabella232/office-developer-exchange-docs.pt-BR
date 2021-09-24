---
title: StatusFrequency
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- StatusFrequency
api_type:
- schema
ms.assetid: 917474e2-a426-4166-b825-53783a41dad4
description: O elemento StatusFrequency representa o valor máximo de tempo limite, em minutos, no qual tentativas são tentadas pelo servidor.
ms.openlocfilehash: f0359bab58167bbe7be5cce8c250240bebc7cc08
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525530"
---
# <a name="statusfrequency"></a>StatusFrequency

O **elemento StatusFrequency** representa o valor máximo de tempo limite, em minutos, no qual tentativas são tentadas pelo servidor. 
  
[Subscribe](subscribe.md)
  
[PushSubscriptionRequest](pushsubscriptionrequest.md)
  
[StatusFrequency](statusfrequency.md)
  
```XML
<StatusFrequency/>
```

 **SubscriptionStatusFrequencyType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |Representa uma assinatura de uma assinatura de notificação de evento baseada em push.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto que representa um inteiro será necessário se esse elemento for usado. Os valores possíveis para esse elemento são de 1 a 1440, inclusive. Esse elemento é opcional. O valor-padrão é 30 minutos.
  
## <a name="remarks"></a>Comentários

O **valor StatusFrequency** é usado pelo servidor para repetir uma notificação por push quando ele não recebe uma resposta a uma notificação por push ou ping de status do cliente. Se o servidor não receber uma resposta, ele recupera o envio da notificação várias vezes antes de parar de enviar a notificação. No EWS, o intervalo de repetir padrão é de 30 segundos e as recuperações subsequentes são sempre o dobro do tempo do último intervalo de tentativa. Os tempos de tentativa não são exatos, pois podem ser adiados devido a outras cargas no servidor. A tabela a seguir mostra como os intervalos de nova tentativa ocorrem nos 30 minutos alocados pelo valor **padrão StatusFrequency** (supondo que o servidor não encontrou nenhum atraso). 
  
|repetir|**Segundos**|**Time**|
|:-----|:-----|:-----|
|0  <br/> |0  <br/> |Sincronização inicial  <br/> |
|1  <br/> |30  <br/> |00:30  <br/> |
|2  <br/> |60  <br/> |01:00  <br/> |
|3  <br/> |120  <br/> |02:00  <br/> |
|4   <br/> |240  <br/> |04:00  <br/> |
|5  <br/> |480  <br/> |08:00  <br/> |
|6   <br/> |960  <br/> |16:00  <br/> |
|7   <br/> |1920  <br/> |32:00 - Valor padrão **statusFrequency** de 30 excedido, repetir não enviado  <br/> |
   
Se o cliente não receber mensagens de notificação do servidor por um período de tempo que exceda o dobro do tempo especificado por **StatusFrequency,** o cliente deverá tomar uma ação como recriar a assinatura. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação Subscribe](subscribe-operation.md)
  
[Operação GetEvents](getevents-operation.md)
  
[Cancelar a operação](unsubscribe-operation.md)
  
[Watermark](watermark.md)

