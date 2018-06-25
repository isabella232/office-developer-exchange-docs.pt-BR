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
description: O elemento de ocorrência representa a ocorrência do dia da semana do mês em que ocorre a transição do fuso horário.
ms.openlocfilehash: bc5160480cc6881bb9d724aa61323f5717d1f2fa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824636"
---
# <a name="occurrence-time-zone-transition"></a>Ocorrência (transição de fuso horário)

O elemento de **ocorrência** representa a ocorrência do dia da semana do mês em que ocorre a transição do fuso horário. 
  
```xml
<Occurrence/>
```

**int**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[RecurringDayTransition](recurringdaytransition.md) <br/> |Representa uma transição de fuso horário que ocorre no mesmo dia cada ano.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto é um inteiro que representa a ocorrência do dia da semana do mês em que ocorre a transição do fuso horário. A tabela a seguir lista os valores possíveis.
  
|**Valor**|**Descrição**|
|:-----|:-----|
|1  <br/> |A primeira ocorrência do dia da semana desde o início do mês especificado.  <br/> |
|2  <br/> |A segunda ocorrência do dia da semana desde o início do mês especificado.  <br/> |
|3  <br/> |A terceira ocorrência do dia da semana desde o início do mês especificado.  <br/> |
|4  <br/> |A quarta ocorrência do dia da semana desde o início do mês especificado.  <br/> |
|-1  <br/> |A primeira ocorrência do dia da semana do final do mês especificado.  <br/> |
|-2  <br/> |A segunda ocorrência do dia da semana do final do mês especificado.  <br/> |
|-3  <br/> |A terceira ocorrência do dia da semana do final do mês especificado.  <br/> |
|-4  <br/> |A quarta ocorrência do dia da semana do final do mês especificado.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

