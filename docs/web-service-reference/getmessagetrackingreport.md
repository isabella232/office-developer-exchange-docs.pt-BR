---
title: GetMessageTrackingReport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetMessageTrackingReport
api_type:
- schema
ms.assetid: b6ffa8ef-90f6-402d-afac-c3f5ee55cf49
description: O elemento GetMessageTrackingReport contém a solicitação para a operação GetMessageTrackingReport recuperar a mensagem completa relatório de rastreamento para a ID especificada.
ms.openlocfilehash: cb16f6e9d322cefb0d59c962af8e2f60ebae0e90
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752564"
---
# <a name="getmessagetrackingreport"></a>GetMessageTrackingReport

O elemento **GetMessageTrackingReport** contém a solicitação para a [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md) recuperar a mensagem completa relatório de rastreamento para a ID especificada. 
  
```XML
<GetMessageTrackingReport>
   <Scope/>
   <ReportTemplate/>
   <RecipientFilter/>
   <MessageTrackingReportId/>
   <ReturnQueueEvents/>
   <DiagnosticsLevel/>
   <Properties/>
</GetMessageTrackingReport>
```

 **GetMessageTrackingReportRequestType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Escopo (NonEmptyStringType)](scope-nonemptystringtype.md) <br/> |Especifica onde a ser pesquisada. Este elemento é obrigatório.  <br/> |
|[ReportTemplate](reporttemplate.md) <br/> |Especifica o tipo de relatório para recuperar de rastreamento. Este elemento é obrigatório.  <br/> |
|[RecipientFilter](recipientfilter.md) <br/> |Especifica um endereço de destinatário para usar com o relatório de controle especificado. Esse elemento é opcional.  <br/> |
|[Messagetrackingreportid deve ser passado](messagetrackingreportid.md) <br/> |Especifica uma cadeia de caracteres de identidade que foi obtida a operação **FindMessageTrackingReport** . Este elemento é obrigatório.  <br/> |
|[ReturnQueueEvents](returnqueueevents.md) <br/> |Especifica que a pessoa que está executando a tarefa tem uma função privilegiada. Esse elemento é opcional.  <br/> |
|[DiagnosticsLevel](diagnosticslevel.md) <br/> |Especifica as informações de desempenho e de tempo que serão usadas para derivar o relatório de controle. Esse elemento é opcional.  <br/> |
|[Propriedades (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |Especifica uma lista de uma ou mais propriedades de controle. Esse elemento é opcional.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação GetMessageTrackingReport](getmessagetrackingreport-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

