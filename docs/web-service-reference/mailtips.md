---
title: MailTips
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MailTips
api_type:
- schema
ms.assetid: c1cba493-bccc-4b8e-be8e-bfa8a8b10882
description: O elemento MailTips representa valores para vários tipos de dicas de email.
ms.openlocfilehash: bf7ed542d51f2a8cb3172275be12cb72104bc5b2
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511135"
---
# <a name="mailtips"></a>MailTips

O **elemento MailTips** representa valores para vários tipos de dicas de email. 
  
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
|[PendingMailTips](pendingmailtips.md) <br/> |Indica que as dicas de email nesse elemento não puderam ser avaliadas antes do tempo de processamento do servidor expirar.  <br/> |
|[OutOfOffice](outofoffice.md) <br/> |Representa a mensagem de resposta e um tempo de duração para o envio da mensagem de resposta.  <br/> |
|[MailboxFull](mailboxfull.md) <br/> |Indica se a caixa de correio do destinatário está cheia.  <br/> |
|[CustomMailTip](custommailtip.md) <br/> |Representa uma mensagem de dica de email personalizada.  <br/> |
|[TotalMemberCount](totalmembercount.md) <br/> |Representa a contagem de todos os membros em um grupo.  <br/> |
|[ExternalMemberCount](externalmembercount.md) <br/> |Representa a contagem de membros externos em um grupo.  <br/> |
|[MaxMessageSize](maxmessagesize.md) <br/> |Representa o tamanho máximo da mensagem que o destinatário pode aceitar.  <br/> |
|[DeliveryRestricted](deliveryrestricted.md) <br/> |Indica se as restrições de entrega impedirão que a mensagem do remetente chegue ao destinatário.  <br/> |
|[IsModerated](ismoderated.md) <br/> |Indica se a caixa de correio do destinatário está sendo moderada.  <br/> |
|[InvalidRecipient (MailTips)](invalidrecipient-mailtips.md) <br/> |Indica se o destinatário é inválido.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MailTipsResponseMessageType](mailtipsresponsemessagetype.md) <br/> |Representa as configurações de dicas de email.  <br/> |
   
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

