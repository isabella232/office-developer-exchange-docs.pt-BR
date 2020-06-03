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
description: O elemento FindMessageTrackingReport especifica critérios para os tipos de mensagens a serem localizados.
ms.openlocfilehash: d30e5391bb4305cae0004a9788df971a57297cae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462933"
---
# <a name="findmessagetrackingreport"></a>FindMessageTrackingReport

O elemento **FindMessageTrackingReport** especifica critérios para os tipos de mensagens a serem localizados. 
  
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
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Escopo (NonEmptyStringType)](scope-nonemptystringtype.md) <br/> |Representa o quão abrangentes o relatório de acompanhamento de mensagens deve ser.  <br/> |
|[Domínio (controle de mensagens)](domain-message-tracking.md) <br/> |Contém o nome do domínio onde o controle de mensagens é executado.  <br/> |
|[Remetente (EmailAddresstype)](sender-emailaddresstype.md) <br/> |Contém informações de contato para o remetente da mensagem de email.  <br/> |
|[PurportedSender](purportedsender.md) <br/> |Contém informações de contato para o remetente supostamente de uma mensagem de email.  <br/> |
|[Recipiente](recipient.md) <br/> |Contém o endereço de email do destinatário da mensagem.  <br/> |
|[Assunto](subject.md) <br/> |Contém o assunto da mensagem de email.  <br/> |
|[StartDateTime](startdatetime.md) <br/> |Contém a data e hora inicial da pesquisa.  <br/> |
|[EndDateTime](enddatetime.md) <br/> |Contém a data e a hora de término da pesquisa.  <br/> |
|[MessageId](messageid.md) <br/> |Contém o identificador de mensagem para a pesquisa.  <br/> |
|[FederatedDeliveryMailbox](federateddeliverymailbox.md) <br/> |Contém o nome da caixa de correio onde a mensagem entre locais foi enviada.  <br/> |
|[DiagnosticsLevel](diagnosticslevel.md) <br/> |Representa o nível de detalhes dos relatórios de diagnóstico.  <br/> |
|[ServerHint](serverhint.md) <br/> |Representa o ponto de partida para rastrear uma mensagem em um site ou floresta remoto.  <br/> |
|[Propriedades (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |Contém uma lista de uma ou mais propriedades de controle. Este elemento é opcional.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="text-value"></a>Valor de texto

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



[Operação FindMessageTrackingReport](findmessagetrackingreport-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

