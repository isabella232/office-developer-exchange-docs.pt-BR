---
title: SearchDumpster
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ddb62dce-c87a-4714-8023-a6b697a29699
description: O elemento SearchDumpster especifica se deve pesquisar no dumpster do Exchange.
ms.openlocfilehash: 067bf8ea3e589aa392c6b8ba6d4dc10b430c1f28
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460488"
---
# <a name="searchdumpster"></a>SearchDumpster

O elemento **SearchDumpster** especifica se deve pesquisar no dumpster do Exchange. 
  
```XML
<SearchDumpster> true | false </SearchDumpster>
```

 ****
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[FindMailboxStatisticsByKeywords](findmailboxstatisticsbykeywords.md)
  
## <a name="text-value"></a>Valor de texto

Um valor de texto **true** para o elemento **SearchDumpster** indica que a pesquisa de estatísticas de caixa de correio inclui o dumpster do Exchange. Um valor **false** indica que o dumpster do Exchange não é pesquisado. 
  
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
   

