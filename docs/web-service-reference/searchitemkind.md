---
title: SearchItemKind
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 89513c26-b751-4619-a300-0ed8f55b0102
description: O elemento SearchItemKind indica o tipo de itens que são pesquisados para uma operação FindMailboxStatisticsByKeyword.
ms.openlocfilehash: e0625ac169c3083702494c094da15d38d220fe67
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463997"
---
# <a name="searchitemkind"></a>SearchItemKind

O elemento **SearchItemKind** indica o tipo de itens que são pesquisados para uma operação **FindMailboxStatisticsByKeyword** . 
  
```XML
<SearchItemKind>Email | Meetings | Tasks | Notes | Docs | Journals | Contacts | Im | Voicemail | Faxes | Posts | Rssfeeds</SearchItemKind>
```

 **SearchItemKindType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[MessageType](messagetypes.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do elemento **SearchItemKind** é o tipo de item procurado por palavras-chave. A lista a seguir contém os valores de texto que podem ser usados no elemento **SearchItemKind** . 
  
- **Email** : indica que as mensagens de email são pesquisadas por palavras-chave. 
    
- **Reuniões** : indica que as reuniões são pesquisadas em busca de palavras-chave. 
    
- **Tarefas** : indica que as tarefas são pesquisadas em busca de palavras-chave. 
    
- **Observações** : indica que as anotações são pesquisadas em busca de palavras-chave. 
    
- **Docs** -indica que os documentos são pesquisados em busca de palavras-chave. 
    
- **Diários** : indica que os diários são pesquisados em busca de palavras-chave. 
    
- **Contatos** : indica que os contatos são pesquisados em busca de palavras-chave. 
    
- **Im** : indica que as mensagens instantâneas são pesquisadas em busca de palavras-chave. 
    
- **Caixa postal** : indica que as mensagens de voz são pesquisadas em busca de palavras-chave. 
    
- **Faxes** : indica que os faxes são pesquisados em busca de palavras-chave. 
    
- **Postagens** -indica que as postagens são pesquisadas em busca de palavras-chave. 
    
- **Rssfeeds** -indica que os RSS feeds são pesquisados em busca de palavras-chave. 
    
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> ||
   

