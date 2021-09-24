---
title: SearchArchiveOnly
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: cce5344c-b622-44d4-bc14-a0de346c9335
description: O elemento SearchArchiveOnly indica se apenas a caixa de correio de arquivo morto é pesquisada para itens não indexáveis.
ms.openlocfilehash: a4766e101394bb83a0dcebdfe5b92f576f4a4160
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521673"
---
# <a name="searcharchiveonly"></a>SearchArchiveOnly

O **elemento SearchArchiveOnly** indica se apenas a caixa de correio de arquivo morto é pesquisada para itens não indexáveis. 
  
```xml
<SearchArchiveOnly>true | false</SearchArchiveOnly>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[GetNonIndexableItemStatistics](getnonindexableitemstatistics.md) │ [GetNonIndexableItemDetails](getnonindexableitemdetails.md)
  
## <a name="text-value"></a>Valor de texto

Um valor de texto **true** para o **elemento SearchArchiveOnly** indica que a pesquisa de item não indexável só é executada na caixa de correio de arquivo morto. Um valor de texto **false** indica que a pesquisa é realizada na caixa de correio principal e na caixa de correio de arquivo morto. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

