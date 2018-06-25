---
title: Destinatário
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Recipient
api_type:
- schema
ms.assetid: 52adbb30-3bfd-48aa-9ea8-9f7d3b4bee44
description: O elemento de destinatário representa o destinatário para o qual o evento ocorreu.
ms.openlocfilehash: e8e8f9d6031d27c7441017c85eb26a143258b183
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824971"
---
# <a name="recipient"></a>Destinatário

O elemento de **destinatário** representa o destinatário para o qual o evento ocorreu. 
  
```XML
<Recipient>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Recipient>
```

 **EmailAddressType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Nome (EmailAddressType)](name-emailaddresstype.md) <br/> |Representa o nome do usuário da caixa de correio. Esse elemento é opcional.  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |Define o endereço de Simple Mail Transfer Protocol (SMTP) principal de um usuário de caixa de correio. Esse elemento é opcional.  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |Define o roteamento que é usado para a caixa de correio. O valor padrão é SMTP. Esse elemento é opcional.  <br/> |
|[MailboxType](mailboxtype.md) <br/> |Representa o tipo de caixa de correio que é representado por um endereço de email. Esse elemento é opcional.  <br/> |
|[ItemId](itemid.md) <br/> |Define o identificador do item de um contato ou uma lista de distribuição particular para destinatários da pasta de contatos do usuário. Esse elemento é opcional.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[RecipientTrackingEvent](recipienttrackingevent.md) <br/> |Contém informações para um único evento de um destinatário.  <br/> |
|[FindMessageTrackingReport](findmessagetrackingreport.md) <br/> |Especifica os critérios para os tipos de mensagens para encontrar.  <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

