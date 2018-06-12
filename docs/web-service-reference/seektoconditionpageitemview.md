---
title: SeekToConditionPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b3b86720-d086-47c3-94af-921fdd719edf
description: O elemento SeekToConditionPageItemView identifica a condição que é usada para identificar o final de uma pesquisa, o índice inicial de uma pesquisa, as entradas máxima para retornar e as instruções de pesquisa para uma pesquisa FindItem ou FindConversation.
ms.openlocfilehash: e95246079f8c6e7acffac1dabb278895265767d9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825328"
---
# <a name="seektoconditionpageitemview"></a>SeekToConditionPageItemView

O elemento **SeekToConditionPageItemView** identifica a condição que é usada para identificar o final de uma pesquisa, o índice inicial de uma pesquisa, as entradas máxima para retornar e as instruções de pesquisa para um **FindItem** ou **FindConversation **pesquisa. 
  
```XML
<SeekToConditionPageItemView BasePoint="" MaxEntriesReturned="">
   <Condition/>
</SeekToConditionPageItemView>
```

 **SeekToConditionPageViewType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|Ponto de base  <br/> |O valor de texto do atributo **ponto de base** é o ponto de base do qual a pesquisa será iniciada. Um valor de texto de **início** indica que a pesquisa começará no início do conjunto de resultados. Um valor de texto do **final** indica que a pesquisa será iniciada no final do conjunto de resultados.  <br/> |
|MaxEntriesReturned  <br/> |O valor de texto do atributo **MaxEntriesReturned** é o número máximo de itens que podem ser retornadas em um conjunto de resultados.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

[Condição (RestrictionType)](condition-restrictiontype.md)
  
### <a name="parent-elements"></a>Elementos pai

[FindConversation](findconversation.md) | [FindItem](finditem.md)
  
## <a name="remarks"></a>Coment�rios

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> |false  <br/> |
   

