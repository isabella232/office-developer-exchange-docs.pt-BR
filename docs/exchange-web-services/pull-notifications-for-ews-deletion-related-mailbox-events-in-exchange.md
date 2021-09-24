---
title: Pull notifications for EWS deletion-related mailbox events in Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 83511eea-e0b5-4ef0-83b1-0c5434e6d3ab
description: Descubra quais eventos de caixa de correio são gerados quando você exclui itens usando o EWS Exchange.
ms.openlocfilehash: fa04d49f02cfec621f00a9b51b121cff22ca393b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510411"
---
# <a name="pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange"></a>Pull notifications for EWS deletion-related mailbox events in Exchange

Descubra quais eventos de caixa de correio são gerados quando você exclui itens usando o EWS Exchange.
  
Quando você [exclui itens e pastas de uma caixa de correio,](deleting-items-by-using-ews-in-exchange.md)isso dispara um evento de caixa de correio. Versões diferentes de Exchange retornam diferentes eventos de caixa de correio em resposta a alterações em itens e pastas em uma caixa de correio. A tabela a seguir identifica os eventos de caixa de correio retornados para exclusões quando você usa notificações pull para assinar eventos de caixa de correio. 
  
**Tabela 1: Eventos de caixa de correio relacionados à exclusão para notificações de pull**

|**Tipo de exclusão e a operação EWS**|**Exchange notificação 2010 quando você especificar cada identificador de pasta**|**Exchange notificação de 2010 quando você especificar todas as pastas**|**Exchange Online e Exchange 2013 quando você especificar cada identificador de pasta**|**Exchange Online e Exchange 2013 quando você especificar todas as pastas**|
|:-----|:-----|:-----|:-----|:-----|
|Exclusão suave por meio da [operação DeleteItem](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |DeletedEvent para o item.  <br/> ModifiedEvent para a pasta pai do item.  <br/> |DeletedEvent para o item.  <br/> ModifiedEvent para a pasta pai do item.  <br/> |MovedEvent para o item. Isso especifica os identificadores de pasta pai antigos e novos. O item é movido para a pasta Exclusões na lixeira.  <br/> ModifiedEvent para a pasta pai do item.  <br/> |DeletedEvent para o item.  <br/> DeletedEvent para o item da pasta de pesquisa padrão AllItems.  <br/> ModifiedEvent para a pasta pai do item.  <br/> |
|Exclusão difícil por meio da [operação DeleteItem](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |DeletedEvent para o item.  <br/> ModifiedEvent para a pasta pai do item.  <br/> |DeletedEvent para o item.  <br/> ModifiedEvent para a pasta pai do item.  <br/> |DeletedEvent para o item.  <br/> ModifiedEvent para a pasta pai do item.  <br/> |DeletedEvent para o item.  <br/> DeletedEvent para o item da pasta de pesquisa padrão AllItems.  <br/> ModifiedEvent para a pasta pai do item.  <br/> |
|Mover para a pasta Itens Excluídos por meio da [operação DeleteItem](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |MovedEvent para o item. Isso especifica os identificadores de pasta pai antigos e novos.  <br/> ModifiedEvent para a pasta pai antiga do item.  <br/> ModifiedEvent para a nova pasta pai do item, que é a pasta Itens Excluídos.  <br/> |MovedEvent para o item. Isso especifica os identificadores de pasta pai antigos e novos.  <br/> ModifiedEvent para a pasta pai antiga do item.  <br/> ModifiedEvent para a nova pasta pai do item, que é a pasta Itens Excluídos.  <br/> |MovedEvent para o item. Isso especifica os identificadores de pasta pai antigos e novos.  <br/> ModifiedEvent para a pasta pai antiga do item.  <br/> ModifiedEvent para a nova pasta pai do item, que é a pasta Itens Excluídos.  <br/> |DeletedEvent da pasta de pesquisa padrão AllItems.  <br/> CreatedEvent para o item na pasta AllItems.  <br/> ModifiedEvent para a pasta pai original do item.  <br/> ModifiedEvent para a pasta Itens Excluídos.  <br/> |
|Exclusão suave por meio da [operação DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |DeletedEvent para a pasta.  <br/> ModifiedEvent para a pasta pai da pasta.  <br/> |DeletedEvent para a pasta.  <br/> ModifiedEvent para a pasta pai da pasta.  <br/> |DeletedEvent para a pasta.  <br/> ModifiedEvent para a pasta pai da pasta.  <br/> |DeletedEvent para a pasta.  <br/> ModifiedEvent para a pasta pai da pasta.  <br/> |
|Exclusão difícil por meio da [operação DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |DeletedEvent para a pasta.  <br/> ModifiedEvent para a pasta pai da pasta.  <br/> |DeletedEvent para a pasta.  <br/> ModifiedEvent para a pasta pai da pasta.  <br/> |DeletedEvent para a pasta.  <br/> ModifiedEvent para a pasta pai da pasta.  <br/> |DeletedEvent para a pasta.  <br/> ModifiedEvent para a pasta pai da pasta.  <br/> |
|Mover para a pasta Itens Excluídos por meio da [operação DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |MovedEvent para a pasta. Isso especifica os identificadores de pasta pai antigos e novos.  <br/> ModifiedEvent para a pasta pai antiga da pasta.  <br/> ModifiedEvent para a nova pasta pai da pasta, que é a pasta Itens Excluídos.  <br/> |MovedEvent para a pasta. Isso especifica os identificadores de pasta pai antigos e novos.  <br/> ModifiedEvent para a pasta pai antiga da pasta.  <br/> ModifiedEvent para a nova pasta pai da pasta, que é a pasta Itens Excluídos.  <br/> |MovedEvent para a pasta. Isso especifica os identificadores de pasta pai antigos e novos.  <br/> ModifiedEvent para a pasta pai antiga da pasta.  <br/> ModifiedEvent para a nova pasta pai da pasta, que é a pasta Itens Excluídos.  <br/> |ModifiedEvent para a pasta pai antiga da pasta.  <br/> ModifiedEvent para a nova pasta pai da pasta, que é a pasta Itens Excluídos.  <br/> |
   
## <a name="see-also"></a>Confira também


- [Assinaturas de notificação, eventos de caixa de correio e EWS no Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    
- [Excluir itens usando o EWS no Exchange](deleting-items-by-using-ews-in-exchange.md)
    
- [Lidar com erros relacionados à exclusão no EWS no Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    

