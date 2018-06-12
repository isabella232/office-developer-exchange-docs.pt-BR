---
title: Operação CreateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: 78a52120-f1d0-4ed7-8748-436e554f75b6
description: A operação CreateItem cria itens no armazenamento do Exchange.
ms.openlocfilehash: 7e1808c685cdbaa1e8867aa7425b2cc52218d001
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751607"
---
# <a name="createitem-operation"></a>Operação CreateItem

A operação CreateItem cria itens no armazenamento do Exchange.
  
## <a name="using-the-createitem-operation"></a>Usando a operação CreateItem

Você pode usar a operação CreateItem para criar o seguinte:
  
- Itens de calendário
    
- Emails
    
- Solicitações de reunião
    
- Tarefas
    
- Contatos
    
Para obter mais informações, consulte o [operação CreateItem (item de calendário)](createitem-operation-calendar-item.md), [operação CreateItem (mensagem de email)](createitem-operation-email-message.md), [operação CreateItem (solicitação de reunião)](createitem-operation-meeting-request.md), [a operação de CreateItem (tarefa)](createitem-operation-task.md)e [operação CreateItem (contato) ](createitem-operation-contact.md).
  
A operação CreateItem suporta o uso de objetos de resposta. Objetos de resposta suportam a aceitação e rejeição de reuniões e o tratamento de botões de votação que estão incluídos em uma mensagem de email padrão. A tabela a seguir lista os objetos de resposta são manipulados na operação CreateItem.
  
|**Objeto de resposta**|**Action**|
|:-----|:-----|
|AcceptItem  <br/> |Aceite uma solicitação de reunião.  <br/> |
|CancelCalendarItem  <br/> |Cancele uma reunião. Isso difere da exclusão de todos os participantes porque ele exclui a reunião para o organizador também.  <br/> |
|DeclineItem  <br/> |Recuse uma solicitação de reunião.  <br/> |
|ForwardItem  <br/> |Envie uma solicitação de reunião para outra pessoa como uma solicitação de reunião.  <br/> |
|RemoveItem  <br/> |Remova uma reunião cancelada do calendário.  <br/> |
|ReplyAllToItem  <br/> |Envie uma mensagem que inclui o corpo da solicitação de reunião original para todos os participantes da reunião.  <br/> |
|ReplyToItem  <br/> |Envie uma mensagem que inclui o corpo da solicitação de reunião original para o remetente da solicitação de reunião.  <br/> |
|SendReadReceipt  <br/> |Envie uma confirmação de leitura para o remetente da solicitação de reunião.  <br/> |
|TentativelyAcceptItem  <br/> |Aceite provisoriamente uma solicitação de reunião.  <br/> |
   
A operação CreateItem também oferece suporte a objetos de reunião adicionais. A tabela a seguir lista os objetos adicionais que suporta a operação CreateItem.
  
|**Objeto de reunião**|**Descrição**|
|:-----|:-----|
|Mensagem de reunião  <br/> |Representa uma mensagem de reunião no armazenamento do Exchange. Esse é o objeto base para os outros objetos de reunião.  <br/> |
|Solicitação de Reunião  <br/> |Representa uma solicitação de reunião no armazenamento do Exchange.  <br/> |
|Resposta à reunião  <br/> |Representa uma resposta de reunião no armazenamento do Exchange.  <br/> |
|Cancelamento de reunião  <br/> |Representa o cancelamento da reunião no armazenamento do Exchange.  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação CreateItem (item de calendário)](createitem-operation-calendar-item.md)
  
[Operação CreateItem (contato)](createitem-operation-contact.md)
  
[Operação CreateItem (mensagem de email)](createitem-operation-email-message.md)
  
[Operação CreateItem (solicitação de reunião)](createitem-operation-meeting-request.md)
  
[Operação CreateItem (tarefa)](createitem-operation-task.md)
  
 **CreateItemType**

