---
title: GetMessageTrackingReport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetMessageTrackingReport
api_type:
- schema
ms.assetid: b6ffa8ef-90f6-402d-afac-c3f5ee55cf49
description: O elemento GetMessageTrackingReport contém a solicitação para a operação GetMessageTrackingReport recuperar o relatório de controle de mensagens completo para a ID especificada.
ms.openlocfilehash: cdf4e2c0f17c7d723dc56f30c445bfd527f891a3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516976"
---
# <a name="getmessagetrackingreport"></a>GetMessageTrackingReport

O **elemento GetMessageTrackingReport** contém a solicitação para a operação [GetMessageTrackingReport](getmessagetrackingreport-operation.md) recuperar o relatório de controle de mensagens completo para a ID especificada. 
  
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
|[Scope (NonEmptyStringType)](scope-nonemptystringtype.md) <br/> |Especifica onde executar a pesquisa. Este elemento é obrigatório.  <br/> |
|[ReportTemplate](reporttemplate.md) <br/> |Especifica o tipo de relatório de rastreamento a ser recuperado. Este elemento é obrigatório.  <br/> |
|[RecipientFilter](recipientfilter.md) <br/> |Especifica um endereço de destinatário a ser usado com o relatório de rastreamento especificado. Esse elemento é opcional.  <br/> |
|[MessageTrackingReportId](messagetrackingreportid.md) <br/> |Especifica uma cadeia de caracteres de identidade obtida da **operação FindMessageTrackingReport.** Este elemento é obrigatório.  <br/> |
|[ReturnQueueEvents](returnqueueevents.md) <br/> |Especifica que a pessoa que está executando a tarefa tem uma função privilegiada. Esse elemento é opcional.  <br/> |
|[DiagnosticsLevel](diagnosticslevel.md) <br/> |Especifica informações de tempo e desempenho que serão usadas para derivar o relatório de rastreamento. Esse elemento é opcional.  <br/> |
|[Properties (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |Especifica uma lista de uma ou mais propriedades de controle. Esse elemento é opcional.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
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

