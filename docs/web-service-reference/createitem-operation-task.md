---
title: Operação CreateItem (tarefa)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CreateItem
api_type:
- schema
ms.assetid: 12c5da4d-290c-4a8a-a965-0bf5d55c7978
description: A operação CreateItem cria itens de tarefa no Exchange store.
ms.openlocfilehash: 814a32e82cd5c1c95be252d1b53387741898dd40
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510250"
---
# <a name="createitem-operation-task"></a>Operação CreateItem (tarefa)

A operação CreateItem cria itens de tarefa no Exchange store.
  
## <a name="task-createitem-request"></a>Solicitação Task CreateItem

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação CreateItem mostra como criar um item de tarefa em uma caixa de correio.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
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

### <a name="comments"></a>Comentários

As solicitações de tarefas recorrentes são alteradas quando são recebidas pelo computador que está executando Microsoft Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada. As seguintes alterações ocorrem:
  
- Somente a data é salva para a [propriedade StartDate (Recurrence)](startdate-recurrence.md) do intervalo de recorrência da tarefa. A parte do tempo é truncada. 
    
- A [propriedade StartDate (Recurrence)](startdate-recurrence.md) pode ser ajustada, dependendo do padrão de recorrência. Por exemplo, se o padrão de recorrência for especificado como toda segunda-feira e StartDate estiver definido como 26 de outubro de 2006, que é uma quinta-feira, StartDate será ajustado para 30 de outubro de 2006, que é a próxima segunda-feira. 
    
- Se a [propriedade StartDate](startdate.md) da tarefa estiver definida, ela será atualizada para corresponder ao [StartDate (Recurrence)](startdate-recurrence.md) do intervalo de recorrência. A [propriedade DueDate](duedate.md) da tarefa também é atualizada com base no novo [StartDate](startdate.md).
    
- Se o [StartDate](startdate.md) não estiver definido, somente a [propriedade DueDate](duedate.md) será atualizada para corresponder ao [StartDate (Recurrence)](startdate-recurrence.md) do intervalo de recorrência. 
    
A tabela a seguir mostra as alterações que o servidor de Acesso para Cliente faz para uma tarefa recorrente que tem um Task.Recurrence.Pattern de todas as segundas-feiras.
  
**Alterações em uma tarefa recorrente**

|**Propriedade**|**Valor Original**|**Valor Atualizado**|
|:-----|:-----|:-----|
|Task.StartDate  <br/> |1º de janeiro de 2006  <br/> |30 de outubro de 2006  <br/> |
|Task.DueDate  <br/> |3 de janeiro de 2006  <br/> |1º de novembro de 2006  <br/> |
|Task.Recurrence.Range.StartDate  <br/> |26 de outubro de 2006  <br/> |30 de outubro de 2006  <br/> |
   
Por padrão, se uma pasta de destino não for especificada, os itens de tarefa serão criados na pasta Tarefas.
  
### <a name="request-elements"></a>Elementos request

Os seguintes elementos são usados na solicitação:
  
- [CreateItem](createitem.md)
    
- [Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md)
    
- [Tarefa](task.md)
    
- [Assunto](subject.md)
    
- [DueDate](duedate.md)
    
- [Status](status.md)
    
## <a name="successful-task-createitem-response"></a>Resposta CreateItem de Tarefa Bem-sucedida

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta bem-sucedida à solicitação CreateItem.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-response-elements"></a>Elementos de resposta bem-sucedidos

Os seguintes elementos estão incluídos na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CreateItemResponse](createitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateItemResponseMessage](createitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md)
    
- [Tarefa](task.md)
    
- [ItemId](itemid.md)
    
## <a name="see-also"></a>Confira também



[Operação CreateItem](createitem-operation.md)


[Criando tarefas](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[Atualizando tarefas](https://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)
  
[Excluir Tarefas](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

