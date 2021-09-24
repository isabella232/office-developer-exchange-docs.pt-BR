---
title: Operação CreateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CreateItem
api_type:
- schema
ms.assetid: 78a52120-f1d0-4ed7-8748-436e554f75b6
description: A operação CreateItem cria itens no Exchange store.
ms.openlocfilehash: 2aee80d883aa623b8074ecc523d1a45fa71962da
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538398"
---
# <a name="createitem-operation"></a>Operação CreateItem

A operação CreateItem cria itens no Exchange store.
  
## <a name="using-the-createitem-operation"></a>Usando a operação CreateItem

Você pode usar a operação CreateItem para criar o seguinte:
  
- Itens de calendário
    
- Emails
    
- Solicitações de reunião
    
- Tarefas
    
- Contatos
    
Para obter mais informações, consulte [CreateItem operation (item](createitem-operation-calendar-item.md)de calendário), [CreateItem operation (email message),](createitem-operation-email-message.md) [CreateItem operation (meeting request),](createitem-operation-meeting-request.md) [CreateItem operation (task)](createitem-operation-task.md)e [CreateItem operation (contact)](createitem-operation-contact.md).
  
A operação CreateItem dá suporte ao uso de objetos de resposta. Os objetos de resposta suportam a aceitação e rejeição de reuniões e a manipulação de botões de votação incluídos em uma mensagem de email padrão. A tabela a seguir lista os objetos de resposta que são manipulados na operação CreateItem.
  
|**Objeto Response**|**Action**|
|:-----|:-----|
|AcceptItem  <br/> |Aceite uma solicitação de reunião.  <br/> |
|CancelCalendarItem  <br/> |Cancele uma reunião. Isso difere da exclusão de todos os participantes porque exclui também a reunião do organizador.  <br/> |
|DeclineItem  <br/> |Recusar uma solicitação de reunião.  <br/> |
|ForwardItem  <br/> |Envie uma solicitação de reunião para outra pessoa como uma solicitação de reunião.  <br/> |
|RemoveItem  <br/> |Remova uma reunião cancelada do calendário.  <br/> |
|ReplyAllToItem  <br/> |Envie uma mensagem que inclua o corpo da solicitação de reunião original para todos os participantes da reunião.  <br/> |
|ReplyToItem  <br/> |Envie uma mensagem que inclua o corpo da solicitação de reunião original para o remetente da solicitação de reunião.  <br/> |
|SendReadReceipt  <br/> |Envie um recibo de leitura para o remetente da solicitação de reunião.  <br/> |
|TentativelyAcceptItem  <br/> |Aceite provisamente uma solicitação de reunião.  <br/> |
   
A operação CreateItem também oferece suporte a objetos de reunião adicionais. A tabela a seguir lista objetos adicionais que a operação CreateItem oferece suporte.
  
|**Objeto Meeting**|**Descrição**|
|:-----|:-----|
|Mensagem de reunião  <br/> |Representa uma mensagem de reunião no Exchange store. Este é o objeto base para os outros objetos de reunião.  <br/> |
|Solicitação de Reunião  <br/> |Representa uma solicitação de reunião no Exchange store.  <br/> |
|Resposta à reunião  <br/> |Representa uma resposta de reunião no Exchange store.  <br/> |
|Cancelamento de Reunião  <br/> |Representa um cancelamento de reunião no Exchange store.  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação CreateItem (item do calendário)](createitem-operation-calendar-item.md)
  
[Operação CreateItem (contato)](createitem-operation-contact.md)
  
[Operação CreateItem (mensagem de e-mail)](createitem-operation-email-message.md)
  
[Operação CreateItem (solicitação de reunião)](createitem-operation-meeting-request.md)
  
[Operação CreateItem (tarefa)](createitem-operation-task.md)
  
 **CreateItemType**

