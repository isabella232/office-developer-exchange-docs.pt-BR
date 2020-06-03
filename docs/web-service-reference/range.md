---
title: Intervalo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ee2891e4-3aa6-4258-9727-1f2ee9622508
description: O elemento Range especifica um intervalo de ocorrências de item de calendário para um item de calendário repetido.
ms.openlocfilehash: b5fb41709905290326b47e2662383031c34fd9c9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465307"
---
# <a name="range"></a>Intervalo

O elemento **Range** especifica um intervalo de ocorrências de item de calendário para um item de calendário repetido. 
  
```XML
<Range Start="" End="" Count="" CompareOriginalStartTime=""/>
```

 **OccurrencesRangeType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**Start** <br/> |O valor de texto do atributo de **início** é a data de início do intervalo de itens recorrentes. Este é um valor de **data/hora** .  <br/> |
|**End** <br/> |O valor de texto do atributo **final** é a data de término do intervalo de itens recorrentes. Este é um valor de **data/hora** .  <br/> |
|**Count** <br/> |O valor de texto do atributo **Count** é o número de ocorrências do item recorrente. Este é um valor **inteiro** .  <br/> |
|**CompareOriginalStartTime** <br/> |O valor de texto **true** para o atributo **CompareOriginalStartTime** indica que o cliente deve comparar a hora de início original com a nova hora de início. Um valor **false** indica que o cliente não precisa comparar a hora de início original com a nova hora de início.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[Ranges](ranges.md)
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> ||
   

