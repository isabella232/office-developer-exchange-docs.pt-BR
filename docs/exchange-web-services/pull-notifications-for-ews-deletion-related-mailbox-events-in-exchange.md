---
title: Receber notificações de eventos de caixa de correio relacionadas a exclusão do EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 83511eea-e0b5-4ef0-83b1-0c5434e6d3ab
description: Descubra quais eventos de caixa de correio são gerados quando você excluir itens usando o EWS no Exchange.
ms.openlocfilehash: b12d6a16cc539f36b6b4dcd7274529e9def3c247
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750948"
---
# <a name="pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange"></a>Receber notificações de eventos de caixa de correio relacionadas a exclusão do EWS no Exchange

Descubra quais eventos de caixa de correio são gerados quando você excluir itens usando o EWS no Exchange.
  
Quando você [Excluir itens e pastas de uma caixa de correio](deleting-items-by-using-ews-in-exchange.md), isso dispara um evento de caixa de correio. Versões diferentes do Exchange retornam eventos de caixa de correio diferentes em resposta às mudanças para itens e pastas em uma caixa de correio. A tabela a seguir identifica os eventos de caixa de correio que são retornados para exclusões quando você usar notificações de recepção a inscrição em eventos de caixa de correio. 
  
**Tabela 1: Eventos de caixa de correio relacionadas a exclusão para notificações de recepção**

|**Tipo de exclusão e a operação de EWS**|**Notificação do Exchange 2010 quando você especifica o identificador de cada pasta**|**Notificação por quando você especifica que todas as pastas do Exchange 2010**|**Notificação do Exchange Online e Exchange 2013 quando você especifica o identificador de cada pasta**|**Quando você especifica que todas as pastas do Exchange Online e Exchange 2013**|
|:-----|:-----|:-----|:-----|:-----|
|Exclusão reversível via a [operação DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |DeletedEvent para o item.  <br/> ModifiedEvent para a pasta do pai do item.  <br/> |DeletedEvent para o item.  <br/> ModifiedEvent para a pasta do pai do item.  <br/> |MovedEvent para o item. Especifica os dois identificadores de pai antiga e nova pasta. O item é movido para a pasta de exclusões no dumpster.  <br/> ModifiedEvent para a pasta do pai do item.  <br/> |DeletedEvent para o item.  <br/> DeletedEvent para o item da pasta de pesquisa selecionando padrão.  <br/> ModifiedEvent para a pasta do pai do item.  <br/> |
|Exclusão dura via a [operação DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |DeletedEvent para o item.  <br/> ModifiedEvent para a pasta do pai do item.  <br/> |DeletedEvent para o item.  <br/> ModifiedEvent para a pasta do pai do item.  <br/> |DeletedEvent para o item.  <br/> ModifiedEvent para a pasta do pai do item.  <br/> |DeletedEvent para o item.  <br/> DeletedEvent para o item da pasta de pesquisa selecionando padrão.  <br/> ModifiedEvent para a pasta do pai do item.  <br/> |
|Mover para a pasta Itens excluídos via a [operação DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |MovedEvent para o item. Especifica os dois identificadores de pasta pai antiga e nova.  <br/> ModifiedEvent para a pasta pai da antiga do item.  <br/> ModifiedEvent para a pasta pai novo do item que é a pasta Itens excluídos.  <br/> |MovedEvent para o item. Especifica os dois identificadores de pasta pai antiga e nova.  <br/> ModifiedEvent para a pasta pai da antiga do item.  <br/> ModifiedEvent para a pasta pai novo do item que é a pasta Itens excluídos.  <br/> |MovedEvent para o item. Especifica os dois identificadores de pasta pai antiga e nova.  <br/> ModifiedEvent para a pasta pai da antiga do item.  <br/> ModifiedEvent para a pasta pai novo do item que é a pasta Itens excluídos.  <br/> |DeletedEvent da pasta de pesquisa selecionando padrão.  <br/> CreatedEvent para o item na pasta selecionando.  <br/> ModifiedEvent para a pasta pai da original do item.  <br/> ModifiedEvent para a pasta Itens excluídos.  <br/> |
|Exclusão reversível via a [operação DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |DeletedEvent para a pasta.  <br/> ModifiedEvent para a pasta do pai.  <br/> |DeletedEvent para a pasta.  <br/> ModifiedEvent para a pasta do pai.  <br/> |DeletedEvent para a pasta.  <br/> ModifiedEvent para a pasta do pai.  <br/> |DeletedEvent para a pasta.  <br/> ModifiedEvent para a pasta do pai.  <br/> |
|Exclusão dura via a [operação DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |DeletedEvent para a pasta.  <br/> ModifiedEvent para a pasta do pai.  <br/> |DeletedEvent para a pasta.  <br/> ModifiedEvent para a pasta do pai.  <br/> |DeletedEvent para a pasta.  <br/> ModifiedEvent para a pasta do pai.  <br/> |DeletedEvent para a pasta.  <br/> ModifiedEvent para a pasta do pai.  <br/> |
|Mover para a pasta Itens excluídos via a [operação DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |MovedEvent para a pasta. Especifica os dois identificadores de pasta pai antiga e nova.  <br/> ModifiedEvent para a pasta do antigo pai.  <br/> ModifiedEvent para nova pasta pai a pasta, que é a pasta Itens excluídos.  <br/> |MovedEvent para a pasta. Especifica os dois identificadores de pasta pai antiga e nova.  <br/> ModifiedEvent para a pasta do antigo pai.  <br/> ModifiedEvent para nova pasta pai a pasta, que é a pasta Itens excluídos.  <br/> |MovedEvent para a pasta. Especifica os dois identificadores de pasta pai antiga e nova.  <br/> ModifiedEvent para a pasta do antigo pai.  <br/> ModifiedEvent para nova pasta pai a pasta, que é a pasta Itens excluídos.  <br/> |ModifiedEvent para a pasta do antigo pai.  <br/> ModifiedEvent para a pasta pai de nova da pasta que é a pasta Itens excluídos.  <br/> |
   
## <a name="see-also"></a>Confira também


- [Inscrições de notificação, eventos de caixa de correio e EWS no Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    
- [Excluindo itens usando o EWS no Exchange](deleting-items-by-using-ews-in-exchange.md)
    
- [Tratando erros relacionados a exclusão no EWS no Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    

