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
description: A operação CreateItem cria itens no repositório do Exchange.
ms.openlocfilehash: f6aaa9ed8e8257f19780492d6137fb015c1b6136
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458863"
---
# <a name="createitem-operation"></a>Operação CreateItem

A operação CreateItem cria itens no repositório do Exchange.
  
## <a name="using-the-createitem-operation"></a>Usando a operação CreateItem

Você pode usar a operação CreateItem para criar o seguinte:
  
- Itens de calendário
    
- Emails
    
- Solicitações de reunião
    
- Tarefas
    
- Contatos
    
Para mais informações, consulte [operação CreateItem (item de calendário)](createitem-operation-calendar-item.md), [operação CreateItem (mensagem de email)](createitem-operation-email-message.md), [operação CreateItem (solicitação de reunião)](createitem-operation-meeting-request.md), [operação CreateItem (tarefa)](createitem-operation-task.md)e [operação CreateItem (contato)](createitem-operation-contact.md).
  
A operação CreateItem oferece suporte ao uso de objetos Response. Os objetos Response dão suporte à aceitação e rejeição de reuniões e ao tratamento de botões de votação incluídos em uma mensagem de email padrão. A tabela a seguir lista os objetos de resposta que são tratados na operação CreateItem.
  
|**Objeto Response**|**Action**|
|:-----|:-----|
|AcceptItem  <br/> |Aceitar uma solicitação de reunião.  <br/> |
|CancelCalendarItem  <br/> |Cancelar uma reunião. Isso difere da exclusão de todos os participantes, pois ele também exclui a reunião do organizador.  <br/> |
|DeclineItem  <br/> |Recusar uma solicitação de reunião.  <br/> |
|ForwardItem  <br/> |Envie uma solicitação de reunião para outra pessoa como uma solicitação de reunião.  <br/> |
|RemoveItem  <br/> |Remover uma reunião cancelada do calendário.  <br/> |
|ReplyAllToItem  <br/> |Envie uma mensagem que inclua o corpo da solicitação de reunião original para todos os participantes da reunião.  <br/> |
|ReplyToItem  <br/> |Envie uma mensagem que inclua o corpo da solicitação de reunião original para o remetente da solicitação de reunião.  <br/> |
|SendReadReceipt  <br/> |Envie uma confirmação de leitura para o remetente da solicitação de reunião.  <br/> |
|TentativelyAcceptItem  <br/> |Aceitar provisoriamente uma solicitação de reunião.  <br/> |
   
A operação CreateItem também oferece suporte a objetos de reunião adicionais. A tabela a seguir lista os objetos adicionais que a operação CreateItem suporta.
  
|**Objeto Meeting**|**Descrição**|
|:-----|:-----|
|Mensagem de reunião  <br/> |Representa uma mensagem de reunião no repositório do Exchange. Este é o objeto base para os outros objetos da reunião.  <br/> |
|Solicitação de Reunião  <br/> |Representa uma solicitação de reunião no repositório do Exchange.  <br/> |
|Resposta da reunião  <br/> |Representa uma resposta de reunião no repositório do Exchange.  <br/> |
|Cancelamento de reunião  <br/> |Representa um cancelamento de reunião no repositório do Exchange.  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação CreateItem (item de calendário)](createitem-operation-calendar-item.md)
  
[Operação CreateItem (contato)](createitem-operation-contact.md)
  
[Operação CreateItem (mensagem de email)](createitem-operation-email-message.md)
  
[Operação CreateItem (solicitação de reunião)](createitem-operation-meeting-request.md)
  
[Operação CreateItem (tarefa)](createitem-operation-task.md)
  
 **CreateItemType**

