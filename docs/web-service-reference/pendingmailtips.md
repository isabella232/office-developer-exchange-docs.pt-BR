---
title: PendingMailTips
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PendingMailTips
api_type:
- schema
ms.assetid: 0cd70eea-8d36-4b1b-bf80-5edf359e7ba7
description: O elemento PendingMailTips indica que as dicas de email nesse elemento não pôde ser avaliadas antes de tempo limite de processamento do servidor expirou.
ms.openlocfilehash: 73d597f6534ea29f7d26d6526c48631251521ae5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824704"
---
# <a name="pendingmailtips"></a>PendingMailTips

O elemento **PendingMailTips** indica que as dicas de email nesse elemento não pôde ser avaliadas antes de tempo limite de processamento do servidor expirou. 
  
```XML
<PendingMailTips>All | OutOfOfficeMessage | MailboxFullStatus | CustomMailTip | ExternalMemberCount | TotalMemberCount | MaxMessageSize | DeliveryRestriction | ModerateStatus | InvalidRecipient</PendingMailTips>
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
|[Dicas de email](mailtips.md) <br/> |Representa os valores para os vários tipos de dicas de email.  <br/> |
   
## <a name="text-value"></a>Text value

A tabela a seguir lista os valores possíveis para o elemento **PendingMailTips** . 
  
|**Valor**|**Descrição**|
|:-----|:-----|
|Todos  <br/> |Representa todas as dicas de email disponíveis.  <br/> |
|OutOfOfficeMessage  <br/> |Representa a mensagem de ausência temporária.  <br/> |
|MailboxFullStatus  <br/> |Representa o status de uma caixa de correio que está sendo completo.  <br/> |
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
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

