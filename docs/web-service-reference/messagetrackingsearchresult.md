---
title: MessageTrackingSearchResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageTrackingSearchResult
api_type:
- schema
ms.assetid: 8ea77aa8-b93f-4287-be36-0a9da06e0946
description: O elemento MessageTrackingSearchResult contém um resultado de mensagem única de um elemento FindMessageTrackingReportResponse.
ms.openlocfilehash: ad4fb9d9e2266222303bd2015a7afba0bb46721b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824460"
---
# <a name="messagetrackingsearchresult"></a>MessageTrackingSearchResult

O elemento **MessageTrackingSearchResult** contém um resultado de mensagem única de um elemento [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) . 
  
```xml
<MessageTrackingSearchResult>
   <Subject/>
   <Sender/>
   <PurportedSender/>
   <Recipients/>
   <SubmittedTime/>
   <MessageTrackingReportId/>
   <PreviousHopServer/>
   <FirstHopServer/>
   <Properties/>
</MessageTrackingSearchResult>
```

 **FindMessageTrackingSearchResultType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Assunto](subject.md) <br/> |Contém o assunto da mensagem de email.  <br/> |
|[Remetente (EmailAddressType)](sender-emailaddresstype.md) <br/> |Contém o endereço do remetente de mensagem de email.  <br/> |
|[PurportedSender](purportedsender.md) <br/> |Contém informações de contato para o emissor Denúncia de uma mensagem de email.  <br/> |
|[Destinatários (ArrayOfRecipientsType)](recipients-arrayofrecipientstype.md) <br/> |Contém uma lista de endereços de email que recebeu esta mensagem.  <br/> |
|[SubmittedTime](submittedtime.md) <br/> |Contém a hora em que a mensagem foi enviada.  <br/> |
|[Messagetrackingreportid deve ser passado](messagetrackingreportid.md) <br/> |Contém uma ID interna que identifica a mensagem no banco de dados de transporte.  <br/> |
|[PreviousHopServer](previoushopserver.md) <br/> |Contém o nome do servidor na floresta que anteriormente aceita a mensagem.  <br/> |
|[FirstHopServer](firsthopserver.md) <br/> |Contém o nome do servidor na floresta que primeiro aceita a mensagem.  <br/> |
|[Propriedades (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |Contém uma lista de uma ou mais propriedades de controle.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MessageTrackingSearchResults](messagetrackingsearchresults.md) <br/> |Contém uma lista de mensagens que correspondem aos critérios de pesquisa.  <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação FindMessageTrackingReport](findmessagetrackingreport-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

