---
title: SeekToConditionPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: b3b86720-d086-47c3-94af-921fdd719edf
description: O elemento SeekToConditionPageItemView identifica a condição usada para identificar o final de uma pesquisa, o índice inicial de uma pesquisa, as entradas máximas a retornar e as instruções de pesquisa para uma pesquisa FindItem ou FindConversation.
ms.openlocfilehash: 6f4797a6b90456a50922db1c829757711816273e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546102"
---
# <a name="seektoconditionpageitemview"></a>SeekToConditionPageItemView

O **elemento SeekToConditionPageItemView** identifica a condição usada para identificar o final de uma pesquisa, o índice inicial de uma pesquisa, as entradas máximas a retornar e as instruções de pesquisa para uma pesquisa **FindItem** ou **FindConversation.** 
  
```XML
<SeekToConditionPageItemView BasePoint="" MaxEntriesReturned="">
   <Condition/>
</SeekToConditionPageItemView>
```

 **SeekToConditionPageViewType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|BasePoint  <br/> |O valor de texto do **atributo BasePoint** é o ponto base de onde a pesquisa será inicial. Um valor de texto **de Início** indica que a pesquisa será iniciada no início do conjunto de resultados. Um valor de texto **de End** indica que a pesquisa começará no final do conjunto de resultados.  <br/> |
|MaxEntriesReturned  <br/> |O valor de texto do **atributo MaxEntriesReturned** é o número máximo de itens que podem ser retornados em um conjunto de resultados.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

[Condition (RestrictionType)](condition-restrictiontype.md)
  
### <a name="parent-elements"></a>Elementos pai

[FindConversation](findconversation.md)  |  [FindItem](finditem.md)
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |falso  <br/> |
   

