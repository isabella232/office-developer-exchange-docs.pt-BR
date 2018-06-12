---
title: ItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemId
api_type:
- schema
ms.assetid: 3350b597-57a0-4961-8f44-8624946719b4
description: O elemento de ItemId contém o identificador e alterar a chave exclusiva de um item no armazenamento do Exchange.
ms.openlocfilehash: 9c5d71a23e1e4b77d2a50016aa4d765d872d04cc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824157"
---
# <a name="itemid"></a>ItemId

O elemento de **ItemId** contém o identificador e alterar a chave exclusiva de um item no armazenamento do Exchange. 
  
```XML
<ItemId Id="" ChangeKey="" />
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**ID de** <br/> |Identifica um item específico no armazenamento do Exchange. **ID** diferencia maiusculas de minúsculas; Portanto, as comparações entre **Ids** devem ser diferencia maiusculas de minúsculas ou binários.  <br/> |
|**ChangeKey** <br/> | Identifica uma versão específica de um item. <br/><br/>Um **ChangeKey** é necessária para os seguintes cenários: <br/> <br/>-O elemento [UpdateItem](updateitem.md) requer um **ChangeKey** se o atributo **ConflictResolution** estiver definido como resolver automaticamente. Resolver automaticamente é um valor padrão. Se o atributo **ChangeKey** não for incluído, a resposta retornará um valor [ResponseCode](responsecode.md) igual a **ErrorChangeKeyRequired**.  <br/><br/>-O elemento [SendItem](senditem.md) requer um **ChangeKey** testar se a operação tentada atuará após a versão mais recente de um item. Se o atributo **ChangeKey** não está incluído no **ItemId** ou se o **ChangeKey** estiver vazia, a resposta retornará um valor [ResponseCode](responsecode.md) igual a **ErrorStaleObject**.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Representa um item de calendário do Exchange.  <br/> |
|[Contato](contact.md) <br/> |Representa um item de contato do Exchange.  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |Representa um evento quando uma pasta ou um item é copiado.  <br/> |
|[CreatedEvent](createdevent.md) <br/> |Representa um evento quando uma pasta ou um item é criada.  <br/> |
|[Excluir (ItemSync)](delete-itemsync.md) <br/> |Identifica um único item a ser excluído no repositório de cliente local.  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |Representa um evento quando uma pasta ou um item é excluída.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Representa uma lista de distribuição.  <br/> |
|[ExportItemsResponseMessage](exportitemsresponsemessage.md) <br/> |Contém o status e os resultados de uma solicitação para exportar um item de caixa de correio única.  <br/> |
|[FirstOccurrence](firstoccurrence.md) <br/> |Representa a primeira ocorrência de um item de calendário recorrente.  <br/> |
|[GlobalItemIds](globalitemids.md) <br/> |Contém o conjunto de identificadores de item para todos os itens de conversa em uma caixa de correio.  <br/> |
|[Ignore](ignore.md) <br/> |Identifica os itens a serem ignorados durante a sincronização.  <br/> |
|[1.1](item.md) <br/> |Representa um item genérico do Exchange.  <br/> |
|[Item (UploadItemType)](item-uploaditemtype.md) <br/> |Representa um único item para carregar em uma caixa de correio.  <br/> |
|[ItemChange](itemchange.md) <br/> |Contém um identificador de item e as atualizações para aplicar ao item.  <br/><br/> Este é a expressão XPath para esse elemento: <br/> <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
|[ItemIds](itemids.md) <br/> | Contém as identidades exclusivas dos itens, itens de ocorrência e itens recorrentes mestres, usados para excluir, enviar, obter, mover ou copiar itens no armazenamento do Exchange. <br/> <br/>  A seguir estão as expressões XPath para esse elemento: <br/> <br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/>  `/MoveItem/ItemIds` <br/>  `/CopyItem//ItemIds` <br/> |
|[ItemIds (NonEmptyArrayOfItemIdsType)](itemids-nonemptyarrayofitemidstype.md) <br/> |Contém uma matriz de identificadores de item que identificam os itens para exportar de uma caixa de correio.  <br/> |
|[LastOccurrence](lastoccurrence.md) <br/> |Representa a última ocorrência de um item de calendário recorrente.  <br/> |
|[Caixa de correio](mailbox.md) <br/> |Identifica um objeto de serviço de diretório do Active Directory habilitado para email.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Representa o cancelamento da reunião no armazenamento do Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Representa uma reunião no armazenamento do Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no armazenamento do Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Representa uma resposta de reunião no armazenamento do Exchange.  <br/> |
|[Mensagem](message-ex15websvcsotherref.md) <br/> |Representa uma mensagem de email do Exchange.  <br/> |
|[ModifiedEvent](modifiedevent.md) <br/> |Representa um evento que ocorre quando um item é modificado.  <br/> |
|[MovedEvent](movedevent.md) <br/> |Representa um evento que ocorre quando um item é movido da pasta pai de um para outra pasta pai.  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |Representa um evento que é disparado por um novo item de email em uma caixa de correio.  <br/> |
|[Ocorrência](occurrence.md) <br/> |Representa uma única ocorrência de modificação de um item de calendário recorrente.  <br/> |
|[PlayOnPhone (serviços Web do Exchange)](playonphone-exchange-web-services.md) <br/> |Representa uma solicitação para ler um item em um telefone.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Remove um item de armazenamento do Exchange.  <br/> |
|[RoomList](roomlist.md) <br/> |Representa um endereço de email que identifica uma lista de salas de reunião.  <br/> |
|[Task](task.md) <br/> |Representa uma tarefa no armazenamento do Exchange.  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |Contém o status e os resultados de uma solicitação para carregar um item de caixa de correio única.  <br/> |
|[UserConfiguration](userconfiguration.md) <br/> |Define um objeto de configuração de usuário único.  <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Operação ExportItems](exportitems-operation.md)
- [Operação UploadItems](uploaditems-operation.md) 
- [Operação FindConversation](findconversation-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

