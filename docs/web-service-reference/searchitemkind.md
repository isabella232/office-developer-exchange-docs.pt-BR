---
title: SearchItemKind
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 89513c26-b751-4619-a300-0ed8f55b0102
description: O elemento SearchItemKind indica o tipo de itens que são pesquisados para uma operação de FindMailboxStatisticsByKeyword.
ms.openlocfilehash: 1c099fc49ec882c1672b265ff0e3aa2c71c5f95b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825298"
---
# <a name="searchitemkind"></a>SearchItemKind

O elemento **SearchItemKind** indica o tipo de itens que são pesquisados para uma operação de **FindMailboxStatisticsByKeyword** . 
  
```XML
<SearchItemKind>Email | Meetings | Tasks | Notes | Docs | Journals | Contacts | Im | Voicemail | Faxes | Posts | Rssfeeds</SearchItemKind>
```

 **SearchItemKindType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[MessageTypes](messagetypes.md)
  
## <a name="text-value"></a>Text value

O valor de texto do elemento **SearchItemKind** é o tipo de item que será pesquisada para palavras-chave. A lista a seguir contém os valores de texto que podem ser usados no elemento **SearchItemKind** . 
  
- **Email** – indica que as mensagens de email são pesquisadas para palavras-chave. 
    
- **Reuniões** - indica que as reuniões são pesquisados para palavras-chave. 
    
- **Tarefas** - indica que as tarefas são pesquisadas para palavras-chave. 
    
- **Observações** - indica que as notas são pesquisadas para palavras-chave. 
    
- **Documentos** - indica que os documentos são pesquisados para palavras-chave. 
    
- **Diários** - indica que o diários são pesquisados para palavras-chave. 
    
- **Contatos** - indica que os contatos são pesquisados para palavras-chave. 
    
- **Mensagens instantâneas** - indica que as mensagens instantâneas são pesquisadas para palavras-chave. 
    
- **Caixa postal** - indica que o postais são pesquisados para palavras-chave. 
    
- **Aparelhos de fax** - indica que os faxes são pesquisados para palavras-chave. 
    
- **Postagens** - indica que as postagens são pesquisadas para palavras-chave. 
    
- **Rssfeeds** - indica que o RSS feeds são pesquisados para palavras-chave. 
    
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

