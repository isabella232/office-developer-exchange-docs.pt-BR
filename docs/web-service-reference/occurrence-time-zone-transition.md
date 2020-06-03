---
title: Ocorrência (transição de fuso horário)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Occurrence
api_type:
- schema
ms.assetid: 5c1142b1-c51f-42e1-bbb2-57e00cad0fdb
description: O elemento ocorrência representa a ocorrência do dia da semana no mês em que ocorre a transição de fuso horário.
ms.openlocfilehash: 846f6b22f43bcda07b9408d768d0845a5acfe668
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467974"
---
# <a name="occurrence-time-zone-transition"></a>Ocorrência (transição de fuso horário)

O elemento **ocorrência** representa a ocorrência do dia da semana no mês em que ocorre a transição de fuso horário. 
  
```xml
<Occurrence/>
```

**int**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[RecurringDayTransition](recurringdaytransition.md) <br/> |Representa uma transição de fuso horário que ocorre no mesmo dia a cada ano.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto é um inteiro que representa a ocorrência do dia da semana no mês em que ocorre a transição de fuso horário. A tabela a seguir lista os valores possíveis.
  
|**Valor**|**Descrição**|
|:-----|:-----|
|1  <br/> |A primeira ocorrência do dia da semana especificado desde o início do mês.  <br/> |
|duas  <br/> |A segunda ocorrência do dia da semana especificado desde o início do mês.  <br/> |
|3D  <br/> |A terceira ocorrência do dia da semana especificado desde o início do mês.  <br/> |
|4   <br/> |A quarta ocorrência do dia da semana especificado desde o início do mês.  <br/> |
|-1  <br/> |A primeira ocorrência do dia da semana especificado do final do mês.  <br/> |
|-2  <br/> |A segunda ocorrência do dia da semana especificado do final do mês.  <br/> |
|-3  <br/> |A terceira ocorrência do dia da semana especificado do final do mês.  <br/> |
|-4  <br/> |A quarta ocorrência do dia da semana especificado do final do mês.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

