---
title: NoEndRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NoEndRecurrence
api_type:
- schema
ms.assetid: ab2ebd9c-388e-45f1-abf9-56e293ef123b
description: O elemento NoEndRecurrence descreve a data de início de um padrão de recorrência do item que não tem uma data de término definidas.
ms.openlocfilehash: fc3eae170f5c07e31d7a80b45836efd07d74e543
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824537"
---
# <a name="noendrecurrence"></a>NoEndRecurrence

O elemento **NoEndRecurrence** descreve a data de início de um padrão de recorrência do item que não tem uma data de término definidas. 
  
```xml
<NoEndRecurrence>
   <StartDate/>
</NoEndRecurrence>
```

 **NoEndRecurrenceRangeType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[StartDate (recorrência)](startdate-recurrence.md) <br/> |Representa a data de início de uma tarefa recorrente ou item de calendário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Recorrência (RecurrenceType)](recurrence-recurrencetype.md) <br/> |Contém o padrão de recorrência para itens de calendário e solicitações de reunião.  <br/> |
|[Recorrência (TaskRecurrenceType)](recurrence-taskrecurrencetype.md) <br/> |Contém informações de recorrência de tarefas recorrentes.  <br/> |
   
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

