---
title: FindMessageTrackingReport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindMessageTrackingReport
api_type:
- schema
ms.assetid: 7ca6e2f7-aae1-4920-b839-73513ba8d4d8
description: O elemento FindMessageTrackingReport Especifica os critérios para os tipos de mensagens para encontrar.
ms.openlocfilehash: 77545121aa056992248c045af3f3d36566678b94
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752294"
---
# <a name="findmessagetrackingreport"></a>FindMessageTrackingReport

O elemento **FindMessageTrackingReport** Especifica os critérios para os tipos de mensagens para encontrar. 
  
```xml
<FindMessageTrackingReport>
   <Scope/>
   <Domain/>
   <Sender/>
   <PurportedSender/>
   <Recipient/>
   <Subject/>
   <StartDateTime/>
   <EndDateTime/>
   <MessageId/>
   <FederatedDeliveryMailbox/>
   <DiagnosticsLevel/>
   <ServerHint/>
   <Properties/>
</FindMessageTrackingReport>
```

 **FindMessageTrackingReportRequestType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Escopo (NonEmptyStringType)](scope-nonemptystringtype.md) <br/> |Representa o quão abrangente o relatório de controle de mensagens devem ser.  <br/> |
|[Domínio (rastreamento de mensagens)](domain-message-tracking.md) <br/> |Contém o nome do domínio onde a acompanhamento de mensagens é executada.  <br/> |
|[Remetente (EmailAddressType)](sender-emailaddresstype.md) <br/> |Contém informações de contato para o remetente da mensagem de email.  <br/> |
|[PurportedSender](purportedsender.md) <br/> |Contém informações de contato para o emissor Denúncia de uma mensagem de email.  <br/> |
|[Recipient](recipient.md) <br/> |Contém o endereço de email para o destinatário da mensagem.  <br/> |
|[Assunto](subject.md) <br/> |Contém o assunto da mensagem de email.  <br/> |
|[StartDateTime](startdatetime.md) <br/> |Contém a data e a hora para a pesquisa inicial.  <br/> |
|[EndDateTime](enddatetime.md) <br/> |Contém a data e a hora para a pesquisa.  <br/> |
|[MessageId](messageid.md) <br/> |Contém o identificador de mensagem para a pesquisa.  <br/> |
|[FederatedDeliveryMailbox](federateddeliverymailbox.md) <br/> |Contém o nome da caixa de correio em que a mensagem de entre local foi enviada.  <br/> |
|[DiagnosticsLevel](diagnosticslevel.md) <br/> |Representa o nível de detalhe para relatórios de diagnóstico.  <br/> |
|[ServerHint](serverhint.md) <br/> |Representa o ponto de partida para rastreamento de uma mensagem em um site remoto ou da floresta.  <br/> |
|[Propriedades (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |Contém uma lista de uma ou mais propriedades de controle. Esse elemento é opcional.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="text-value"></a>Text value

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



[Operação FindMessageTrackingReport](findmessagetrackingreport-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

