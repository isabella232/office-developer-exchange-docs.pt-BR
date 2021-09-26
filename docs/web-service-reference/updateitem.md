---
title: UpdateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: 34643d58-2743-45b0-a08d-bff6dc1da61d
description: O elemento UpdateItem define uma solicitação para atualizar um item em uma caixa de correio.
ms.openlocfilehash: 544ccfb8c42b2a4d4f69ae04d383233203c235b8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542783"
---
# <a name="updateitem"></a>UpdateItem

O **elemento UpdateItem** define uma solicitação para atualizar um item em uma caixa de correio. 
  
```XML
<UpdateItem ConflictResolution="" MessageDisposition="" SendMeetingInvitationsOrCancellations="" SuppressReadReceipts="">
   <SavedItemFolderId/>
   <ItemChanges/>
</UpdateItem>
```

 **UpdateItemType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**ConflictResolution** <br/> |Identifica o tipo de resolução de conflitos a ser tentada durante uma atualização. O valor padrão é AutoResolve.  <br/> |
|**MessageDisposition** <br/> |Descreve como o item será manipulado depois de atualizado. O **atributo MessageDisposition** é necessário para itens de mensagem, incluindo mensagens de reunião, como cancelamentos de reunião, solicitações de reunião e respostas de reunião.  <br/> |
|**SendMeetingInvitationsOrCancellations** <br/> |Descreve como as atualizações de reunião são comunicadas depois que um item de calendário é atualizado. Esse atributo é necessário para itens de calendário e ocorrências de item de calendário.  <br/> |
|**SuppressReadReceipts** <br/> |Indica se os recibos de leitura do item atualizado devem ser suprimidos. Um valor de texto **true** indica que os recibos de leitura devem ser suprimidos. Um valor **false** indica que os recibos de leitura serão enviados ao remetente. Esse atributo é opcional.  <br/> Esse atributo foi introduzido no Exchange Server 2013 SP1.  <br/> |
   
#### <a name="conflictresolution-attribute"></a>Atributo ConflictResolution

|**Valor**|**Descrição**|
|:-----|:-----|
|NeverOverwrite  <br/> |Se houver um conflito, a operação de atualização falhará e um erro será retornado.  <br/> |
|AutoResolve  <br/> |A operação de atualização resolve automaticamente qualquer conflito.  <br/> |
|AlwaysOverwrite  <br/> |Se houver um conflito, a operação de atualização substituirá informações.  <br/> |
   
#### <a name="messagedisposition-attribute"></a>Atributo MessageDisposition

|**Valor**|**Descrição**|
|:-----|:-----|
|SaveOnly  <br/> |O item é atualizado e salvo de volta à pasta atual.  <br/> |
|SendOnly  <br/> |O item é atualizado e enviado, mas nenhuma cópia é salva.  <br/> |
|SendAndSaveCopy  <br/> |O item é atualizado e uma cópia é salva na pasta identificada pelo [elemento SavedItemFolderId.](saveditemfolderid.md)  <br/> |
   
#### <a name="sendmeetinginvitationsorcancellations-attribute"></a>Atributo SendMeetingInvitationsOrCancellations

|**Valor**|**Descrição**|
|:-----|:-----|
|SendToNone  <br/> |O item de calendário é atualizado, mas as atualizações não são enviadas aos participantes.  <br/> |
|SendOnlyToAll  <br/> |O item de calendário é atualizado e a atualização da reunião é enviada a todos os participantes, mas não é salva na pasta Itens Enviados.  <br/> |
|SendOnlyToChanged  <br/> |O item de calendário é atualizado e a atualização da reunião é enviada somente aos participantes afetados pela alteração na reunião.  <br/> |
|SendToAllAndSaveCopy  <br/> |O item de calendário é atualizado, a atualização da reunião é enviada a todos os participantes e uma cópia é salva na pasta Itens Enviados.  <br/> |
|SendToChangedAndSaveCopy  <br/> |O item de calendário é atualizado, a atualização da reunião é enviada a todos os participantes afetados pela alteração na reunião e uma cópia é salva na pasta Itens Enviados.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SavedItemFolderId](saveditemfolderid.md) <br/> |Identifica a pasta de destino para operações que atualizem, enviem e criem itens no Exchange store.  <br/> |
|[ItemChanges](itemchanges.md) <br/> |Contém uma matriz de [elementos ItemChange](itemchange.md) que identificam itens e as atualizações a aplicar aos itens.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação UpdateItem](updateitem-operation.md)

