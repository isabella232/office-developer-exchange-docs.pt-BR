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
description: O elemento PreviousWatermark representa a marca d'água do evento mais recente que foi comunicada com êxito para o cliente para a assinatura.
ms.openlocfilehash: 93c6f90d0866ae13618391b8544ab593fe33922b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824886"
---
# <a name="previouswatermark"></a>PreviousWatermark

O elemento **PreviousWatermark** representa a marca d'água do evento mais recente que foi comunicada com êxito para o cliente para a assinatura. 
  
```xml
<PreviousWatermark/>
```

 **WatermarkType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Notificação](notification-ex15websvcsotherref.md) <br/> |Contém informações sobre a inscrição e os eventos que ocorreram desde a última notificação.  <br/> |
   
## <a name="text-value"></a>Text value

É necessário um valor de texto. O valor de texto representa a marca d'água mais recente. O valor de texto não pode ser uma sequência vazia.
  
## <a name="remarks"></a>Coment�rios

A propriedade **PreviousWatermark** é útil para o cliente na determinação da última notificação bem-sucedida. Por exemplo, se uma assinatura tem três eventos com marcas d'água 1, 2 e 3 e a próxima notificação é enviada com um valor **PreviousWatermark** 3, o cliente pode comparar este valor como o valor de marca d'água da última notificação recebida. Isso permite que o cliente garantir a continuidade de eventos. 
  
Para clientes de push, o **PreviousWatermark** é comparado com a local, no lado do cliente última conhecida marca d'água. Se os valores forem diferentes, o cliente perdeu uma notificação de evento e deverá restabelecer uma inscrição usando a marca d'água local mais recente. Por exemplo, se um cliente de push recebe eventos de três para uma inscrição com marcas d'água 1, 2 e 3 e a próxima notificação vem com um valor **PreviousWatermark** 5, o cliente perdeu a notificação de pelo menos um e crie uma nova assinatura, passando um 3 como a marca d'água. 
  
No caso de um cliente de recepção, o valor de **PreviousWatermark** será o mesmo que a [marca d'água](watermark.md) incluídos pelo cliente na chamada GetEvents. 
  
O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Inscrever-se a operação](subscribe-operation.md)
  
[Operação GetEvents](getevents-operation.md)
  
[Cancelar a operação](unsubscribe-operation.md)

