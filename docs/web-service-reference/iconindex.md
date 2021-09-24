---
title: IconIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 92020822-2a86-4dfc-aee1-3067af4d4edf
description: O elemento IconIndex identifica o índice de ícone de um item ou conversa.
ms.openlocfilehash: f0c024eeedcbda9aa5ad8afdea09a68f2499798e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541158"
---
# <a name="iconindex"></a>IconIndex

O **elemento IconIndex** identifica o índice de ícone de um item ou conversa. 
  
```XML
<IconIndex>Default | PostItem | MailRead | MailUnread | MailReplied | MailForwarded | MailEncrypted | MailSmimeSigned | MailEncrytedReplied | MailSmimeSignedReplied | MailEncryptedForwarded | MailSmimeSignedForwarded | MailEncryptedRead | MailSmimeSignedRead | MailIrm | MailIrmForwarded | MailIrmReplied | SmsSubmitted | SmsRoutedToDeliveryPoint | SmsRoutedToExternalMessagingSystem | SmsDelivered | OutlookDefaultForContacts | AppointmentItem | AppointmentRecur | AppointmentMeet | AppointmentMeetRecur | AppointmentMeetNY | AppointmentMeetYes | AppointmentMeetNo | AppointmentMeetMaybe | AppointmentMeetCancel | AppointmentMeetInfo | TaskItem | TaskRecur | TaskOwned | TaskDelegated</IconIndex>
```

 **IconIndexType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[Conversation (ConversationType)](conversation-conversationtype.md)  |  [Item](item.md)  |  [Contato](contact.md)  |  [DistributionList](distributionlist.md)  |  [Mensagem](message-ex15websvcsotherref.md)  |  [CalendarItem](calendaritem.md)  |  [PostItem](postitem.md)  |  [Tarefa](task.md)
  
## <a name="text-value"></a>Valor de texto

A tabela a seguir contém os valores de texto possíveis para o **elemento IconIndex.** 
  
|**Valor**|**Descrição**|
|:-----|:-----|
|||
|Padrão  <br/> |Especifica o ícone padrão.  <br/> |
|PostItem  <br/> |Especifica o ícone de um item de postagem.  <br/> |
|MailRead  <br/> |Especifica o ícone de leitura de email.  <br/> |
|MailUnread  <br/> |Especifica o ícone de email não lido.  <br/> |
|MailReplied  <br/> |Especifica o ícone de email respondido.  <br/> |
|MailForwarded  <br/> |Especifica o ícone de email encaminhado.  <br/> |
|MailEncrypted  <br/> |Especifica o ícone de email criptografado.  <br/> |
|MailSmimeSigned  <br/> |Especifica o ícone de email assinado Secure/Multipurpose Internet Mail Extensions (S/MIME).  <br/> |
|MailEncryptedReplied  <br/> |Especifica o ícone de email criptografado.  <br/> |
|MailSmimeSignedReplied  <br/> |Especifica o ícone de email assinado por S/MIME.  <br/> |
|MailEncryptedForwarded  <br/> |Especifica o ícone de email criptografado encaminhado.  <br/> |
|MailSmimeSignedForwarded  <br/> |Especifica o ícone de email assinado pelo S/MIME.  <br/> |
|MailEncryptedRead  <br/> |Especifica o ícone de email de leitura criptografado.  <br/> |
|MailSmimeSignedRead  <br/> |Especifica o ícone de email de leitura assinado por S/MIME.  <br/> |
|MailIrm  <br/> |Especifica o ícone de email protegido pelo IRM (Gerenciamento de Direitos de Informação).  <br/> |
|MailIrmForwarded  <br/> |Especifica o ícone de email protegido por IRM.  <br/> |
|MailIrmReplied  <br/> |Especifica o ícone de email protegido por IRM.  <br/> |
|SmsSubmitted  <br/> |Especifica o email de ícone enviado para roteamento do Serviço de Mensagem Curta (SMS).  <br/> |
|SmsRoutedToDeliveryPoint  <br/> |Especifica o ícone para roteamento de SMS para um ponto de entrega externo.  <br/> |
|SmsRoutedToExternalMessagingSystem  <br/> |Especifica o ícone para roteamento de SMS para um sistema de mensagens externo.  <br/> |
|SmsDelivered  <br/> |Especifica o ícone de email entregue por SMS.  <br/> |
|OutlookDefaultForContacts  <br/> |Especifica o ícone padrão para contatos.  <br/> |
|AppointmentItem  <br/> |Especifica o ícone do item de compromisso.  <br/> |
|AppointmentRecur  <br/> |Especifica o ícone de compromisso recorrente.  <br/> |
|AppointmentMeet  <br/> |Especifica o ícone da reunião.  <br/> |
|AppointmentMeetRecur  <br/> |Especifica o ícone de reunião recorrente.  <br/> |
|AppointmentMeetNY  <br/> |Especifica o ícone para uma resposta provisória à reunião.  <br/> |
|AppointmentMeetYes  <br/> |Especifica o ícone de aceitação da reunião.  <br/> |
|AppointmentMeetNo  <br/> |Especifica o ícone recusado da reunião.  <br/> |
|AppointmentMeetMaybe  <br/> |Especifica o ícone para uma resposta talvez à reunião.  <br/> |
|AppointmentMeetCancel  <br/> |Especifica o ícone de cancelamento da reunião.  <br/> |
|AppointmentMeetInfo  <br/> |Especifica o ícone de informações da reunião.  <br/> |
|Item de tarefa  <br/> |Especifica o ícone do item de tarefa.  <br/> |
|TaskRecur  <br/> |Especifica o ícone de tarefa recorrente.  <br/> |
|TaskOwned  <br/> |Especifica o ícone de propriedade da tarefa.  <br/> |
|TaskDelegated  <br/> |Especifica o ícone delegado da tarefa.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |falso  <br/> |
   

