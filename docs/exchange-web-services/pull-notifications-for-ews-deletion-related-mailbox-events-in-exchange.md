---
title: Notificações de recebimento para eventos de caixa de correio relacionados à exclusão do EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 83511eea-e0b5-4ef0-83b1-0c5434e6d3ab
description: Descubra quais eventos de caixa de correio são gerados quando você exclui itens usando o EWS no Exchange.
ms.openlocfilehash: c3d98ff798e3d0f6d214111d51da2c81278fd17d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457652"
---
# <a name="pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange"></a>Notificações de recebimento para eventos de caixa de correio relacionados à exclusão do EWS no Exchange

Descubra quais eventos de caixa de correio são gerados quando você exclui itens usando o EWS no Exchange.
  
Quando você [exclui itens e pastas de uma caixa de correio](deleting-items-by-using-ews-in-exchange.md), isso dispara um evento de caixa de correio. Versões diferentes do Exchange retornam diferentes eventos de caixa de correio em resposta às alterações feitas em itens e pastas em uma caixa de correio. A tabela a seguir identifica os eventos de caixa de correio que são retornados para exclusões quando você usa notificações de recebimento para inscrever-se em eventos de caixa de correio. 
  
**Tabela 1: eventos de caixa de correio relacionados à exclusão para notificações de recebimento**

|**Tipo de exclusão e operação do EWS**|**Notificação do Exchange 2010 ao especificar cada identificador de pasta**|**Notificação do Exchange 2010 ao especificar todas as pastas**|**Notificação do Exchange Online e do Exchange 2013 ao especificar cada identificador de pasta**|**Exchange Online e Exchange 2013 ao especificar todas as pastas**|
|:-----|:-----|:-----|:-----|:-----|
|Exclusão reversível por meio da [Operação DeleteItem](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |DeletedEvent para o item.  <br/> ModifiedEvent para a pasta pai do item.  <br/> |DeletedEvent para o item.  <br/> ModifiedEvent para a pasta pai do item.  <br/> |MovedEvent para o item. Isso especifica os identificadores de pasta pai antigo e novo. O item é movido para a pasta exclusões no dumpster.  <br/> ModifiedEvent para a pasta pai do item.  <br/> |DeletedEvent para o item.  <br/> DeletedEvent para o item da pasta de pesquisa padrão AllItems.  <br/> ModifiedEvent para a pasta pai do item.  <br/> |
|Exclusão impressa por meio da [Operação DeleteItem](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |DeletedEvent para o item.  <br/> ModifiedEvent para a pasta pai do item.  <br/> |DeletedEvent para o item.  <br/> ModifiedEvent para a pasta pai do item.  <br/> |DeletedEvent para o item.  <br/> ModifiedEvent para a pasta pai do item.  <br/> |DeletedEvent para o item.  <br/> DeletedEvent para o item da pasta de pesquisa padrão AllItems.  <br/> ModifiedEvent para a pasta pai do item.  <br/> |
|Mover para a pasta itens excluídos por meio da [Operação DeleteItem](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |MovedEvent para o item. Isso especifica os identificadores de pasta pai antigo e novo.  <br/> ModifiedEvent para a pasta pai antiga do item.  <br/> ModifiedEvent para a nova pasta pai do item, que é a pasta itens excluídos.  <br/> |MovedEvent para o item. Isso especifica os identificadores de pasta pai antigo e novo.  <br/> ModifiedEvent para a pasta pai antiga do item.  <br/> ModifiedEvent para a nova pasta pai do item, que é a pasta itens excluídos.  <br/> |MovedEvent para o item. Isso especifica os identificadores de pasta pai antigo e novo.  <br/> ModifiedEvent para a pasta pai antiga do item.  <br/> ModifiedEvent para a nova pasta pai do item, que é a pasta itens excluídos.  <br/> |DeletedEvent da pasta de pesquisa padrão AllItems.  <br/> CreatedEvent para o item na pasta AllItems.  <br/> ModifiedEvent para a pasta pai do item original.  <br/> ModifiedEvent para a pasta itens excluídos.  <br/> |
|Exclusão reversível por meio da [operação DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |DeletedEvent para a pasta.  <br/> ModifiedEvent para a pasta pai da pasta.  <br/> |DeletedEvent para a pasta.  <br/> ModifiedEvent para a pasta pai da pasta.  <br/> |DeletedEvent para a pasta.  <br/> ModifiedEvent para a pasta pai da pasta.  <br/> |DeletedEvent para a pasta.  <br/> ModifiedEvent para a pasta pai da pasta.  <br/> |
|Exclusão impressa por meio da [operação DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |DeletedEvent para a pasta.  <br/> ModifiedEvent para a pasta pai da pasta.  <br/> |DeletedEvent para a pasta.  <br/> ModifiedEvent para a pasta pai da pasta.  <br/> |DeletedEvent para a pasta.  <br/> ModifiedEvent para a pasta pai da pasta.  <br/> |DeletedEvent para a pasta.  <br/> ModifiedEvent para a pasta pai da pasta.  <br/> |
|Mover para a pasta itens excluídos por meio da [operação DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |MovedEvent para a pasta. Isso especifica os identificadores de pasta pai antigo e novo.  <br/> ModifiedEvent para a pasta pai antiga da pasta.  <br/> ModifiedEvent para a nova pasta pai da pasta, que é a pasta itens excluídos.  <br/> |MovedEvent para a pasta. Isso especifica os identificadores de pasta pai antigo e novo.  <br/> ModifiedEvent para a pasta pai antiga da pasta.  <br/> ModifiedEvent para a nova pasta pai da pasta, que é a pasta itens excluídos.  <br/> |MovedEvent para a pasta. Isso especifica os identificadores de pasta pai antigo e novo.  <br/> ModifiedEvent para a pasta pai antiga da pasta.  <br/> ModifiedEvent para a nova pasta pai da pasta, que é a pasta itens excluídos.  <br/> |ModifiedEvent para a pasta pai antiga da pasta.  <br/> ModifiedEvent para a nova pasta pai da pasta que é a pasta itens excluídos.  <br/> |
   
## <a name="see-also"></a>Confira também


- [Assinaturas de notificação, eventos de caixa de correio e EWS no Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    
- [Excluir itens usando o EWS no Exchange](deleting-items-by-using-ews-in-exchange.md)
    
- [Tratamento de erros relacionados à exclusão no EWS no Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    

