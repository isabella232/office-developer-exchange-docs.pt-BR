---
title: Operação CreateItem (tarefa)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: 12c5da4d-290c-4a8a-a965-0bf5d55c7978
description: A operação CreateItem cria itens de tarefa no armazenamento do Exchange.
ms.openlocfilehash: 5a5203202071ae9391faa9348902424317ee96d1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751606"
---
# <a name="createitem-operation-task"></a>Operação CreateItem (tarefa)

A operação CreateItem cria itens de tarefa no armazenamento do Exchange.
  
## <a name="task-createitem-request"></a>Solicitação de CreateItem de tarefa

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação de CreateItem mostra como criar um item de tarefa em uma caixa de correio.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                MessageDisposition="SaveOnly">
      <Items>
        <t:Task>
          <t:Subject>My task</t:Subject>
          <t:DueDate>2006-10-26T21:32:52</t:DueDate>
          <t:Status>NotStarted</t:Status>
        </t:Task>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comments

Solicitações de tarefas recorrentes são alteradas quando eles são recebidos pelo computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada. Ocorrem as seguintes alterações:
  
- Somente a data é salva para a propriedade [StartDate (recorrência)](startdate-recurrence.md) do intervalo de recorrência da tarefa. A parte do tempo será truncada. 
    
- Propriedade [StartDate (recorrência)](startdate-recurrence.md) pode ser ajustada, dependendo do padrão de recorrência. Por exemplo, se o padrão de recorrência é especificado como toda segunda-feira e o StartDate for definido como 26 de outubro de 2006, que é uma quinta-feira, StartDate é ajustado para 30 de outubro de 2006, que é a próxima segunda-feira. 
    
- Se a propriedade [StartDate](startdate.md) da tarefa é definida, ele é atualizado para coincidir com o [StartDate (recorrência)](startdate-recurrence.md) do intervalo de recorrência. A propriedade [DueDate](duedate.md) da tarefa também é atualizada com base em que o novo [StartDate](startdate.md).
    
- Se o [StartDate](startdate.md) não estiver definida, apenas a propriedade [DueDate](duedate.md) é atualizada para coincidir com o [StartDate (recorrência)](startdate-recurrence.md) do intervalo de recorrência. 
    
A tabela a seguir mostra as alterações que faz com que o servidor de acesso para cliente para uma tarefa recorrente que tem um Task.Recurrence.Pattern de toda segunda-feira.
  
**Alterações em uma tarefa recorrente**

|**Property**|**Valor original**|**Valor atualizado**|
|:-----|:-----|:-----|
|Task.StartDate  <br/> |1º de janeiro de 2006  <br/> |30 de outubro de 2006  <br/> |
|Task.DueDate  <br/> |3 de janeiro de 2006  <br/> |1 de novembro de 2006  <br/> |
|Task.Recurrence.Range.StartDate  <br/> |26 de outubro de 2006  <br/> |30 de outubro de 2006  <br/> |
   
Por padrão, se uma pasta de destino não for especificada, os itens de tarefa são criados na pasta tarefas.
  
### <a name="request-elements"></a>Elementos de solicitação

Os seguintes elementos são usados na solicitação:
  
- [CreateItem](createitem.md)
    
- [Itens (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md)
    
- [Task](task.md)
    
- [Assunto](subject.md)
    
- [DueDate](duedate.md)
    
- [Status](status.md)
    
## <a name="successful-task-createitem-response"></a>Tarefa bem-sucedida CreateItem resposta

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta bem-sucedida à solicitação de CreateItem.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Task>
              <t:ItemId Id="AAAtAE=" ChangeKey="EwAAABYA"/>
            </t:Task>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a>Elementos de resposta bem-sucedida

Os seguintes elementos são incluídos na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CreateItemResponse](createitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateItemResponseMessage](createitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Itens (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md)
    
- [Task](task.md)
    
- [ItemId](itemid.md)
    
## <a name="see-also"></a>Confira também



[Operação CreateItem](createitem-operation.md)


[Criação de tarefas](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[Atualizar as tarefas](http://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)
  
[A exclusão de tarefas](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

