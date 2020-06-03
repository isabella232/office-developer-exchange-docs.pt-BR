---
title: MailboxScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c9778823-f290-4827-ba19-5f391ed4f877
description: O elemento MailboxScope identifica se uma pesquisa ou busca de uma conversa deve abranger a caixa de correio principal, a caixa de correio de arquivo morto ou a caixa de correio principal e de arquivo morto.
ms.openlocfilehash: 92823c06d4fe186917c3cfb532eda821bd6a95a7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455370"
---
# <a name="mailboxscope"></a>MailboxScope

O elemento **MailboxScope** identifica se uma pesquisa ou busca de uma conversa deve abranger a caixa de correio principal, a caixa de correio de arquivo morto ou a caixa de correio principal e de arquivo morto. 
  
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

[FindConversation](findconversation.md)  |  [GetConversationItems](getconversationitems.md)  |  [Conversa (conversatype)](conversation-conversationtype.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do elemento **MailboxScope** é o escopo para localizar ou obter itens em uma conversa entre caixas de correio primárias, caixas de correio de arquivo morto ou caixas de correio primárias e de arquivo morto. Um valor de texto **PrimaryOnly** indica um escopo que direciona a caixa de correio principal de um usuário. Um valor de texto **ArchiveOnly** indica um escopo direcionado para a caixa de correio de arquivo morto de um usuário. Um valor de texto **All** indica um escopo que direciona a caixa de correio principal e a caixa de correio de arquivo morto. 
  
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
   

