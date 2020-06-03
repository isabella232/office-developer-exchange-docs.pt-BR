---
title: SeekToConditionPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b3b86720-d086-47c3-94af-921fdd719edf
description: O elemento SeekToConditionPageItemView identifica a condição usada para identificar o final de uma pesquisa, o índice inicial de uma pesquisa, o número máximo de entradas a serem retornadas e as direções de pesquisa para uma pesquisa do FindItem ou do FindConversation.
ms.openlocfilehash: dbb073263740ccdf75367f85f672b7d5ec78f7a0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466833"
---
# <a name="seektoconditionpageitemview"></a>SeekToConditionPageItemView

O elemento **SeekToConditionPageItemView** identifica a condição usada para identificar o final de uma pesquisa, o índice inicial de uma pesquisa, o número máximo de entradas a serem retornadas e as direções de pesquisa para uma pesquisa do **FindItem** ou do **FindConversation** . 
  
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
|BasePoint  <br/> |O valor de texto do atributo **BasePoint** é o ponto base de onde a pesquisa começará. Um valor de texto **início** indica que a pesquisa começará no início do conjunto de resultados. Um valor de **fim** de texto indica que a pesquisa começará no final do conjunto de resultados.  <br/> |
|MaxEntriesReturned  <br/> |O valor de texto do atributo **MaxEntriesReturned** é o número máximo de itens que podem ser retornados em um conjunto de resultados.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

[Condição (RestrictionType)](condition-restrictiontype.md)
  
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
   

