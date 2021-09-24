---
title: DeleteItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DeleteItem
api_type:
- schema
ms.assetid: 055cdee8-3c7d-47db-9f27-740f4a674729
description: O elemento DeleteItem define uma solicitação para excluir um item de uma caixa de correio no Exchange store.
ms.openlocfilehash: aa421de447126a22c1f01b3a0dc7498ff5b74a65
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59528884"
---
# <a name="deleteitem"></a>DeleteItem

O **elemento DeleteItem** define uma solicitação para excluir um item de uma caixa de correio no Exchange store. 
  
```XML
<DeleteItem DeleteType="" SendMeetingCancellations="" AffectedTaskOccurrences="" SuppressReadReceipts="">
   <ItemIds/>
</DeleteItem>
```

 **DeleteItemType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**DeleteType** <br/> |Descreve como um item é excluído. Esse atributo é necessário.  <br/> |
|**SendMeetingCancellations** <br/> |Descreve se uma exclusão de item de calendário é comunicada aos participantes. Esse atributo é necessário quando os itens de calendário são excluídos. Esse atributo é opcional se itens não calendários são excluídos.  <br/> |
|**AffectedTaskOccurrences** <br/> |Descreve se uma instância de tarefa ou um mestre de tarefas é excluído por uma [operação DeleteItem](deleteitem-operation.md). Esse atributo é necessário quando as tarefas são excluídas. Esse atributo é opcional quando itens que não são da tarefa são excluídos.  <br/> |
|**SuppressReadReceipts** <br/> |Indica se os recibos de leitura do item excluído são suprimidos. Um valor de texto **true**, indica que os recibos de leitura são suprimidos. Um valor **false** indica que os recibos de leitura são enviados ao remetente. Esse atributo é opcional.  <br/> |
   
#### <a name="deletetype-attribute"></a>Atributo DeleteType

|**Valor**|**Descrição**|
|:-----|:-----|
|HardDelete  <br/> |Um item é removido permanentemente do armazenamento.  <br/> |
|SoftDelete  <br/> |Um item é movido para a lixeira se a lixeira estiver habilitada.  <br/> |
|MoveToDeletedItems  <br/> |Um item é movido para a Itens Excluídos.  <br/> |
   
#### <a name="sendmeetingcancellations-attribute"></a>Atributo SendMeetingCancellations

|**Valor**|**Descrição**|
|:-----|:-----|
|SendToNone  <br/> |Um item de calendário é excluído sem enviar uma mensagem de cancelamento.  <br/> |
|SendOnlyToAll  <br/> |Um item de calendário é excluído e uma mensagem de cancelamento é enviada a todos os participantes.  <br/> |
|SendToAllAndSaveCopy  <br/> |Um item de calendário é excluído e uma mensagem de cancelamento é enviada a todos os participantes. Uma cópia da mensagem de cancelamento é salva na pasta Itens Enviados.  <br/> |
   
#### <a name="affectedtaskoccurrences-attribute"></a>Atributo AffectedTaskOccurrences

|**Valor**|**Descrição**|
|:-----|:-----|
|AllOccurrences  <br/> |Uma solicitação de item de exclusão exclui a tarefa mestra e, portanto, todas as tarefas recorrentes associadas à tarefa mestra.  <br/> |
|SpecifiedOccurrenceOnly  <br/> |Uma solicitação de item de exclusão exclui apenas ocorrências específicas de uma tarefa.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ItemIds](itemids.md) <br/> |Contém uma matriz de itens, itens de ocorrência e itens mestras recorrentes para excluir de uma caixa de correio no Exchange store. A [operação DeleteItem](deleteitem-operation.md) pode ser executada em qualquer tipo de item.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

As **opções MoveToDeletedItems** e **HardDelete** são transacionais, o que significa que, quando uma chamada de serviço Web é concluída, o banco de dados moveu o item para a pasta Itens Excluídos ou removeu permanentemente o item do banco de dados Exchange. Esse comportamento é o mesmo para o MicrosoftExchange Server 2007 e Exchange Server 2010. 
  
A **opção SoftDelete** funciona de forma diferente para versões de destino diferentes Exchange. **SoftDelete** para Exchange 2007 define um pouco sobre o item que indica para o banco de dados Exchange que o item será movido para a pasta de lixeira em um momento indeterminado no futuro. **SoftDelete** para Exchange 2010 move imediatamente o item para a lixeira. **SoftDelete** não é uma opção para exclusão de pasta. **As pesquisas transmissões do SoftDelete** para itens e pastas não retornarão nenhum resultado. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [DeleteItemResponse](deleteitemresponse.md)  
- [Operação DeleteItem](deleteitem-operation.md)

