---
title: Lidar com erros relacionados à exclusão no EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 1bbe8507-7730-45e5-9232-c4f6fc39c2d9
description: Saiba como lidar com erros relacionados à exclusão em aplicativos que você desenvolve usando a API Gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: d82901a2ebc8577258e191cbd014db93cc40d099
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513252"
---
# <a name="handling-deletion-related-errors-in-ews-in-exchange"></a>Lidar com erros relacionados à exclusão no EWS no Exchange

Saiba como lidar com erros relacionados à exclusão em aplicativos que você desenvolve usando a API Gerenciada do EWS ou o EWS no Exchange.
  
Se o aplicativo [excluir itens e pastas,](deleting-items-by-using-ews-in-exchange.md)talvez seja preciso lidar com erros relacionados à exclusão. Você pode manipular esses erros em tempo de execução ou enquanto desenvolve seu aplicativo do EWS.
  
**Tabela 1: Erros relacionados à exclusão e como lidar com eles**

|**Erro**|**Ocorre quando você tenta...**|**Manipulá-lo pelo …**|
|:-----|:-----|:-----|
|ErrorAffectedTaskOccurrencesRequired  <br/> |Exclua uma instância de uma tarefa recorrente e a **propriedade AffectedTaskOccurrence** não está definida.  <br/> |Definindo **a propriedade AffectedTaskOccurrence** e tentando novamente a exclusão.  <br/> |
|ErrorCalendarCannotUpdateDeletedItem  <br/> |Atualize um item de calendário localizado na pasta Itens Excluídos quando a atualização resultaria no envio de um convite de reunião aos participantes.  <br/> |Cancelando a atualização ou movendo o item de calendário de volta para a pasta de calendário padrão e atualizando o item de calendário.  <br/> |
|ErrorCalendarOccurrenceIsDeletedFromRecurrence  <br/> |Fazer referência a uma ocorrência excluída de um compromisso recorrente.  <br/> |Removendo uma referência a uma ocorrência excluída.  <br/> |
|ErrorCannotDeleteObject  <br/> |Exclua um item que não pode ser excluído.  <br/> |A quitação tenta excluir o item.  <br/> |
|ErrorCannotDeleteTaskOccurrence  <br/> |Exclua uma ocorrência de uma tarefa não recorrente ou exclua a última ocorrência de uma tarefa recorrente.  <br/> |Excluir uma tarefa não recorrente ou encerrar tentativas de excluir a última ocorrência de uma tarefa recorrente.  <br/> |
|ErrorDeleteDistinguishedFolder  <br/> |Excluir uma pasta distinta.  <br/> |Indicando que as pastas padrão não podem ser excluídas.  <br/> |
|ErrorItemNotFound  <br/> |Acesse um item excluído permanentemente.  <br/> |Removendo referências a um item quando ele é excluído do armazenamento. Se um item for recuperado, certifique-se de que você reinstale as referências necessárias ao cliente.  <br/> |
|ErrorSendMeetingCancellationsRequired  <br/> |Exclua um item de calendário sem especificar se os cancelamentos de reunião devem ser enviados.  <br/> |Especificando que os cancelamentos de reunião devem ou não ser enviados.  <br/> |
   
## <a name="see-also"></a>Confira também


- [Excluir itens usando o EWS no Exchange](deleting-items-by-using-ews-in-exchange.md)
    
- [Pull notifications for EWS deletion-related mailbox events in Exchange](pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange.md)
    
- [Excluir compromissos e cancelar reuniões usando o EWS no Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md)
    

