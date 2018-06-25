---
title: Intervalo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ee2891e4-3aa6-4258-9727-1f2ee9622508
description: O elemento Range Especifica um intervalo de ocorrências do item de calendário para um item de calendário de repetição.
ms.openlocfilehash: 0264c541604808b46a50e292b8ff75f205796295
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824946"
---
# <a name="range"></a>Intervalo

O elemento **Range** Especifica um intervalo de ocorrências do item de calendário para um item de calendário de repetição. 
  
```XML
<Range Start="" End="" Count="" CompareOriginalStartTime=""/>
```

 **OccurrencesRangeType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**Start** <br/> |O valor de texto do atributo **Iniciar** é a data de início do intervalo de item recorrente. Este é um valor de **data/hora** .  <br/> |
|**End** <br/> |O valor de texto do atributo **final** é a data de término do intervalo de item recorrente. Este é um valor de **data/hora** .  <br/> |
|**Count** <br/> |O valor de texto do atributo **Count** é o número de ocorrências do item recorrente. Este é um valor **inteiro** .  <br/> |
|**CompareOriginalStartTime** <br/> |O valor de texto de **true** para o atributo **CompareOriginalStartTime** indica que o cliente compare a hora de início original com a nova hora de início. Um valor **false** indica que o cliente não precisa comparar a hora de início original com a nova hora de início.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[Ranges](ranges.md)
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

