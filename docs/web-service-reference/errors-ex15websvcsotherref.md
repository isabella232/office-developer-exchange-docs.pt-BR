---
title: Erros
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Errors
api_type:
- schema
ms.assetid: ea37a2b5-e2d1-4089-960f-7014b9535a50
description: O elemento de erros contém um recipiente de propriedades para armazenar os erros são retornados pelo serviço Web.
ms.openlocfilehash: a029492c1e3c11cc31d3501bd4ea0024ef8ecb91
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752101"
---
# <a name="errors"></a>Erros

O elemento de **erros** contém um recipiente de propriedades para armazenar os erros são retornados pelo serviço Web. 
  
[FindMessageTrackingReport](findmessagetrackingreport.md)
  
[Erros](errors-ex15websvcsotherref.md)
  
```xml
<Errors>
   <Properties/>
</Errors>
```

 **ArrayOfArraysOfTrackingPropertiesType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Propriedades (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |Contém uma lista de uma ou mais propriedades de controle.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) <br/> |Contém o status e o resultado de uma única solicitação de [operação FindMessageTrackingReport](findmessagetrackingreport-operation.md) .  <br/> |
|[GetMessageTrackingReportResponse](getmessagetrackingreportresponse.md) <br/> |Contém o resultado de uma única solicitação de [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md) .  <br/> |
   
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



[Operação FindMessageTrackingReport](findmessagetrackingreport-operation.md)
  
[Operação GetMessageTrackingReport](getmessagetrackingreport-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

