---
title: Tempo limite
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Timeout
api_type:
- schema
ms.assetid: c2e1ca5a-6667-4f6f-aac4-89de33bddc54
description: O elemento Timeout representa a duração, em minutos, de que a assinatura pode permanecer ociosa sem uma solicitação GetEvents do cliente.
ms.openlocfilehash: d0b5945f5d116e0ebb7a24a23970e785761fb0c9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59534164"
---
# <a name="timeout"></a>Tempo limite

O **elemento Timeout** representa a duração, em minutos, de que a assinatura pode permanecer ociosa sem uma solicitação GetEvents do cliente. 
  
```xml
<Timeout/>
```

 **int**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[PullSubscriptionRequest](pullsubscriptionrequest.md) <br/> |Representa uma assinatura de uma assinatura de notificação de evento baseada em pull.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto que representa um inteiro será necessário se esse elemento for usado. Os valores possíveis para esse elemento são de 1 a 1440, inclusive. Este elemento é obrigatório.
  
## <a name="remarks"></a>Comentários

O temporizador de tempo de tempo para a assinatura é redefinido por uma solicitação GetEvents bem-sucedida.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente. 
  
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

