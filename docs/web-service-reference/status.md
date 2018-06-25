---
title: Status
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Status
api_type:
- schema
ms.assetid: 80121e41-291b-4fc0-a55e-6f677d4b5fb5
description: O elemento de Status representa o status de um item de tarefa.
ms.openlocfilehash: 224b61913a5ae8e5b4aa0d756a9f2488df2741bd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825584"
---
# <a name="status"></a>Status

O elemento de **Status** representa o status de um item de tarefa. 
  
```xml
<Status/>
```

 **TaskStatusType**
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
   
## <a name="text-value"></a>Text value

É necessário um valor de texto. Estes são os valores de texto possíveis para esse elemento:
  
- NotStarted
    
- InProgress
    
- Completed
    
- WaitingOnOthers
    
- Adiada
    
## <a name="remarks"></a>Comentários

A definição de [CompleteDate](completedate.md) tem o mesmo efeito que a definição de [PercentComplete](percentcomplete.md) como 100 ou **Status** como **concluído**. Em uma solicitação que conjuntos de pelo menos dois dessas propriedades, a propriedade processada última determinará o valor que está definido para esses elementos. Por exemplo, se **PercentComplete** for 100, **CompleteDate** é 1/1/2007 e **o Status** é NotStarted e as propriedades são transmitidas nesta ordem, o efeito será definir o **Status** da tarefa como NotStarted, o **CompleteDate ** **Nulo**e a **PercentComplete** como 0. 
  
O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.
  
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

