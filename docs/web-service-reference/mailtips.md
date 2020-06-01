---
title: MailTips
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTips
api_type:
- schema
ms.assetid: c1cba493-bccc-4b8e-be8e-bfa8a8b10882
description: O elemento de dicas de email representa valores de vários tipos de dicas de email.
ms.openlocfilehash: 9bacdea7b4f3108f700ed102025445e01a73e69d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44447593"
---
# <a name="mailtips"></a>MailTips

O elemento de **dicas** de email representa valores de vários tipos de dicas de email. 
  
```XML
<MailTips>
   <RecipientAddress/>
   <PendingMailTips/>
   <OutOfOffice/>
   <MailboxFull/>
   <CustomMailTip/>
   <TotalMemberCount/>
   <ExternalMemberCount/>
   <MaxMessageSize/>
   <DeliveryRestricted/>
   <IsModerated/>
   <InvalidRecipient/>
</MailTips>
```

 **Dicas de Email**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[RecipientAddress](recipientaddress.md) <br/> |Representa a caixa de correio do destinatário.  <br/> |
|[PendingMailTips](pendingmailtips.md) <br/> |Indica que as dicas de email neste elemento não puderam ser avaliadas antes que o tempo limite de processamento do servidor tenha expirado.  <br/> |
|[Fora](outofoffice.md) <br/> |Representa a mensagem de resposta e um tempo de duração para envio da mensagem de resposta.  <br/> |
|[MailboxFull](mailboxfull.md) <br/> |Indica se a caixa de correio do destinatário está cheia.  <br/> |
|[CustomMailTip](custommailtip.md) <br/> |Representa uma mensagem de dica de email personalizada.  <br/> |
|[TotalMemberCount](totalmembercount.md) <br/> |Representa a contagem de todos os membros de um grupo.  <br/> |
|[ExternalMemberCount](externalmembercount.md) <br/> |Representa a contagem de membros externos em um grupo.  <br/> |
|[MaxMessageSize](maxmessagesize.md) <br/> |Representa o tamanho máximo de mensagem que o destinatário pode aceitar.  <br/> |
|[DeliveryRestricted](deliveryrestricted.md) <br/> |Indica se as restrições de entrega impedirão que a mensagem do remetente atinja o destinatário.  <br/> |
|[Ismoderadod](ismoderated.md) <br/> |Indica se a caixa de correio do destinatário está sendo moderada.  <br/> |
|[InvalidRecipient (dicas de dicas)](invalidrecipient-mailtips.md) <br/> |Indica se o destinatário é inválido.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MailTipsResponseMessageType](mailtipsresponsemessagetype.md) <br/> |Representa configurações de dicas de email.  <br/> |
   
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

