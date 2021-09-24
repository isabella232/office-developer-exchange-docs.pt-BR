---
title: EndDate (Recurrence)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- EndDate
api_type:
- schema
ms.assetid: 16026595-26f8-4770-8a6d-0d3e4157effd
description: O elemento EndDate representa a data de término de uma tarefa recorrente ou um item de calendário que tenha o tipo de padrão EndDateRecurrence.
ms.openlocfilehash: c53d83a3fb2f3a6a841d7e16c94d20dd3c7a92a4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540086"
---
# <a name="enddate-recurrence"></a>EndDate (Recurrence)

O **elemento EndDate** representa a data de término de uma tarefa recorrente ou um item de calendário que tenha o tipo de padrão EndDateRecurrence. 
  
```xml
<EndDate/>
```

 **data**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[EndDateRecurrence](enddaterecurrence.md) <br/> |Descreve a data de início e a data de término de um padrão de recorrência de item.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto que representa uma data será necessário se esse elemento for usado. O valor não pode ser maior do que 1º de setembro de 4500 00:00:00.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

