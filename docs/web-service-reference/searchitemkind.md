---
title: SearchItemKind
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 89513c26-b751-4619-a300-0ed8f55b0102
description: O elemento SearchItemKind indica o tipo de itens pesquisados para uma operação FindMailboxStatisticsByKeyword.
ms.openlocfilehash: 93803d181f32d88c30ab0fa9a72bb92f22907dde
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510852"
---
# <a name="searchitemkind"></a>SearchItemKind

O **elemento SearchItemKind** indica o tipo de itens pesquisados para uma **operação FindMailboxStatisticsByKeyword.** 
  
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

[MessageTypes](messagetypes.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do **elemento SearchItemKind** é o tipo de item pesquisado para palavras-chave. A lista a seguir contém os valores de texto que podem ser usados no **elemento SearchItemKind.** 
  
- **Email** - Indica que as mensagens de email são pesquisadas por palavras-chave. 
    
- **Reuniões** - Indica que as reuniões são pesquisadas por palavras-chave. 
    
- **Tarefas** - Indica que as tarefas são pesquisadas por palavras-chave. 
    
- **Observações** - Indica que as anotações são pesquisadas por palavras-chave. 
    
- **Documentos** - Indica que os documentos são pesquisados por palavras-chave. 
    
- **Diários** - Indica que os diários são pesquisados por palavras-chave. 
    
- **Contatos** - Indica que os contatos são pesquisados por palavras-chave. 
    
- **Im** - Indica que as mensagens instantâneas são pesquisadas por palavras-chave. 
    
- **Caixa** Postal - Indica que as mensagens de voz são pesquisadas por palavras-chave. 
    
- **Faxes** - Indica que os faxes são pesquisados por palavras-chave. 
    
- **Postagens** - Indica que as postagens são pesquisadas por palavras-chave. 
    
- **Rssfeeds** - Indica que feeds RSS são pesquisados por palavras-chave. 
    
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

