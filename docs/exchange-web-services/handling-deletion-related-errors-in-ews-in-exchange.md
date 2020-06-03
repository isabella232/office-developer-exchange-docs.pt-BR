---
title: Tratamento de erros relacionados à exclusão no EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1bbe8507-7730-45e5-9232-c4f6fc39c2d9
description: Descubra como lidar com erros relacionados à exclusão em aplicativos que você desenvolve usando a API gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: 41c217c1c3815606d898b8237ea327f34869174b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455944"
---
# <a name="handling-deletion-related-errors-in-ews-in-exchange"></a>Tratamento de erros relacionados à exclusão no EWS no Exchange

Descubra como lidar com erros relacionados à exclusão em aplicativos que você desenvolve usando a API gerenciada do EWS ou o EWS no Exchange.
  
Se o aplicativo [excluir itens e pastas](deleting-items-by-using-ews-in-exchange.md), talvez seja necessário lidar com erros relacionados à exclusão. Você pode manipular esses erros em tempo de execução ou enquanto desenvolve seu aplicativo do EWS.
  
**Tabela 1: erros relacionados à exclusão e como tratá-los**

|**Error**|**Ocorre quando você tenta...**|**Manipulá-lo pelo …**|
|:-----|:-----|:-----|
|ErrorAffectedTaskOccurrencesRequired  <br/> |Exclua uma instância de uma tarefa recorrente, e a propriedade **AffectedTaskOccurrence** não está definida.  <br/> |Definir a propriedade **AffectedTaskOccurrence** e repetir a exclusão.  <br/> |
|ErrorCalendarCannotUpdateDeletedItem  <br/> |Atualize um item de calendário localizado na pasta itens excluídos quando a atualização resultará no envio de um convite de reunião para os participantes.  <br/> |Cancelar a atualização ou mover o item de calendário de volta para a pasta de calendário padrão e atualizar o item de calendário.  <br/> |
|ErrorCalendarOccurrenceIsDeletedFromRecurrence  <br/> |Fazer referência a uma ocorrência excluída de um compromisso recorrente.  <br/> |Removendo uma referência a uma ocorrência excluída.  <br/> |
|ErrorCannotDeleteObject  <br/> |Excluir um item que não pode ser excluído.  <br/> |Encerrar tentativas de excluir o item.  <br/> |
|ErrorCannotDeleteTaskOccurrence  <br/> |Excluir uma ocorrência de uma tarefa recorrente ou excluir a última ocorrência de uma tarefa recorrente.  <br/> |Excluir uma tarefa recorrente ou encerrar tentativas de excluir a última ocorrência de uma tarefa recorrente.  <br/> |
|ErrorDeleteDistinguishedFolder  <br/> |Exclua uma pasta distinta.  <br/> |Indicando que as pastas padrão não podem ser excluídas.  <br/> |
|ErrorItemNotFound  <br/> |Acessar um item permanentemente excluído.  <br/> |Remover referências a um item quando ele é excluído da loja. Se um item for recuperado, certifique-se de restabelecer as referências necessárias ao cliente.  <br/> |
|ErrorSendMeetingCancellationsRequired  <br/> |Excluir um item de calendário sem especificar se o cancelamento de reunião deve ser enviado.  <br/> |Especificar que o cancelamento de reunião deve ou não deve ser enviado.  <br/> |
   
## <a name="see-also"></a>Confira também


- [Excluir itens usando o EWS no Exchange](deleting-items-by-using-ews-in-exchange.md)
    
- [Notificações de recebimento para eventos de caixa de correio relacionados à exclusão do EWS no Exchange](pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange.md)
    
- [Excluir compromissos e cancelar reuniões usando o EWS no Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

