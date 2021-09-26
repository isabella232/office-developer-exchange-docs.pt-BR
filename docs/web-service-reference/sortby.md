---
title: SortBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 3dc4ab23-26b0-42b3-8930-f1c7eefecdeb
description: O elemento SortBy contém uma propriedade de item usada para classificar o resultado da pesquisa.
ms.openlocfilehash: 8718bad3749a0409be2715b0e03001b97a4fb87e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544686"
---
# <a name="sortby"></a>SortBy

O **elemento SortBy** contém uma propriedade de item usada para classificar o resultado da pesquisa. 
  
```XML
<SortBy Order="">
   <FieldURI/>
   <IndexedFieldURI/>
</SortBy>
```

 **FieldOrderType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|Ordem  <br/> |O valor de texto do **atributo Order** é a ordem de classificação. Um valor de texto **de Ascending** indica que os resultados estão em ordem crescente. Um valor de texto **de Descending** indica que os resultados estão em ordem decrescente.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

[FieldURI](fielduri.md)  |  [IndexedFieldURI](indexedfielduri.md)
  
### <a name="parent-elements"></a>Elementos pai

[SearchMailboxes](searchmailboxes.md)
  
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
   

