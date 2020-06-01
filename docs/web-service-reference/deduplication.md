---
title: Duplicidades
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a38acc3d-29a8-4466-81a4-73cb30fe5e80
description: O elemento de eliminação de duplicatas indica se o resultado da pesquisa deve remover itens duplicados.
ms.openlocfilehash: c39f980658aba7036cfabb3b51af5a41005f97b6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463710"
---
# <a name="deduplication"></a>Duplicidades

O elemento de **eliminação de duplicatas** indica se o resultado da pesquisa deve remover itens duplicados. 
  
```XML
<Deduplication> true | false </Deduplication>
```

**Boolean**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[SearchMailboxes](searchmailboxes.md)  |  [SetHoldOnMailboxes](setholdonmailboxes.md)
  
## <a name="text-value"></a>Valor de texto

Um valor de texto **true** para o elemento de eliminação de duplicatas indica que os resultados da pesquisa não podem conter itens duplicados. Um valor **false** indica que os resultados da pesquisa podem conter itens duplicados. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> |falso  <br/> |
   

