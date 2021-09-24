---
title: FindMailboxStatisticsByKeywordsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: d3835800-8887-43db-9a8a-fe3cfea7a863
description: O elemento FindMailboxStatisticsByKeywordsResponseMessage especifica a mensagem de resposta para uma solicitação FindMailboxStatisticsByKeywords.
ms.openlocfilehash: f41a44ebb90b59c7458162dffe445bbeba7c2ba0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513714"
---
# <a name="findmailboxstatisticsbykeywordsresponsemessage"></a>FindMailboxStatisticsByKeywordsResponseMessage

O **elemento FindMailboxStatisticsByKeywordsResponseMessage** especifica a mensagem de resposta para uma **solicitação FindMailboxStatisticsByKeywords.** 
  
```XML
<FindMailboxStatisticsByKeywordsResponseMessage ResponseClass=" Success | Warning | Error ">
    <MailboxStatisticsSearchResult/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</FindMailboxStatisticsByKeywordsResponseMessage>
```

 **FindMailboxStatisticsByKeywordsResponseMessageType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|ResponseClass  <br/> |Especifica a classe de resposta.  <br/> |
   
#### <a name="responseclass"></a>ResponseClass

|**Valor**|**Descrição**|
|:-----|:-----|
|Sucesso  <br/> |Indica sucesso.  <br/> |
|Aviso  <br/> |Indica um aviso.  <br/> |
|Erro  <br/> |Indica um erro.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MailboxStatisticsSearchResult](mailboxstatisticssearchresult.md) <br/> |Especifica o resultado de uma pesquisa de caixa de correio.  <br/> |
|[MessageText](messagetext.md) <br/> |Fornece uma descrição de texto do status da resposta.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fornece informações de status sobre a solicitação.  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Atualmente não usado e reservado para uso futuro.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fornece informações adicionais de resposta a erros.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Especifica uma matriz de mensagens de resposta.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |messages.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

