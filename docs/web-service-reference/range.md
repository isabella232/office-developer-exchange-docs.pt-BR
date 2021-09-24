---
title: Intervalo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: ee2891e4-3aa6-4258-9727-1f2ee9622508
description: O elemento Range especifica um intervalo de ocorrências de item de calendário para um item de calendário repetido.
ms.openlocfilehash: 0d16dad24dda48f084b3011d7b96eb719431d9da
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519097"
---
# <a name="range"></a>Intervalo

O **elemento Range** especifica um intervalo de ocorrências de item de calendário para um item de calendário repetido. 
  
```XML
<Range Start="" End="" Count="" CompareOriginalStartTime=""/>
```

 **OccurrencesRangeType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**Start** <br/> |O valor de texto do **atributo Start** é a data de início do intervalo de itens recorrente. Este é um **valor dateTime.**  <br/> |
|**End** <br/> |O valor de texto do atributo **End** é a data de término do intervalo de itens recorrente. Este é um **valor dateTime.**  <br/> |
|**Count** <br/> |O valor de texto **do atributo Count** é o número de ocorrências do item recorrente. Este é um **valor inteiro.**  <br/> |
|**CompareOriginalStartTime** <br/> |O valor de texto **true** para o **atributo CompareOriginalStartTime** indica que o cliente deve comparar a hora de início original com a nova hora de início. Um valor **false** indica que o cliente não precisa comparar a hora de início original com o novo horário de início.  <br/> |
   
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
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

