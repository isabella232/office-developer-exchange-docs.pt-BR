---
title: Occurrence (Time Zone Transition)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Occurrence
api_type:
- schema
ms.assetid: 5c1142b1-c51f-42e1-bbb2-57e00cad0fdb
description: O elemento Occurrence representa a ocorrência do dia da semana no mês em que ocorre a transição de fuso horário.
ms.openlocfilehash: 9790b0e9541da0c22f2eac59850b8a361645c7b4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539273"
---
# <a name="occurrence-time-zone-transition"></a>Occurrence (Time Zone Transition)

O **elemento Occurrence** representa a ocorrência do dia da semana no mês em que ocorre a transição de fuso horário. 
  
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

O valor do texto é um inteiro que representa a ocorrência do dia da semana no mês em que ocorre a transição de fuso horário. A tabela a seguir lista os valores possíveis.
  
|**Valor**|**Descrição**|
|:-----|:-----|
|1  <br/> |A primeira ocorrência do dia especificado da semana desde o início do mês.  <br/> |
|2  <br/> |A segunda ocorrência do dia especificado da semana desde o início do mês.  <br/> |
|3  <br/> |A terceira ocorrência do dia especificado da semana desde o início do mês.  <br/> |
|4   <br/> |A quarta ocorrência do dia especificado da semana desde o início do mês.  <br/> |
|-1  <br/> |A primeira ocorrência do dia especificado da semana a partir do final do mês.  <br/> |
|-2  <br/> |A segunda ocorrência do dia especificado da semana a partir do final do mês.  <br/> |
|-3  <br/> |A terceira ocorrência do dia especificado da semana a partir do final do mês.  <br/> |
|-4  <br/> |A quarta ocorrência do dia especificado da semana a partir do final do mês.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

