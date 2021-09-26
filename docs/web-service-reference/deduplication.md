---
title: Deduplication
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: a38acc3d-29a8-4466-81a4-73cb30fe5e80
description: O elemento Deduplication indica se o resultado da pesquisa deve remover itens duplicados.
ms.openlocfilehash: 6178502d102b8c24b39d7276352c31740c62352c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543405"
---
# <a name="deduplication"></a>Deduplication

O **elemento Deduplication** indica se o resultado da pesquisa deve remover itens duplicados. 
  
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

Um valor de texto **true** para o elemento Deduplication indica que os resultados da pesquisa podem não conter itens duplicados. Um valor false indica **que** os resultados da pesquisa podem conter itens duplicados. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |types.xsd  <br/> |
|Pode estar vazio  <br/> |falso  <br/> |
   

