---
title: DeleteItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItem
api_type:
- schema
ms.assetid: 055cdee8-3c7d-47db-9f27-740f4a674729
description: O elemento DeleteItem define uma solicitação para excluir um item de uma caixa de correio no repositório do Exchange.
ms.openlocfilehash: ed13ee32b487f49740aed80e8705257d3e2e6938
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529200"
---
# <a name="deleteitem"></a>DeleteItem

O elemento **DeleteItem** define uma solicitação para excluir um item de uma caixa de correio no repositório do Exchange. 
  
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
|**SendMeetingCancellations** <br/> |Descreve se uma exclusão de item de calendário é comunicada aos participantes. Esse atributo é obrigatório quando os itens de calendário são excluídos. Esse atributo é opcional se itens que não são de calendário são excluídos.  <br/> |
|**AffectedTaskOccurrences** <br/> |Descreve se uma instância de tarefa ou um mestre de tarefa é excluído por uma [Operação DeleteItem](deleteitem-operation.md). Esse atributo é necessário quando as tarefas são excluídas. Este atributo é opcional quando itens de não tarefa são excluídos.  <br/> |
|**SuppressReadReceipts** <br/> |Indica se as confirmações de leitura para o item excluído são suprimidas. Um valor de texto **true**, indica que as confirmações de leitura são suprimidas. Um valor **false** indica que as confirmações de leitura são enviadas para o remetente. Esse atributo é opcional.  <br/> |
   
#### <a name="deletetype-attribute"></a>Atributo DeleteType

|**Valor**|**Descrição**|
|:-----|:-----|
|HardDelete  <br/> |Um item é removido permanentemente da loja.  <br/> |
|SoftDelete  <br/> |Um item será movido para o dumpster se o dumpster estiver habilitado.  <br/> |
|MoveToDeletedItems  <br/> |Um item é movido para a Itens Excluídos.  <br/> |
   
#### <a name="sendmeetingcancellations-attribute"></a>Atributo SendMeetingCancellations

|**Valor**|**Descrição**|
|:-----|:-----|
|SendToNone  <br/> |Um item de calendário é excluído sem enviar uma mensagem de cancelamento.  <br/> |
|SendOnlyToAll  <br/> |Um item de calendário é excluído e uma mensagem de cancelamento é enviada a todos os participantes.  <br/> |
|SendToAllAndSaveCopy  <br/> |Um item de calendário é excluído e uma mensagem de cancelamento é enviada a todos os participantes. Uma cópia da mensagem de cancelamento é salva na pasta Itens enviados.  <br/> |
   
#### <a name="affectedtaskoccurrences-attribute"></a>Atributo AffectedTaskOccurrences

|**Valor**|**Descrição**|
|:-----|:-----|
|Todas as ocorrências  <br/> |Uma solicitação de exclusão de item exclui a tarefa mestre e, portanto, todas as tarefas recorrentes associadas à tarefa mestre.  <br/> |
|SpecifiedOccurrenceOnly  <br/> |Uma solicitação de exclusão de item exclui apenas ocorrências específicas de uma tarefa.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ItemIds](itemids.md) <br/> |Contém uma matriz de itens, itens de ocorrência e itens mestres recorrentes para excluir de uma caixa de correio no repositório do Exchange. A [Operação DeleteItem](deleteitem-operation.md) pode ser executada em qualquer tipo de item.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="remarks"></a>Comentários

As opções **MoveToDeletedItems** e **HardDelete** são transacionais, o que significa que, quando uma chamada de serviço Web é concluída, o banco de dados moveu o item para a pasta itens excluídos ou removeu permanentemente o item do banco de dados do Exchange. Esse comportamento é o mesmo para o MicrosoftExchange Server 2007 e o Exchange Server 2010. 
  
A opção **SoftDelete** funciona de forma diferente para diferentes versões de destino do Exchange. **SoftDelete** para o Exchange 2007 define um bit no item que indica ao banco de dados do Exchange que o item será movido para a pasta dumpster em um momento indeterminado no futuro. **SoftDelete** para Exchange 2010 move imediatamente o item para o dumpster. **SoftDelete** não é uma opção para exclusão de pasta. **SoftDelete** passagem pesquisa por itens e pastas não retornará nenhum resultado. 
  
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

