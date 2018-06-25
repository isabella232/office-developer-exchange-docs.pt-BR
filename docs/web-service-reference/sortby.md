---
title: SortBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3dc4ab23-26b0-42b3-8930-f1c7eefecdeb
description: O elemento de SortBy contém uma propriedade de item usada para classificar os resultados de pesquisa.
ms.openlocfilehash: 357958e393ba9331d23ee48661f21e2afe00cf01
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825518"
---
# <a name="sortby"></a>SortBy

O elemento de **SortBy** contém uma propriedade de item usada para classificar os resultados de pesquisa. 
  
```XML
<SortBy Order="">
   <FieldURI/>
   <IndexedFieldURI/>
</SortBy>
```

 **FieldOrderType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|Ordem  <br/> |O valor de texto do atributo **ordem** é a ordem de classificação. Um valor de texto de **crescente** indica que os resultados são em ordem crescente. Um valor de texto de **Decrescente** indica que os resultados em ordem decrescente.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

[FieldURI](fielduri.md) | [IndexedFieldURI](indexedfielduri.md)
  
### <a name="parent-elements"></a>Elementos pai

[SearchMailboxes](searchmailboxes.md)
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

