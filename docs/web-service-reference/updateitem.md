---
title: UpdateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: 34643d58-2743-45b0-a08d-bff6dc1da61d
description: O elemento UpdateItem define uma solicitação para atualizar um item em uma caixa de correio.
ms.openlocfilehash: 43821db58457ffce22be918a7ba6427f57230010
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466567"
---
# <a name="updateitem"></a>UpdateItem

O elemento **UpdateItem** define uma solicitação para atualizar um item em uma caixa de correio. 
  
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
|**ConflictResolution** <br/> |Identifica o tipo de resolução de conflitos a ser tentada durante uma atualização. O valor padrão é autoresolver.  <br/> |
|**MessageDisposition** <br/> |Descreve como o item será manipulado após a atualização. O atributo **MessageDisposition** é necessário para itens de mensagem, incluindo mensagens de reunião, como cancelamentos de reunião, solicitações de reunião e respostas de reunião.  <br/> |
|**SendMeetingInvitationsOrCancellations** <br/> |Descreve como as atualizações de reunião são comunicadas após a atualização de um item de calendário. Esse atributo é necessário para itens de calendário e ocorrências de itens de calendário.  <br/> |
|**SuppressReadReceipts** <br/> |Indica se as confirmações de leitura para o item atualizado devem ser suprimidas. Um valor de texto **true** indica que as confirmações de leitura devem ser suprimidas. Um valor **false** indica que as confirmações de leitura serão enviadas ao remetente. Esse atributo é opcional.  <br/> Este atributo foi introduzido no Exchange Server 2013 SP1.  <br/> |
   
#### <a name="conflictresolution-attribute"></a>Atributo ConflictResolution

|**Valor**|**Descrição**|
|:-----|:-----|
|NeverOverwrite  <br/> |Se houver um conflito, a operação de atualização falhará e um erro será retornado.  <br/> |
|Resolver automaticamente  <br/> |A operação de atualização resolve qualquer conflito automaticamente.  <br/> |
|AlwaysOverwrite  <br/> |Se houver um conflito, a operação de atualização substituirá as informações.  <br/> |
   
#### <a name="messagedisposition-attribute"></a>Atributo MessageDisposition

|**Valor**|**Descrição**|
|:-----|:-----|
|SaveOnly  <br/> |O item é atualizado e salvo novamente na pasta atual.  <br/> |
|SendOnly  <br/> |O item é atualizado e enviado, mas nenhuma cópia é salva.  <br/> |
|SendAndSaveCopy  <br/> |O item é atualizado e uma cópia é salva na pasta identificada pelo elemento [SavedItemFolderId](saveditemfolderid.md) .  <br/> |
   
#### <a name="sendmeetinginvitationsorcancellations-attribute"></a>Atributo SendMeetingInvitationsOrCancellations

|**Valor**|**Descrição**|
|:-----|:-----|
|SendToNone  <br/> |O item de calendário é atualizado, mas as atualizações não são enviadas aos participantes.  <br/> |
|SendOnlyToAll  <br/> |O item de calendário é atualizado e a atualização da reunião é enviada a todos os participantes, mas não é salvo na pasta Itens enviados.  <br/> |
|SendOnlyToChanged  <br/> |O item de calendário é atualizado e a atualização da reunião é enviada somente para os participantes afetados pela alteração na reunião.  <br/> |
|SendToAllAndSaveCopy  <br/> |O item de calendário é atualizado, a atualização da reunião é enviada a todos os participantes e uma cópia é salva na pasta Itens enviados.  <br/> |
|SendToChangedAndSaveCopy  <br/> |O item de calendário é atualizado, a atualização da reunião é enviada a todos os participantes afetados pela alteração na reunião, e uma cópia é salva na pasta Itens enviados.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SavedItemFolderId](saveditemfolderid.md) <br/> |Identifica a pasta de destino para operações que atualizam, enviam e criam itens no repositório do Exchange.  <br/> |
|[Alterações](itemchanges.md) <br/> |Contém uma matriz de elementos [ItemChange](itemchange.md) que identificam itens e as atualizações a serem aplicadas aos itens.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
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

