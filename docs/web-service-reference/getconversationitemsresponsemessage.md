---
title: GetConversationItemsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2e930650-7848-4bf2-a975-026309b3ea02
description: O elemento GetConversationItemsResponseMessage especifica a mensagem de resposta para uma solicitação GetConversationItems.
ms.openlocfilehash: b38bca60bb51c24a7635391c4e23e5426366cd72
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461069"
---
# <a name="getconversationitemsresponsemessage"></a>GetConversationItemsResponseMessage

O elemento **GetConversationItemsResponseMessage** especifica a mensagem de resposta para uma solicitação **GetConversationItems** . 
  
```XML
<GetConversationItemsResponseMessage ResponseClass="Success | Warning | Error">
    <Conversation/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetConversationItemsResponseMessage>
```

 **GetConversationItemsResponseMessageType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|ResponseClass  <br/> |Indica a classe da resposta.  <br/> |
   
#### <a name="responseclass"></a>ResponseClass

|**Valor**|**Descrição**|
|:-----|:-----|
|Êxito  <br/> |Indica êxito.  <br/> |
|Aviso  <br/> |Indica um aviso.  <br/> |
|Erro  <br/> |Indica um erro.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Conversa (ConversationResponseType)](conversation-conversationresponsetype.md) <br/> |Representa uma única conversa retornada em uma resposta **GetConversationItems** .  <br/> |
|[DescriptiveLinkKey](descriptivelinkkey.md) <br/> |Atualmente não usado e reservado para uso futuro.  <br/> |
|[MessageText](messagetext.md) <br/> |Fornece uma descrição de texto do status da resposta.  <br/> |
|[MessageXml](messagexml.md) <br/> |Fornece informações adicionais de resposta de erro.  <br/> |
|[ResponseCode](responsecode.md) <br/> |Fornece informações de status sobre a solicitação.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ResponseMessages](responsemessages.md) <br/> |Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange (EWS).  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |messages. xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

