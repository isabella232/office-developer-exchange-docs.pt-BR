---
title: Properties (ArrayOfTrackingPropertiesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Properties
api_type:
- schema
ms.assetid: 175566d2-fd62-45a2-8518-2827912cec88
description: O elemento Properties contém uma lista de uma ou mais propriedades de controle.
ms.openlocfilehash: 8232b94effe3aae5b07be12bdaf1b5e85331938f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542978"
---
# <a name="properties-arrayoftrackingpropertiestype"></a>Properties (ArrayOfTrackingPropertiesType)

O **elemento Properties** contém uma lista de uma ou mais propriedades de controle. 
  
- [FindMessageTrackingReport](findmessagetrackingreport.md)
  
- [Properties (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md)
  
```xml
<Properties>
   <TrackingPropertyType/>
</Properties>
```

**ArrayOfTrackingPropertiesType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[TrackingPropertyType](trackingpropertytype.md) <br/> |Representa um nome e um par de valores de cadeias de caracteres usadas para criar propriedades para relatórios de controle de mensagens.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindMessageTrackingReport](findmessagetrackingreport.md) <br/> |Especifica critérios para os tipos de mensagens a encontrar.  <br/> |
|[FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) <br/> |Contém o status e o resultado de uma única [solicitação de operação FindMessageTrackingReport.](findmessagetrackingreport-operation.md)  <br/> |
|[GetMessageTrackingReport](getmessagetrackingreport.md) <br/> |Contém a solicitação para a [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md) recuperar o relatório de controle de mensagens completo para a ID especificada.  <br/> |
|[GetMessageTrackingReportResponse](getmessagetrackingreportresponse.md) <br/> |Contém o resultado de uma única [solicitação de operação GetMessageTrackingReport.](getmessagetrackingreport-operation.md)  <br/> |
|[RecipientTrackingEvent](recipienttrackingevent.md) <br/> |Contém informações de um único evento para um destinatário.  <br/> |
|[MessageTrackingReport](messagetrackingreport.md) <br/> |Contém uma única mensagem retornada em uma [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md).  <br/> |
|[MessageTrackingSearchResult](messagetrackingsearchresult.md) <br/> |Contém um único resultado de mensagem para [um elemento FindMessageTrackingReportResponse.](findmessagetrackingreportresponse.md)  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services. Esse elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação FindMessageTrackingReport](findmessagetrackingreport-operation.md)
- [Operação GetMessageTrackingReport](getmessagetrackingreport-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

