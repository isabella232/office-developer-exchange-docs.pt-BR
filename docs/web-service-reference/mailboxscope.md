---
title: MailboxScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: c9778823-f290-4827-ba19-5f391ed4f877
description: O elemento MailboxScope identifica se uma pesquisa ou busca para uma conversa deve abranger a caixa de correio principal, a caixa de correio de arquivo morto ou a caixa de correio principal e arquivada.
ms.openlocfilehash: 705c72ae2aefbb16599f392eb712d080668490b0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522877"
---
# <a name="mailboxscope"></a>MailboxScope

O **elemento MailboxScope** identifica se uma pesquisa ou busca para uma conversa deve abranger a caixa de correio principal, a caixa de correio de arquivo morto ou a caixa de correio principal e arquivada. 
  
```XML
<MailboxScope> PrimaryOnly | ArchiveOnly | All </MailboxScope>
```

**MailboxSearchLocationType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[FindConversation](findconversation.md)  |  [GetConversationItems](getconversationitems.md)  |  [Conversation (ConversationType)](conversation-conversationtype.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do elemento **MailboxScope** é o escopo para localizar ou obter itens em uma conversa em caixas de correio primárias, caixas de correio de arquivo morto ou caixas de correio primárias e de arquivo morto. Um valor de texto **primaryOnly** indica um escopo destinado à caixa de correio principal para um usuário. Um valor de texto **de ArchiveOnly** indica um escopo destinado à caixa de correio de arquivo morto para um usuário. Um valor de texto **de All** indica um escopo destinado à caixa de correio principal e à caixa de correio de arquivo morto. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |falso  <br/> |
   

