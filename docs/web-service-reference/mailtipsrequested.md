---
title: MailTipsRequested
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MailTipsRequested
api_type:
- schema
ms.assetid: 8037bbe5-a37f-4f77-8209-27a94f9095ef
description: O elemento MailTipsRequested contém os tipos de dicas de email solicitadas ao serviço.
ms.openlocfilehash: 14a463d3b00a9f8b3e2aa2e822209ff87a221f9b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524851"
---
# <a name="mailtipsrequested"></a>MailTipsRequested

O **elemento MailTipsRequested** contém os tipos de dicas de email solicitadas ao serviço. 
  
```XML
<MailTipsRequested/>
```

 **MailTipTypes**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetMailTips](getmailtips.md) <br/> |Contém os destinatários e os tipos de dicas de email a recuperar.  <br/> |
   
## <a name="text-value"></a>Valor de texto

A tabela a seguir lista os valores possíveis para o **elemento MailTipsRequested.** 
  
|**Valor**|**Descrição**|
|:-----|:-----|
|Todos  <br/> |Representa todas as dicas de email disponíveis.  <br/> |
|OutOfOfficeMessage  <br/> |Representa a mensagem Out of Office (OOF).  <br/> |
|MailboxFullStatus  <br/> |Representa o status de uma caixa de correio que está cheia.  <br/> |
|CustomMailTip  <br/> |Representa uma dica de email personalizada.  <br/> |
|ExternalMemberCount  <br/> |Representa a contagem de membros externos.  <br/> |
|TotalMemberCount  <br/> |Representa a contagem de todos os membros.  <br/> |
|MaxMessageSize  <br/> |Representa o tamanho máximo de mensagem que um destinatário pode aceitar.  <br/> |
|DeliveryRestriction  <br/> |Indica se as restrições de entrega impedirão que a mensagem do remetente chegue ao destinatário.  <br/> |
|ModerationStatus  <br/> |Indica se a mensagem do remetente será revisada por um moderador.  <br/> |
|InvalidRecipient  <br/> |Indica se o destinatário é inválido.  <br/> |
   
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

