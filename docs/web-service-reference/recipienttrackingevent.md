---
title: RecipientTrackingEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RecipientTrackingEvent
api_type:
- schema
ms.assetid: 2bffdac7-c2f5-4805-ae7e-bd865301acb6
description: O elemento RecipientTrackingEvent contém informações para um único evento para um destinatário.
ms.openlocfilehash: 30d9cd4ca075fda9607b191f576cac1b7a529988
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525760"
---
# <a name="recipienttrackingevent"></a>RecipientTrackingEvent

O **elemento RecipientTrackingEvent** contém informações para um único evento para um destinatário. 
  
```XML
<RecipientTrackingEvent>
   <Date/>
   <Recipient/>
   <DeliveryStatus/>
   <EventDescription/>
   <EventData/>
   <Server/>
   <InternalId/>
   <BccRecipient/>
   <HiddenRecipient/>
   <UniquePathId/>
   <RootAddress/>
   <Properties/>
</RecipientTrackingEvent>
```

 **RecipientTrackingEventType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Date (MessageTracking)](date-messagetracking.md) <br/> |Este elemento é obrigatório.  <br/> |
|[Recipiente](recipient.md) <br/> |Este elemento é obrigatório.  <br/> |
|[DeliveryStatus](deliverystatus.md) <br/> |Este elemento é obrigatório.  <br/> |
|[EventDescription](eventdescription.md) <br/> |Este elemento é obrigatório.  <br/> |
|[EventData](eventdata.md) <br/> |Esse elemento é opcional.  <br/> |
|[Server (MessageTracking)](server-messagetracking.md) <br/> |Este elemento é obrigatório.  <br/> |
|[InternalId](internalid.md) <br/> |Este elemento é obrigatório.  <br/> |
|[BccRecipient](bccrecipient.md) <br/> |Esse elemento é opcional.  <br/> |
|[HiddenRecipient](hiddenrecipient.md) <br/> |Esse elemento é opcional.  <br/> |
|[UniquePathId](uniquepathid.md) <br/> |Esse elemento é opcional.  <br/> |
|[RootAddress](rootaddress.md) <br/> |Esse elemento é opcional.  <br/> |
|[Properties (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |Esse elemento é opcional.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[RecipientTrackingEvents](recipienttrackingevents.md) <br/> |Contém uma lista de um ou mais eventos de controle para um destinatário.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetMessageTrackingReport](getmessagetrackingreport-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

