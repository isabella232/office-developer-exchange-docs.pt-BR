---
title: FindMessageTrackingReport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FindMessageTrackingReport
api_type:
- schema
ms.assetid: 7ca6e2f7-aae1-4920-b839-73513ba8d4d8
description: O elemento FindMessageTrackingReport especifica critérios para os tipos de mensagens a encontrar.
ms.openlocfilehash: ec2ab16c6649d85edd86b9438e00ea7cfb9841ef
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513686"
---
# <a name="findmessagetrackingreport"></a>FindMessageTrackingReport

O **elemento FindMessageTrackingReport** especifica critérios para os tipos de mensagens a encontrar. 
  
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
|[Scope (NonEmptyStringType)](scope-nonemptystringtype.md) <br/> |Representa a extensiva extensiva que o relatório de controle de mensagens deve ser.  <br/> |
|[Domain (Message Tracking)](domain-message-tracking.md) <br/> |Contém o nome do domínio em que o controle de mensagens é executado.  <br/> |
|[Sender (EmailAddressType)](sender-emailaddresstype.md) <br/> |Contém informações de contato para o remetente da mensagem de email.  <br/> |
|[PurportedSender](purportedsender.md) <br/> |Contém informações de contato para o suposto remetente de uma mensagem de email.  <br/> |
|[Recipiente](recipient.md) <br/> |Contém o endereço de email do destinatário da mensagem.  <br/> |
|[Assunto](subject.md) <br/> |Contém o assunto da mensagem de email.  <br/> |
|[StartDateTime](startdatetime.md) <br/> |Contém a data e a hora de início da pesquisa.  <br/> |
|[EndDateTime](enddatetime.md) <br/> |Contém a data e a hora finais da pesquisa.  <br/> |
|[MessageId](messageid.md) <br/> |Contém o identificador de mensagem da pesquisa.  <br/> |
|[FederatedDeliveryMailbox](federateddeliverymailbox.md) <br/> |Contém o nome da caixa de correio onde a mensagem entre locais foi enviada.  <br/> |
|[DiagnosticsLevel](diagnosticslevel.md) <br/> |Representa o nível de detalhes para relatórios de diagnóstico.  <br/> |
|[ServerHint](serverhint.md) <br/> |Representa o ponto de partida para rastrear uma mensagem em um site remoto ou floresta.  <br/> |
|[Properties (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |Contém uma lista de uma ou mais propriedades de controle. Esse elemento é opcional.  <br/> |
   
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

