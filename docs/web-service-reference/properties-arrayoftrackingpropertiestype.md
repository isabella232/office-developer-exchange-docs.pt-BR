---
title: Propriedades (ArrayOfTrackingPropertiesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Properties
api_type:
- schema
ms.assetid: 175566d2-fd62-45a2-8518-2827912cec88
description: O elemento de propriedades contém uma lista de uma ou mais propriedades de controle.
ms.openlocfilehash: 079d2d2c101fdeb7f26d65798048c3c6c59f3e94
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824897"
---
# <a name="properties-arrayoftrackingpropertiestype"></a>Propriedades (ArrayOfTrackingPropertiesType)

O elemento de **Propriedades** contém uma lista de uma ou mais propriedades de controle. 
  
- [FindMessageTrackingReport](findmessagetrackingreport.md)
  
- [Propriedades (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md)
  
```xml
<Properties>
   <TrackingPropertyType/>
</Properties>
```

**ArrayOfTrackingPropertiesType**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[TrackingPropertyType](trackingpropertytype.md) <br/> |Representa um par de nome e valor de cadeias de caracteres que é usado para criar propriedades para relatórios de acompanhamento de mensagens.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindMessageTrackingReport](findmessagetrackingreport.md) <br/> |Especifica os critérios para os tipos de mensagens para encontrar.  <br/> |
|[FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) <br/> |Contém o status e o resultado de uma única solicitação de [operação FindMessageTrackingReport](findmessagetrackingreport-operation.md) .  <br/> |
|[GetMessageTrackingReport](getmessagetrackingreport.md) <br/> |Contém a solicitação para a [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md) recuperar a mensagem completa relatório de rastreamento para a ID especificada.  <br/> |
|[GetMessageTrackingReportResponse](getmessagetrackingreportresponse.md) <br/> |Contém o resultado de uma única solicitação de [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md) .  <br/> |
|[RecipientTrackingEvent](recipienttrackingevent.md) <br/> |Contém informações para um único evento de um destinatário.  <br/> |
|[MessageTrackingReport](messagetrackingreport.md) <br/> |Contém uma única mensagem retornada em uma [operação de GetMessageTrackingReport](getmessagetrackingreport-operation.md).  <br/> |
|[MessageTrackingSearchResult](messagetrackingsearchresult.md) <br/> |Contém um resultado de mensagem única de um elemento [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .  <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação FindMessageTrackingReport](findmessagetrackingreport-operation.md)
- [Operação GetMessageTrackingReport](getmessagetrackingreport-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

