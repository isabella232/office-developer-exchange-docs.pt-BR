---
title: EndDate (recorrência)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndDate
api_type:
- schema
ms.assetid: 16026595-26f8-4770-8a6d-0d3e4157effd
description: O elemento EndDate representa a data de término de uma tarefa recorrente ou um item de calendário que tenha o tipo de padrão de EndDateRecurrence.
ms.openlocfilehash: b8570a069fc0a2d05044a9c85ab2d5c39d70ccdf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752047"
---
# <a name="enddate-recurrence"></a>EndDate (recorrência)

O elemento **EndDate** representa a data de término de uma tarefa recorrente ou um item de calendário que tenha o tipo de padrão de EndDateRecurrence. 
  
```xml
<EndDate/>
```

 **Data**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[EndDateRecurrence](enddaterecurrence.md) <br/> |Descreve a data de início e a data final do padrão de recorrência de um item.  <br/> |
   
## <a name="text-value"></a>Text value

Se este elemento for usado, será necessário um valor de texto que representa uma data. O valor não pode ser maior que 1 de setembro de 4500 00:00:00.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

