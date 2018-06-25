---
title: FederatedDeliveryMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FederatedDeliveryMailbox
api_type:
- schema
ms.assetid: cd56bcc0-d24a-4e8b-87bd-999bf69234b7
description: O elemento FederatedDeliveryMailbox representa a caixa de correio ao qual uma mensagem entre local foi enviada.
ms.openlocfilehash: 4a9250455f8de3ede25f2b5ba9433690137ca1d3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752235"
---
# <a name="federateddeliverymailbox"></a>FederatedDeliveryMailbox

O elemento **FederatedDeliveryMailbox** representa a caixa de correio ao qual uma mensagem entre local foi enviada. 
  
```XML
<FederatedDeliveryMailbox>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</FederatedDeliveryMailbox>
```

 **EmailAddressType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Nome (EmailAddressType)](name-emailaddresstype.md) <br/> |Define o nome do usuário da caixa de correio. Esse elemento é opcional.  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |Define o endereço de Simple Mail Transfer Protocol (SMTP) de um usuário de caixa de correio. Esse elemento é opcional.  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |Define o roteamento que é usado para a caixa de correio. O padrão é SMTP. Esse elemento é opcional.  <br/> |
|[MailboxType](mailboxtype.md) <br/> |Define o tipo de caixa de correio de um usuário de caixa de correio. Esse elemento é opcional.  <br/> |
|[ItemId](itemid.md) <br/> |Define o identificador do item de um contato ou uma lista de distribuição particular para destinatários da pasta de contatos do usuário. Esse elemento é opcional.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindMessageTrackingReport](findmessagetrackingreport.md) <br/> |Contém os critérios para os tipos de mensagens para encontrar.  <br/> |
   
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



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

