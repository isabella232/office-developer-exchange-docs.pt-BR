---
title: IconIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 92020822-2a86-4dfc-aee1-3067af4d4edf
description: O elemento IconIndex identifica o índice do ícone de um item ou conversa.
ms.openlocfilehash: 8ada9da2df1cf128009c9b153736b434925f1a3f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823848"
---
# <a name="iconindex"></a>IconIndex

O elemento **IconIndex** identifica o índice do ícone de um item ou conversa. 
  
```XML
<IconIndex>Default | PostItem | MailRead | MailUnread | MailReplied | MailForwarded | MailEncrypted | MailSmimeSigned | MailEncrytedReplied | MailSmimeSignedReplied | MailEncryptedForwarded | MailSmimeSignedForwarded | MailEncryptedRead | MailSmimeSignedRead | MailIrm | MailIrmForwarded | MailIrmReplied | SmsSubmitted | SmsRoutedToDeliveryPoint | SmsRoutedToExternalMessagingSystem | SmsDelivered | OutlookDefaultForContacts | AppointmentItem | AppointmentRecur | AppointmentMeet | AppointmentMeetRecur | AppointmentMeetNY | AppointmentMeetYes | AppointmentMeetNo | AppointmentMeetMaybe | AppointmentMeetCancel | AppointmentMeetInfo | TaskItem | TaskRecur | TaskOwned | TaskDelegated</IconIndex>
```

 **IconIndexType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[Conversa (ConversationType)](conversation-conversationtype.md) | [Item](item.md) | [contato](contact.md) | [DistributionList](distributionlist.md) | [mensagem](message-ex15websvcsotherref.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [tarefa ](task.md)
  
## <a name="text-value"></a>Text value

A tabela a seguir contém os valores de texto possíveis para o elemento **IconIndex** . 
  
|**Valor**|**Descrição**|
|:-----|:-----|
|||
|Default  <br/> |Especifica o ícone padrão.  <br/> |
|PostItem  <br/> |Especifica o ícone de um item de postagem.  <br/> |
|MailRead  <br/> |Especifica o que ícone de ler o email.  <br/> |
|MailUnread  <br/> |Especifica o ícone de email não lido.  <br/> |
|MailReplied  <br/> |Especifica o respondidas para ícone email.  <br/> |
|MailForwarded  <br/> |Especifica o ícone de email encaminhado.  <br/> |
|MailEncrypted  <br/> |Especifica o ícone de email criptografado.  <br/> |
|MailSmimeSigned  <br/> |Especifica o ícone de email assinadas Secure/Multipurpose Internet Mail Extensions (S/MIME).  <br/> |
|MailEncryptedReplied  <br/> |Especifica que o criptografadas respondido ícone email.  <br/> |
|MailSmimeSignedReplied  <br/> |Especifica que o S/MIME assinadas respondidas ícone email.  <br/> |
|MailEncryptedForwarded  <br/> |Especifica o ícone de email encaminhadas criptografado.  <br/> |
|MailSmimeSignedForwarded  <br/> |Especifica o S/MIME assinada encaminhado ícone email.  <br/> |
|MailEncryptedRead  <br/> |Especifica o ícone de leitura do email criptografado.  <br/> |
|MailSmimeSignedRead  <br/> |Especifica o S/MIME assinada ler ícone email.  <br/> |
|MailIrm  <br/> |Especifica o ícone de email protegido por IRM de gerenciamento de direitos de informação.  <br/> |
|MailIrmForwarded  <br/> |Especifica o protegidas por IRM encaminhado ícone email.  <br/> |
|MailIrmReplied  <br/> |Especifica que o protegidas por IRM respondido ícone email.  <br/> |
|SmsSubmitted  <br/> |Especifica o email de ícone enviado para roteamento do serviço SMS (Short Message).  <br/> |
|SmsRoutedToDeliveryPoint  <br/> |Especifica o ícone de roteamento de SMS para um ponto de entrega externo.  <br/> |
|SmsRoutedToExternalMessagingSystem  <br/> |Especifica o ícone para roteamento de SMS para um sistema de mensagens externo.  <br/> |
|SmsDelivered  <br/> |Especifica o ícone de email entregue SMS.  <br/> |
|OutlookDefaultForContacts  <br/> |Especifica o ícone padrão de contatos.  <br/> |
|AppointmentItem  <br/> |Especifica o ícone do item de compromisso.  <br/> |
|AppointmentRecur  <br/> |Especifica o ícone de compromisso recorrente.  <br/> |
|AppointmentMeet  <br/> |Especifica o ícone de reunião.  <br/> |
|AppointmentMeetRecur  <br/> |Especifica o ícone de reunião recorrente.  <br/> |
|AppointmentMeetNY  <br/> |Especifica o ícone uma resposta provisório à reunião.  <br/> |
|AppointmentMeetYes  <br/> |Especifica a reunião ícone de aceitação.  <br/> |
|AppointmentMeetNo  <br/> |Especifica o ícone de reunião recusada.  <br/> |
|AppointmentMeetMaybe  <br/> |Especifica o ícone uma resposta talvez à reunião.  <br/> |
|AppointmentMeetCancel  <br/> |Especifica o ícone de cancelar a reunião.  <br/> |
|AppointmentMeetInfo  <br/> |Especifica a reunião ícone informações.  <br/> |
|TaskItem  <br/> |Especifica o ícone do item de tarefa.  <br/> |
|TaskRecur  <br/> |Especifica o ícone de tarefa recorrente.  <br/> |
|TaskOwned  <br/> |Especifica a tarefa pertencente ícone.  <br/> |
|TaskDelegated  <br/> |Especifica o ícone delegada da tarefa.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |false  <br/> |
   

