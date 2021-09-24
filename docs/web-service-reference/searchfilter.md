---
title: SearchFilter
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 1a7ee364-b7da-4197-aab2-57134537109a
description: O elemento SearchFilter contém a cadeia de caracteres de consulta para filtrar as caixas de correio a serem retornadas de uma solicitação GetSearchableMailboxes.
ms.openlocfilehash: 19bb3109942c9a3064cbeaae4a19380d97c94feb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509354"
---
# <a name="searchfilter"></a>SearchFilter

O **elemento SearchFilter** contém a cadeia de caracteres de consulta para filtrar as caixas de correio a serem retornadas de uma **solicitação GetSearchableMailboxes.** 
  
```XML
<SearchFilter></SearchFilter>
```

 **cadeia de caracteres**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[GetSearchableMailboxes](getsearchablemailboxes.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do **elemento SearchFilter** é uma cadeia de caracteres de consulta para filtrar caixas de correio para pesquisa de descoberta. 
  
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
   

