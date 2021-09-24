---
title: MessageTrackingSearchResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MessageTrackingSearchResult
api_type:
- schema
ms.assetid: 8ea77aa8-b93f-4287-be36-0a9da06e0946
description: O elemento MessageTrackingSearchResult contém um único resultado de mensagem para um elemento FindMessageTrackingReportResponse.
ms.openlocfilehash: 2bd70461b2896d0204b163365d525f76d42bb213
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523877"
---
# <a name="messagetrackingsearchresult"></a>MessageTrackingSearchResult

O **elemento MessageTrackingSearchResult** contém um único resultado de mensagem para um [elemento FindMessageTrackingReportResponse.](findmessagetrackingreportresponse.md) 
  
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
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Assunto](subject.md) <br/> |Contém o assunto da mensagem de email.  <br/> |
|[Sender (EmailAddressType)](sender-emailaddresstype.md) <br/> |Contém o endereço do remetente da mensagem de email.  <br/> |
|[PurportedSender](purportedsender.md) <br/> |Contém informações de contato para o suposto remetente de uma mensagem de email.  <br/> |
|[Recipients (ArrayOfRecipientsType)](recipients-arrayofrecipientstype.md) <br/> |Contém uma lista de endereços de email que receberam essa mensagem.  <br/> |
|[SubmittedTime](submittedtime.md) <br/> |Contém a hora em que a mensagem foi enviada.  <br/> |
|[MessageTrackingReportId](messagetrackingreportid.md) <br/> |Contém uma ID interna que identifica a mensagem no banco de dados de transporte.  <br/> |
|[PreviousHopServer](previoushopserver.md) <br/> |Contém o nome do servidor na floresta que anteriormente aceitou a mensagem.  <br/> |
|[FirstHopServer](firsthopserver.md) <br/> |Contém o nome do servidor na floresta que aceitou a mensagem pela primeira vez.  <br/> |
|[Properties (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |Contém uma lista de uma ou mais propriedades de controle.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MessageTrackingSearchResults](messagetrackingsearchresults.md) <br/> |Contém uma lista de mensagens que corresponderão aos critérios de pesquisa.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services. Esse elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação FindMessageTrackingReport](findmessagetrackingreport-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

