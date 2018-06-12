---
title: Dicas de email
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
description: O elemento de dicas de email representa os valores para os vários tipos de dicas de email.
ms.openlocfilehash: 3a2e95225b09fd2d81db32f821ea3069ab7e7852
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824311"
---
# <a name="mailtips"></a>Dicas de email

O elemento de **dicas de email** representa os valores para os vários tipos de dicas de email. 
  
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

 **Dicas de email**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[RecipientAddress](recipientaddress.md) <br/> |Representa a caixa de correio do destinatário.  <br/> |
|[PendingMailTips](pendingmailtips.md) <br/> |Indica que as dicas de email nesse elemento não pôde ser avaliadas antes de tempo limite de processamento do servidor expirou.  <br/> |
|[Fora do escritório](outofoffice.md) <br/> |Representa a mensagem de resposta e um tempo de duração para enviar a mensagem de resposta.  <br/> |
|[MailboxFull](mailboxfull.md) <br/> |Indica se a caixa de correio do destinatário está cheio.  <br/> |
|[CustomMailTip](custommailtip.md) <br/> |Representa uma mensagem de dica de email personalizada.  <br/> |
|[TotalMemberCount](totalmembercount.md) <br/> |Representa a contagem de todos os membros em um grupo.  <br/> |
|[ExternalMemberCount](externalmembercount.md) <br/> |Representa a contagem de membros externos em um grupo.  <br/> |
|[MaxMessageSize](maxmessagesize.md) <br/> |Representa o tamanho máximo da mensagem que o destinatário possa aceitar.  <br/> |
|[DeliveryRestricted](deliveryrestricted.md) <br/> |Indica se as restrições de entrega impede que a mensagem do remetente está atingindo o destinatário.  <br/> |
|[IsModerated](ismoderated.md) <br/> |Indica se a caixa de correio do destinatário está sendo moderada.  <br/> |
|[InvalidRecipient (dicas de email)](invalidrecipient-mailtips.md) <br/> |Indica se o destinatário é inválido.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MailTipsResponseMessageType](mailtipsresponsemessagetype.md) <br/> |Representa as configurações de dicas de email.  <br/> |
   
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

