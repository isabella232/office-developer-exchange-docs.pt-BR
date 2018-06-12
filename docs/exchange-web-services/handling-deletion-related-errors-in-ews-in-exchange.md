---
title: Tratando erros relacionados a exclusão no EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1bbe8507-7730-45e5-9232-c4f6fc39c2d9
description: Descubra como lidar com erros relacionados a exclusão em aplicativos que você desenvolva usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: 0dc16c3350bb75fb1e91650f0a0f0b7423727eeb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750655"
---
# <a name="handling-deletion-related-errors-in-ews-in-exchange"></a>Tratando erros relacionados a exclusão no EWS no Exchange

Descubra como lidar com erros relacionados a exclusão em aplicativos que você desenvolva usando a API gerenciada de EWS ou EWS no Exchange.
  
Se seu aplicativo [exclui os itens e pastas](deleting-items-by-using-ews-in-exchange.md), você pode precisar manipular erros relacionados a exclusão. Você pode manipular esses erros em tempo de execução ou enquanto desenvolve seu aplicativo do EWS.
  
**Tabela 1: Erros relacionados a exclusão e como lidar com eles**

|**Erro**|**Ocorre quando você tenta …**|**Manipulá-lo pelo …**|
|:-----|:-----|:-----|
|ErrorAffectedTaskOccurrencesRequired  <br/> |Excluir uma instância de uma tarefa recorrente e a propriedade **AffectedTaskOccurrence** não estiver definida.  <br/> |A configuração da propriedade **AffectedTaskOccurrence** e tentar novamente a exclusão.  <br/> |
|ErrorCalendarCannotUpdateDeletedItem  <br/> |Atualize um item de calendário, localizado na pasta Itens excluídos quando a atualização for resultar em enviando um convite de reunião a participantes.  <br/> |Cancelando a atualização ou mover o item de calendário de volta para a pasta de calendário padrão e atualizar o item de calendário.  <br/> |
|ErrorCalendarOccurrenceIsDeletedFromRecurrence  <br/> |Referência a uma ocorrência excluída de um compromisso recorrente.  <br/> |Removendo uma referência a uma ocorrência excluída.  <br/> |
|ErrorCannotDeleteObject  <br/> |Exclua um item que não pode ser excluído.  <br/> |Sair de tentativas para excluir o item.  <br/> |
|ErrorCannotDeleteTaskOccurrence  <br/> |Excluir uma ocorrência de uma tarefa nonrecurring ou excluir a última ocorrência de uma tarefa recorrente.  <br/> |Excluindo uma tarefa nonrecurring ou sair tenta excluir a última ocorrência de uma tarefa recorrente.  <br/> |
|ErrorDeleteDistinguishedFolder  <br/> |Exclua uma pasta diferenciada.  <br/> |Indicando que as pastas padrão não podem ser excluídas.  <br/> |
|ErrorItemNotFound  <br/> |Acesse um item excluído permanentemente.  <br/> |Removendo referências a um item quando ele é excluído do repositório. Se um item é recuperado, certifique-se de que você restabelecer referências necessárias para o cliente.  <br/> |
|ErrorSendMeetingCancellationsRequired  <br/> |Exclua um item de calendário sem especificação se cancelamentos de reunião devem ser enviados.  <br/> |Especificando que cancelamentos de reunião deve ou não deve ser enviada.  <br/> |
   
## <a name="see-also"></a>Confira também


- [Excluindo itens usando o EWS no Exchange](deleting-items-by-using-ews-in-exchange.md)
    
- [Receber notificações de eventos de caixa de correio relacionadas a exclusão do EWS no Exchange](pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange.md)
    
- [Excluir compromissos e cancelar reuniões usando o EWS no Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

