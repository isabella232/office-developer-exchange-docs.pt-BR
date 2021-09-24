---
title: MessageTrackingReport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MessageTrackingReport
api_type:
- schema
ms.assetid: 2740bcf6-f86d-4756-a0f2-24ed6e9b75f7
description: O elemento MessageTrackingReport contém uma única mensagem retornada em uma operação GetMessageTrackingReport.
ms.openlocfilehash: aa55bb9e4f81a4cc0586d7258720aefd743923fd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539350"
---
# <a name="messagetrackingreport"></a>MessageTrackingReport

O **elemento MessageTrackingReport** contém uma única mensagem retornada em uma [operação GetMessageTrackingReport](getmessagetrackingreport-operation.md).
  
```XML
<MessageTrackingReport>
   <Sender/>
   <PurportedSender/>
   <Subject/>
   <SubmitTime/>
   <OriginalRecipients/>
   <RecipientTrackingEvents/>
   <Properties/>
</MessageTrackingReport>
```

 **MessageTrackingReportType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Sender (EmailAddressType)](sender-emailaddresstype.md) <br/> |Contém informações de contato para o remetente da mensagem de email.  <br/> |
|[PurportedSender](purportedsender.md) <br/> |Contém informações de contato para o suposto remetente de uma mensagem de email.  <br/> |
|[Assunto](subject.md) <br/> |Contém o assunto da mensagem de email.  <br/> |
|[SubmitTime](submittime.md) <br/> |Contém a hora do dia em que a mensagem de email foi enviada.  <br/> |
|[OriginalRecipients](originalrecipients.md) <br/> |Contém uma lista dos destinatários da mensagem de email.  <br/> |
|[RecipientTrackingEvents](recipienttrackingevents.md) <br/> |Contém uma lista de um ou mais eventos de controle para os destinatários.  <br/> |
|[Properties (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |Contém uma lista de uma ou mais propriedades de controle.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetMessageTrackingReportResponse](getmessagetrackingreportresponse.md) <br/> |Contém o resultado de uma única [solicitação de operação GetMessageTrackingReport.](getmessagetrackingreport-operation.md)  <br/> |
   
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



[Operação FindMessageTrackingReport](findmessagetrackingreport-operation.md)
  
[Operação GetMessageTrackingReport](getmessagetrackingreport-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)
  
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

