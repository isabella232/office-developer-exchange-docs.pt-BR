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
description: O elemento FederatedDeliveryMailbox representa a caixa de correio para a qual uma mensagem entre instalações foi enviada.
ms.openlocfilehash: d493ed81e82237b7257e8c469f4552d931b73aa6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461944"
---
# <a name="federateddeliverymailbox"></a>FederatedDeliveryMailbox

O elemento **FederatedDeliveryMailbox** representa a caixa de correio para a qual uma mensagem entre instalações foi enviada. 
  
```XML
<FederatedDeliveryMailbox>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</FederatedDeliveryMailbox>
```

 **EmailAddresstype**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Nome (EmailAddresstype)](name-emailaddresstype.md) <br/> |Define o nome do usuário da caixa de correio. Este elemento é opcional.  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |Define o endereço SMTP (Simple Mail Transfer Protocol) de um usuário de caixa de correio. Este elemento é opcional.  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |Define o roteamento usado para a caixa de correio. O padrão é SMTP. Este elemento é opcional.  <br/> |
|[MailboxType](mailboxtype.md) <br/> |Define o tipo de caixa de correio de um usuário de caixa de correio. Este elemento é opcional.  <br/> |
|[ItemId](itemid.md) <br/> |Define o identificador de item de um contato ou de uma lista de distribuição privada para destinatários da pasta contatos de um usuário. Este elemento é opcional.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FindMessageTrackingReport](findmessagetrackingreport.md) <br/> |Contém critérios para os tipos de mensagens a serem localizados.  <br/> |
   
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



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

