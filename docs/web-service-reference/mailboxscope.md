---
title: MailboxScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c9778823-f290-4827-ba19-5f391ed4f877
description: O elemento MailboxScope identifica se uma pesquisa ou fetch para uma conversa deve abranger a caixa de correio primária, caixa de correio de arquivo morto ou ambos os primário e arquivar caixas de correio.
ms.openlocfilehash: 89c9776079d686b114d6b744150f1c6df3711eab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824293"
---
# <a name="mailboxscope"></a>MailboxScope

O elemento **MailboxScope** identifica se uma pesquisa ou fetch para uma conversa deve abranger a caixa de correio primária, caixa de correio de arquivo morto ou ambos os primário e arquivar caixas de correio. 
  
```XML
<MailboxScope> PrimaryOnly | ArchiveOnly | All </MailboxScope>
```

**MailboxSearchLocationType**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[FindConversation](findconversation.md) | [GetConversationItems](getconversationitems.md) | [conversa (ConversationType)](conversation-conversationtype.md)
  
## <a name="text-value"></a>Text value

O valor de texto do elemento **MailboxScope** é o escopo para localizar ou obter itens em uma conversa entre um dos caixas de correio primárias, arquivar caixas de correio ou ambos primário e arquivar caixas de correio. Um valor de texto de **PrimaryOnly** indica um escopo que refere-se a caixa de correio principal para um usuário. Um valor de texto de **ArchiveOnly** indica um escopo que refere-se a caixa de correio de arquivo morto para um usuário. Um valor de texto de **todas as** indica um escopo que refere-se a caixa de correio principal e a caixa de correio de arquivo morto. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |false  <br/> |
   

