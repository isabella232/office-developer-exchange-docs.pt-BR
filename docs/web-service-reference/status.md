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
description: O elemento status representa o status de um item de tarefa.
ms.openlocfilehash: 5d022827990b96fd8790ae9566ef49028ebe404c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459956"
---
# <a name="status"></a>Status

O elemento **status** representa o status de um item de tarefa. 
  
```xml
<Status/>
```

 **TaskStatusType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Tarefa](task.md) <br/> |Representa uma tarefa no repositório do Exchange.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é obrigatório. Estes são os valores de texto possíveis para este elemento:
  
- NotStarted
    
- InProgress
    
- Completed
    
- WaitingOnOthers
    
- Adiado
    
## <a name="remarks"></a>Comentários

A configuração foi [concluída](completedate.md) tem o mesmo efeito que configurar a [PorcentagemConcluída](percentcomplete.md) como 100 ou **status** como **concluído**. Em uma solicitação que define pelo menos duas dessas propriedades, a última Propriedade processada determinará o valor definido para esses elementos. Por exemplo, se a **PorcentagemConcluída** é 100 **, Completed** é 1/1/2007, e o **status** é não é iniciado e as propriedades são transmitidas nesta ordem, o efeito será definir o **status** da tarefa como não iniciada, **concluída** como **nulo**e a **PorcentagemConcluída** como 0. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)


[Criando tarefas](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[Excluir tarefas](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

