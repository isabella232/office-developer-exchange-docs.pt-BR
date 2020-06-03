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
description: O elemento RecipientTrackingEvent contém informações de um único evento para um destinatário.
ms.openlocfilehash: e9a014cdfac122f112205cfa5032535a770f9d82
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465482"
---
# <a name="recipienttrackingevent"></a>RecipientTrackingEvent

O elemento **RecipientTrackingEvent** contém informações de um único evento para um destinatário. 
  
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
|[Data (MessageTracking)](date-messagetracking.md) <br/> |Este elemento é obrigatório.  <br/> |
|[Recipiente](recipient.md) <br/> |Este elemento é obrigatório.  <br/> |
|[DeliveryStatus](deliverystatus.md) <br/> |Este elemento é obrigatório.  <br/> |
|[EventDescription](eventdescription.md) <br/> |Este elemento é obrigatório.  <br/> |
|[EventData](eventdata.md) <br/> |Este elemento é opcional.  <br/> |
|[Servidor (MessageTracking)](server-messagetracking.md) <br/> |Este elemento é obrigatório.  <br/> |
|[InternalId](internalid.md) <br/> |Este elemento é obrigatório.  <br/> |
|[BccRecipient](bccrecipient.md) <br/> |Este elemento é opcional.  <br/> |
|[HiddenRecipient](hiddenrecipient.md) <br/> |Este elemento é opcional.  <br/> |
|[UniquePathId](uniquepathid.md) <br/> |Este elemento é opcional.  <br/> |
|[RootAddress](rootaddress.md) <br/> |Este elemento é opcional.  <br/> |
|[Propriedades (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |Este elemento é opcional.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[RecipientTrackingEvents](recipienttrackingevents.md) <br/> |Contém uma lista de um ou mais eventos de controle de um destinatário.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetMessageTrackingReport](getmessagetrackingreport-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

