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
description: O elemento de DeleteItem define uma solicitação para excluir um item de uma caixa de correio no armazenamento do Exchange.
ms.openlocfilehash: de64787750c88c8a47bb69daddc0a1d2ebe8bde9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751758"
---
# <a name="deleteitem"></a>DeleteItem

O elemento de **DeleteItem** define uma solicitação para excluir um item de uma caixa de correio no armazenamento do Exchange. 
  
```XML
<DeleteItem DeleteType="" SendMeetingCancellations="" AffectedTaskOccurrences="" SuppressReadReceipts="">
   <ItemIds/>
</DeleteItem>
```

 **DeleteItemType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**DeleteType** <br/> |Descreve como um item é excluído. Este atributo é necessário.  <br/> |
|**SendMeetingCancellations** <br/> |Descreve se uma exclusão de item de calendário é comunicada aos participantes. Este atributo é necessário quando itens de calendário são excluídas. Este atributo é opcional se os itens de calendário não são excluídos.  <br/> |
|**AffectedTaskOccurrences** <br/> |Descreve se uma instância de tarefa ou um mestre de tarefa é excluído por uma [operação DeleteItem](deleteitem-operation.md). Este atributo é necessário quando as tarefas são excluídas. Este atributo é opcional quando os itens de tarefa não são excluídos.  <br/> |
|**SuppressReadReceipts** <br/> |Indica se as confirmações de leitura para o item excluído são suprimidas. Um valor de texto de **true**, indica que as confirmações de leitura estão suprimidas. Um valor **false** indica que as confirmações de leitura são enviadas para o remetente. Este atributo é opcional.  <br/> |
   
#### <a name="deletetype-attribute"></a>Atributo DeleteType

|**Valor**|**Descrição**|
|:-----|:-----|
|HardDelete  <br/> |Um item é removido permanentemente do repositório.  <br/> |
|SoftDelete  <br/> |Um item é movido para o dumpster se o dumpster está habilitado.  <br/> |
|MoveToDeletedItems  <br/> |Um item é movido para a pasta Itens excluídos.  <br/> |
   
#### <a name="sendmeetingcancellations-attribute"></a>Atributo SendMeetingCancellations

|**Valor**|**Descrição**|
|:-----|:-----|
|SendToNone  <br/> |Um item de calendário será excluído sem enviar uma mensagem de cancelamento.  <br/> |
|SendOnlyToAll  <br/> |Um item de calendário é excluído e uma mensagem de cancelamento é enviada a todos os participantes.  <br/> |
|SendToAllAndSaveCopy  <br/> |Um item de calendário é excluído e uma mensagem de cancelamento é enviada a todos os participantes. Uma cópia da mensagem de cancelamento é salva na pasta Itens enviados.  <br/> |
   
#### <a name="affectedtaskoccurrences-attribute"></a>Atributo AffectedTaskOccurrences

|**Valor**|**Descrição**|
|:-----|:-----|
|AllOccurrences  <br/> |Uma solicitação de item delete Exclui a tarefa mestre e, portanto, todas as tarefas recorrentes que estão associados a tarefa mestre.  <br/> |
|SpecifiedOccurrenceOnly  <br/> |Uma solicitação de item delete Exclui apenas as ocorrências específicas de uma tarefa.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ItemIds](itemids.md) <br/> |Contém uma matriz de itens, itens de ocorrência e itens recorrentes de mestres para excluir de uma caixa de correio no armazenamento do Exchange. A [operação DeleteItem](deleteitem-operation.md) pode ser executado em qualquer tipo de item.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

As opções **MoveToDeletedItems** e **HardDelete** são transacionais, o que significa que no momento em uma chamada de serviço da Web for concluído, o banco de dados tiver movido o item para a pasta Itens excluídos ou removido permanentemente o item do banco de dados do Exchange. Esse comportamento é o mesmo para MicrosoftExchange Server 2007 e o Exchange Server 2010. 
  
A opção **SoftDelete** funciona de modo diferente para versões diferentes de destino do Exchange. **SoftDelete** para o Exchange 2007 define um pouco no item que indica no banco de dados do Exchange que o item será movido para o dumpster pasta em um tempo indeterminado no futuro. **SoftDelete** para o Exchange 2010 imediatamente move o item para o dumpster. **SoftDelete** não é uma opção para exclusão da pasta. Pesquisas de passagem **SoftDelete** para itens e pastas não retornará nenhum resultado. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [DeleteItemResponse](deleteitemresponse.md)  
- [Operação DeleteItem](deleteitem-operation.md)

