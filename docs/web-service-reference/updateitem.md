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
description: O elemento de UpdateItem define uma solicitação de atualização de um item em uma caixa de correio.
ms.openlocfilehash: 7b9b5f1dcffb95eb127572cb91f92d961c05a77e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/21/2018
ms.locfileid: "19837917"
---
# <a name="updateitem"></a>UpdateItem

O elemento de **UpdateItem** define uma solicitação de atualização de um item em uma caixa de correio. 
  
```XML
<UpdateItem ConflictResolution="" MessageDisposition="" SendMeetingInvitationsOrCancellations="" SuppressReadReceipts="">
   <SavedItemFolderId/>
   <ItemChanges/>
</UpdateItem>
```

 **UpdateItemType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**ConflictResolution** <br/> |Identifica o tipo de resolução de conflito para tentar durante uma atualização. O valor padrão é resolver automaticamente.  <br/> |
|**MessageDisposition** <br/> |Descreve como o item será tratado após ele ser atualizado. O atributo **MessageDisposition** é necessário para itens de mensagem, incluindo mensagens de reunião como cancelamentos de reunião, solicitações de reunião e respostas de reunião.  <br/> |
|**SendMeetingCancellations** <br/> |Descreve como as atualizações de reunião são comunicadas depois que um item de calendário for atualizado. Este atributo é necessário para itens de calendário e ocorrências de item de calendário.  <br/> |
|**SuppressReadReceipts** <br/> |Indica se as confirmações de leitura para o item atualizado devem ser suprimidas. Um valor de texto de **true** indica que devem ser suprimidas confirmações de leitura. Um valor **false** indica que as confirmações de leitura serão enviadas ao remetente. Este atributo é opcional.  <br/> Este atributo foi introduzido no Exchange Server 2013 SP1.  <br/> |
   
#### <a name="conflictresolution-attribute"></a>Atributo ConflictResolution

|**Valor**|**Descrição**|
|:-----|:-----|
|NeverOverwrite  <br/> |Se houver um conflito, a operação de atualização falhará e um erro será retornado.  <br/> |
|Resolver automaticamente  <br/> |A operação de atualização resolve automaticamente qualquer conflito.  <br/> |
|AlwaysOverwrite  <br/> |Se houver um conflito, a operação de atualização substituirá informações.  <br/> |
   
#### <a name="messagedisposition-attribute"></a>Atributo MessageDisposition

|**Valor**|**Descrição**|
|:-----|:-----|
|SaveOnly  <br/> |O item está atualizado e salvos de volta a sua pasta atual.  <br/> |
|SendOnly  <br/> |O item é atualizado e enviado, mas nenhuma cópia é salva.  <br/> |
|SendAndSaveCopy  <br/> |O item é atualizado e uma cópia é salva na pasta identificada pelo elemento [SavedItemFolderId](saveditemfolderid.md) .  <br/> |
   
#### <a name="sendmeetinginvitationsorcancellations-attribute"></a>Atributo SendMeetingCancellations

|**Valor**|**Descrição**|
|:-----|:-----|
|SendToNone  <br/> |O item de calendário é atualizado mas atualizações não são enviadas aos participantes.  <br/> |
|SendOnlyToAll  <br/> |O item de calendário é atualizado e a atualização de reunião é enviada a todos os participantes, mas não é salvo na pasta Itens enviados.  <br/> |
|SendOnlyToChanged  <br/> |O item de calendário é atualizado e a atualização de reunião é enviada apenas aos participantes que são afetados pela alteração na reunião.  <br/> |
|SendToAllAndSaveCopy  <br/> |O item de calendário é atualizado, a atualização de reunião é enviada a todos os participantes e uma cópia é salva na pasta Itens enviados.  <br/> |
|SendToChangedAndSaveCopy  <br/> |O item de calendário é atualizado, a atualização de reunião é enviada a todos os participantes que são afetados pela alteração na reunião e uma cópia é salva na pasta Itens enviados.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SavedItemFolderId](saveditemfolderid.md) <br/> |Identifica a pasta de destino para operações de atualização, enviar e crie itens no armazenamento do Exchange.  <br/> |
|[ItemChanges](itemchanges.md) <br/> |Contém uma matriz de elementos [ItemChange](itemchange.md) que identificam os itens e as atualizações para aplicar aos itens.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação UpdateItem](updateitem-operation.md)

