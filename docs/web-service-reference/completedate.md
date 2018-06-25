---
title: CompleteDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CompleteDate
api_type:
- schema
ms.assetid: b2b53b87-6a0b-4a55-bcfc-3bf67d3c1700
description: O elemento CompleteDate representa a data em que um item foi concluído.
ms.openlocfilehash: 00a1ec25be737ec0a5cc874063e1bce19a96cee0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751403"
---
# <a name="completedate"></a>CompleteDate

O elemento **CompleteDate** representa a data em que um item foi concluído. 
  
```xml
<CompleteDate/>
```

 **DateTime**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Task](task.md) <br/> |Representa uma tarefa no armazenamento do Exchange.  <br/> |
|[Flag](flag.md) <br/> |Especifica um sinalizador em um item de caixa de correio.  <br/> |
   
## <a name="text-value"></a>Text value

Se este elemento for usado, será necessário um valor de texto que representa a data e hora.
  
## <a name="remarks"></a>Comentários

A definição de **CompleteDate** tem o mesmo efeito que a definição de [PercentComplete](percentcomplete.md) como 100 ou [Status](status.md) como **concluído**. Em uma solicitação que conjuntos de pelo menos dois dessas propriedades, a propriedade processada última determinará o valor que está definido para esses elementos. Por exemplo, se [PercentComplete](percentcomplete.md) é 100, **CompleteDate** é 1º de janeiro de 2007, [o Status](status.md) é **NotStarted**e as propriedades são transmitidas nesta ordem, o efeito será definir o [Status](status.md) da tarefa a ser **NotStarted **, o [CompleteDate](completedate.md) **Nulo**e [PercentComplete](percentcomplete.md) como 0. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Criação de tarefas](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[A exclusão de tarefas](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

