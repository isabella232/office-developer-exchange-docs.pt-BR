---
title: ItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- ItemId
api_type:
- schema
ms.assetid: 3350b597-57a0-4961-8f44-8624946719b4
description: O elemento ItemId contém o identificador exclusivo e a chave de alteração de um item no repositório do Exchange.
localization_priority: Priority
ms.openlocfilehash: d5931702225c6864b1ca60a6f0753b65f65aca30
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44441559"
---
# <a name="itemid"></a>ItemId

O elemento **ItemId** contém o identificador exclusivo e a chave de alteração de um item no repositório do Exchange. 
  
```XML
<ItemId Id="" ChangeKey="" />
```

 **ItemIdtype**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**Id** <br/> |Identifica um item específico no repositório do Exchange. A **ID** diferencia maiúsculas de minúsculas; Portanto, as comparações entre as **IDs** devem diferenciar maiúsculas de minúsculas ou binários.  <br/> |
|**ChangeKey** <br/> | Identifica uma versão específica de um item. <br/><br/>Um **ChangeKey** é necessário para os seguintes cenários: <br/> <br/>– O elemento [UpdateItem](updateitem.md) requer um **ChangeKey** se o atributo **ConflictResolution** estiver definido como autoresolver. Autoresolver é um valor padrão. Se o atributo **ChangeKey** não for incluído, a resposta retornará um valor [ResponseCode](responsecode.md) igual a **ErrorChangeKeyRequired**.  <br/><br/>– O elemento [SendItem](senditem.md) requer um **ChangeKey** para testar se a operação tentada atuará na versão mais recente de um item. Se o atributo **ChangeKey** não estiver incluído no **ItemId** ou se o **ChangeKey** estiver vazio, a resposta retornará um valor de [ResponseCode](responsecode.md) igual a **ErrorStaleObject**.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Representa um item de calendário do Exchange.  <br/> |
|[Contato](contact.md) <br/> |Representa um item de contato do Exchange.  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |Representa um evento quando um item ou pasta é copiado.  <br/> |
|[CreatedEvent](createdevent.md) <br/> |Representa um evento quando um item ou pasta é criado.  <br/> |
|[Excluir (issync)](delete-itemsync.md) <br/> |Identifica um único item a ser excluído no repositório do cliente local.  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |Representa um evento quando um item ou pasta é excluído.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Representa uma lista de distribuição.  <br/> |
|[ExportItemsResponseMessage](exportitemsresponsemessage.md) <br/> |Contém o status e os resultados de uma solicitação para exportar um único item de caixa de correio.  <br/> |
|[FirstOccurrence](firstoccurrence.md) <br/> |Representa a primeira ocorrência de um item de calendário recorrente.  <br/> |
|[GlobalItemIds](globalitemids.md) <br/> |Contém a coleção de identificadores de item para todos os itens de conversa em uma caixa de correio.  <br/> |
|[Ignore](ignore.md) <br/> |Identifica os itens a serem ignorados durante a sincronização.  <br/> |
|[Item](item.md) <br/> |Representa um item genérico do Exchange.  <br/> |
|[Item (UploadItemType)](item-uploaditemtype.md) <br/> |Representa um único item a ser carregado em uma caixa de correio.  <br/> |
|[ItemChange](itemchange.md) <br/> |Contém um identificador de item e as atualizações a serem aplicadas ao item.  <br/><br/> A seguir está a expressão XPath para este elemento: <br/> <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
|[ItemIds](itemids.md) <br/> | Contém as identidades exclusivas de itens, itens de ocorrência e itens mestre recorrentes usados para excluir, enviar, obter, mover ou copiar itens no repositório do Exchange. <br/> <br/>  A seguir estão as expressões XPath para este elemento: <br/> <br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/>  `/MoveItem/ItemIds` <br/>  `/CopyItem//ItemIds` <br/> |
|[ItemIds (NonEmptyArrayOfItemIdsType)](itemids-nonemptyarrayofitemidstype.md) <br/> |Contém uma matriz de identificadores de item que identificam os itens a serem exportados de uma caixa de correio.  <br/> |
|[LastOccurrence](lastoccurrence.md) <br/> |Representa a última ocorrência de um item de calendário recorrente.  <br/> |
|[Caixa de Correio](mailbox.md) <br/> |Identifica um objeto de serviço de diretório do Active Directory habilitado para email.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Representa um cancelamento de reunião no repositório do Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Representa uma reunião no repositório do Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Representa uma solicitação de reunião no repositório do Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Representa uma resposta de reunião no repositório do Exchange.  <br/> |
|[Mensagem](message-ex15websvcsotherref.md) <br/> |Representa uma mensagem de email do Exchange.  <br/> |
|[ModifiedEvent](modifiedevent.md) <br/> |Representa um evento que ocorre quando um item é modificado.  <br/> |
|[MovedEvent](movedevent.md) <br/> |Representa um evento que ocorre quando um item é movido de uma pasta pai para outra pasta pai.  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |Representa um evento que é disparado por um novo item de email em uma caixa de correio.  <br/> |
|[Ocorrência](occurrence.md) <br/> |Representa uma única ocorrência modificada de um item de calendário recorrente.  <br/> |
|[PlayOnPhone (serviços Web do Exchange)](playonphone-exchange-web-services.md) <br/> |Representa uma solicitação para ler um item em um telefone.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Remove um item do repositório do Exchange.  <br/> |
|[RoomList](roomlist.md) <br/> |Representa um endereço de email que identifica uma lista de salas de reunião.  <br/> |
|[Tarefa](task.md) <br/> |Representa uma tarefa no repositório do Exchange.  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |Contém o status e os resultados de uma solicitação para carregar um único item de caixa de correio.  <br/> |
|[Userconfiguration](userconfiguration.md) <br/> |Define um único objeto de configuração do usuário.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação ExportItems](exportitems-operation.md)
- [Operação UploadItems](uploaditems-operation.md) 
- [Operação FindConversation](findconversation-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

