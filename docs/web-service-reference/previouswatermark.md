---
title: PreviousWatermark
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PreviousWatermark
api_type:
- schema
ms.assetid: 474f4f7c-47da-47d4-8126-230012172fb5
description: O elemento PreviousWatermark representa a marca d'água do evento mais recente que foi comunicado com êxito ao cliente para a assinatura.
ms.openlocfilehash: c46e18c7a58405fe2149666531cb2af773110816
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543020"
---
# <a name="previouswatermark"></a>PreviousWatermark

O **elemento PreviousWatermark** representa a marca d'água do evento mais recente que foi comunicado com êxito ao cliente para a assinatura. 
  
```xml
<PreviousWatermark/>
```

 **WatermarkType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Notificação](notification-ex15websvcsotherref.md) <br/> |Contém informações sobre a assinatura e os eventos que ocorreram desde a última notificação.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é necessário. O valor do texto representa a marca d'água mais recente. O valor do texto não pode ser uma cadeia de caracteres vazia.
  
## <a name="remarks"></a>Comentários

A **propriedade PreviousWatermark** é útil para o cliente na determinação da última notificação bem-sucedida. Por exemplo, se uma assinatura tiver três eventos com marcas d'água 1, 2 e 3, e a próxima notificação for enviada com um **valor PreviousWatermark** de 3, o cliente poderá comparar esse valor com o valor Watermark da última notificação recebida. Isso permite que o cliente garanta a continuidade dos eventos. 
  
Para clientes push, **PreviousWatermark** é comparado com a última marca d'água conhecida do lado do cliente local. Se os valores são diferentes, o cliente perdeu uma notificação de evento e deve restabelecer uma assinatura usando a marca d'água local mais recente. Por exemplo, se um cliente de push recebe três eventos para uma assinatura com marcas d'água 1, 2 e 3, e a próxima notificação vem com um **valor PreviousWatermark** de 5, o cliente perdeu pelo menos uma notificação e deve criar uma nova assinatura, passando um 3 como marca d'água. 
  
No caso de um cliente pull, o valor **de PreviousWatermark** será o mesmo que o [Watermark](watermark.md) incluído pelo cliente na chamada GetEvents. 
  
O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação Subscribe](subscribe-operation.md)
  
[Operação GetEvents](getevents-operation.md)
  
[Cancelar a operação](unsubscribe-operation.md)

