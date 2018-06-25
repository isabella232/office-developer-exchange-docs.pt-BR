---
title: RecipientTrackingEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecipientTrackingEvent
api_type:
- schema
ms.assetid: 2bffdac7-c2f5-4805-ae7e-bd865301acb6
description: O elemento RecipientTrackingEvent contém informações para um único evento de um destinatário.
ms.openlocfilehash: c5488ba105f9a853a490d6f0f4ff9ff15b537e23
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824989"
---
# <a name="recipienttrackingevent"></a>RecipientTrackingEvent

O elemento **RecipientTrackingEvent** contém informações para um único evento de um destinatário. 
  
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
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Data (MessageTracking)](date-messagetracking.md) <br/> |Este elemento é obrigatório.  <br/> |
|[Recipient](recipient.md) <br/> |Este elemento é obrigatório.  <br/> |
|[DeliveryStatus](deliverystatus.md) <br/> |Este elemento é obrigatório.  <br/> |
|[EventDescription](eventdescription.md) <br/> |Este elemento é obrigatório.  <br/> |
|[EventData](eventdata.md) <br/> |Esse elemento é opcional.  <br/> |
|[Servidor (MessageTracking)](server-messagetracking.md) <br/> |Este elemento é obrigatório.  <br/> |
|[InternalId](internalid.md) <br/> |Este elemento é obrigatório.  <br/> |
|[BccRecipient](bccrecipient.md) <br/> |Esse elemento é opcional.  <br/> |
|[HiddenRecipient](hiddenrecipient.md) <br/> |Esse elemento é opcional.  <br/> |
|[UniquePathId](uniquepathid.md) <br/> |Esse elemento é opcional.  <br/> |
|[RootAddress](rootaddress.md) <br/> |Esse elemento é opcional.  <br/> |
|[Propriedades (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |Esse elemento é opcional.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[RecipientTrackingEvents](recipienttrackingevents.md) <br/> |Contém uma lista de um ou mais eventos de rastreamento para um destinatário.  <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação GetMessageTrackingReport](getmessagetrackingreport-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

