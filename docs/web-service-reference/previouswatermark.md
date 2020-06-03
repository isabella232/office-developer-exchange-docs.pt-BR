---
title: PreviousWatermark
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PreviousWatermark
api_type:
- schema
ms.assetid: 474f4f7c-47da-47d4-8126-230012172fb5
description: O elemento PreviousWatermark representa a marca d' água do último evento que foi comunicado com êxito ao cliente para a assinatura.
ms.openlocfilehash: 1b26a645a5ec6dbbd2874b118f968866aadc32af
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461650"
---
# <a name="previouswatermark"></a>PreviousWatermark

O elemento **PreviousWatermark** representa a marca d' água do último evento que foi comunicado com êxito ao cliente para a assinatura. 
  
```xml
<PreviousWatermark/>
```

 **Marca d' água**
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

Um valor de texto é obrigatório. O valor de texto representa a marca d' água mais recente. O valor de texto não pode ser uma cadeia de caracteres vazia.
  
## <a name="remarks"></a>Comentários

A propriedade **PreviousWatermark** é útil para o cliente para determinar a última notificação bem-sucedida. Por exemplo, se uma assinatura tem três eventos com marcas d' água 1, 2 e 3 e a próxima notificação é enviada com um valor de **PreviousWatermark** de 3, o cliente pode comparar esse valor ao valor da marca d' água da última notificação recebida. Isso permite ao cliente garantir a continuidade de eventos. 
  
Para clientes de envio, o **PreviousWatermark** é comparado com a marca d' água local, da última chamada do cliente. Se os valores forem diferentes, o cliente perdeu uma notificação de evento e deve restabelecer uma assinatura usando a marca d' água local mais recente. Por exemplo, se um cliente de envio receber três eventos para uma assinatura com marcas d' água 1, 2 e 3 e a próxima notificação vier com um valor de 5 **PreviousWatermark** , o cliente perderá pelo menos uma notificação e deverá criar uma nova assinatura, passando um 3 como a marca d' água. 
  
No caso de um cliente de recebimento, o valor de **PreviousWatermark** será o mesmo que a [marca d' água](watermark.md) incluída pelo cliente na chamada GetEvents. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação Subscribe](subscribe-operation.md)
  
[Operação GetEvents](getevents-operation.md)
  
[Cancelar a operação](unsubscribe-operation.md)

