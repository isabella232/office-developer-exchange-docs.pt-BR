---
title: MailTipsRequested
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTipsRequested
api_type:
- schema
ms.assetid: 8037bbe5-a37f-4f77-8209-27a94f9095ef
description: O elemento MailTipsRequested contém os tipos de dicas de email solicitadas do serviço.
ms.openlocfilehash: fa2bef394ea8473aa65bdc2f1d39c0794186fdc6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824348"
---
# <a name="mailtipsrequested"></a>MailTipsRequested

O elemento **MailTipsRequested** contém os tipos de dicas de email solicitadas do serviço. 
  
```XML
<MailTipsRequested/>
```

 **MailTipTypes**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetMailTips](getmailtips.md) <br/> |Contém os destinatários e os tipos de dicas de email para recuperar.  <br/> |
   
## <a name="text-value"></a>Text value

A tabela a seguir lista os valores possíveis para o elemento **MailTipsRequested** . 
  
|**Valor**|**Descrição**|
|:-----|:-----|
|Todos  <br/> |Representa todas as dicas de email disponíveis.  <br/> |
|OutOfOfficeMessage  <br/> |Representa a mensagem de ausência temporária.  <br/> |
|MailboxFullStatus  <br/> |Representa o status de uma caixa de correio que está cheio.  <br/> |
|CustomMailTip  <br/> |Representa uma dica de email personalizado.  <br/> |
|ExternalMemberCount  <br/> |Representa a contagem de membros externos.  <br/> |
|TotalMemberCount  <br/> |Representa a contagem de todos os membros.  <br/> |
|MaxMessageSize  <br/> |Representa o tamanho de mensagem máximo que um destinatário pode aceitar.  <br/> |
|DeliveryRestriction  <br/> |Indica se as restrições de entrega impede que a mensagem do remetente está atingindo o destinatário.  <br/> |
|ModerationStatus  <br/> |Indica se a mensagem do remetente será revisada por um moderador.  <br/> |
|InvalidRecipient  <br/> |Indica se o destinatário é inválido.  <br/> |
   
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

