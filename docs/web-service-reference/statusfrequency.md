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
description: O elemento StatusFrequency representa o valor de tempo limite máximo, em minutos, em que as tentativas são tentadas pelo servidor.
ms.openlocfilehash: db14ecfd54584188b3da16bb369db6c8089c70f4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468240"
---
# <a name="statusfrequency"></a>StatusFrequency

O elemento **StatusFrequency** representa o valor de tempo limite máximo, em minutos, em que as tentativas são tentadas pelo servidor. 
  
[Assinar](subscribe.md)
  
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
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |Representa uma assinatura para uma assinatura de notificação de eventos baseada em push.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto que representa um inteiro será necessário se esse elemento for usado. Os valores possíveis para esse elemento são 1 a 1440, inclusive. Este elemento é opcional. O valor-padrão é 30 minutos.
  
## <a name="remarks"></a>Comentários

O valor **StatusFrequency** é usado pelo servidor para repetir uma notificação por push quando não recebe uma resposta para uma notificação por Push ou o status ping do cliente. Se o servidor não receber uma resposta, ele tentará enviar a notificação várias vezes antes de parar de enviar a notificação. No EWS, o intervalo de repetição padrão é de 30 segundos e as novas tentativas subsequentes sempre têm o dobro da hora do último intervalo de repetição. Horários de tentativas não são exatos, já que podem ser atrasados devido a outras cargas no servidor. A tabela a seguir mostra como os intervalos de repetição ocorrem nos 30 minutos alocados pelo valor padrão do **StatusFrequency** (supondo que o servidor não encontrou atrasos). 
  
|repetir|**Segundos**|**Time**|
|:-----|:-----|:-----|
|,0  <br/> |,0  <br/> |Sincronização inicial  <br/> |
|1   <br/> |até  <br/> |00:30  <br/> |
|duas  <br/> |60  <br/> |01:00  <br/> |
|3D  <br/> |120  <br/> |02:00  <br/> |
|4   <br/> |240  <br/> |04:00  <br/> |
|5   <br/> |480  <br/> |08:00  <br/> |
|6   <br/> |960  <br/> |16:00  <br/> |
|7   <br/> |1920  <br/> |32:00- **StatusFrequency** valor padrão de 30 excedido, repetir não enviado  <br/> |
   
Se o cliente não receber mensagens de notificação do servidor por um período de tempo que exceder o tempo especificado por **StatusFrequency**, o cliente deverá executar uma ação, como recriar a assinatura. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação Subscribe](subscribe-operation.md)
  
[Operação GetEvents](getevents-operation.md)
  
[Cancelar a operação](unsubscribe-operation.md)
  
[Marca d'água](watermark.md)

