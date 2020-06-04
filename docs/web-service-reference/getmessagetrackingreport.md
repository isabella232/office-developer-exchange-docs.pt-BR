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
description: O elemento GetMessageTrackingReport contém a solicitação para a operação GetMessageTrackingReport recuperar o relatório completo de controle de mensagens para a ID especificada.
ms.openlocfilehash: 30596acd209580147e0f03e12a7868502159b29c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466574"
---
# <a name="getmessagetrackingreport"></a>GetMessageTrackingReport

O elemento **GetMessageTrackingReport** contém a solicitação para a [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md) recuperar o relatório completo de controle de mensagens para a ID especificada. 
  
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
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Escopo (NonEmptyStringType)](scope-nonemptystringtype.md) <br/> |Especifica onde executar a pesquisa. Este elemento é obrigatório.  <br/> |
|[ReportTemplate](reporttemplate.md) <br/> |Especifica o tipo de relatório de controle a ser recuperado. Este elemento é obrigatório.  <br/> |
|[RecipientFilter](recipientfilter.md) <br/> |Especifica um endereço de destinatário a ser usado com o relatório de acompanhamento especificado. Este elemento é opcional.  <br/> |
|[MessageTrackingReportId](messagetrackingreportid.md) <br/> |Especifica uma cadeia de caracteres de identidade obtida da operação **FindMessageTrackingReport** . Este elemento é obrigatório.  <br/> |
|[ReturnQueueEvents](returnqueueevents.md) <br/> |Especifica que a pessoa que está executando a tarefa tem uma função privilegiada. Este elemento é opcional.  <br/> |
|[DiagnosticsLevel](diagnosticslevel.md) <br/> |Especifica as informações de tempo e desempenho que serão usadas para derivar o relatório de controle. Este elemento é opcional.  <br/> |
|[Propriedades (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |Especifica uma lista de uma ou mais propriedades de controle. Este elemento é opcional.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetMessageTrackingReport](getmessagetrackingreport-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

