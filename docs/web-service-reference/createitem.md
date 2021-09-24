---
title: CreateItem
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
ms.assetid: c3707feb-3fd4-4b8a-a68f-2abadd455163
description: O elemento CreateItem define uma solicitação para criar um item no Exchange store.
ms.openlocfilehash: 7276b88bd3b90edc68d7ac8fd4a7646324eadb61
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526495"
---
# <a name="createitem"></a>CreateItem

O **elemento CreateItem** define uma solicitação para criar um item no Exchange store. 
  
```xml
<CreateItem MessageDisposition="" SendMeetingInvitations="">
   <SavedItemFolderId/>
   <Items/>
</CreateItem>
```

**CreateItemType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|Atributo|Descrição|
|:-----|:-----|
|**MessageDisposition** <br/> |Descreve como o item será manipulado depois que ele for criado. O atributo é necessário para mensagens de email. Esse atributo só é aplicável a mensagens de email.  <br/> |
|**SendMeetingInvitations** <br/> |Descreve como as solicitações de reunião são tratadas após a criação. Esse atributo é necessário para itens de calendário.  <br/> |
   
#### <a name="messagedisposition-attribute"></a>Atributo MessageDisposition

|Valor|Descrição|
|:-----|:-----|
|SaveOnly  <br/> |O item de mensagem é salvo na pasta especificada pelo [elemento SavedItemFolderId.](saveditemfolderid.md) As mensagens podem ser enviadas posteriormente usando a [operação SendItem](senditem-operation.md). Um identificador de item é retornado na resposta. Os identificadores de item não são retornados para nenhum tipo de item, exceto para itens de mensagem. Isso inclui objetos de resposta.  <br/> |
|SendOnly  <br/> |O item é enviado, mas nenhuma cópia é salva na pasta Itens Enviados. Um identificador de item não é retornado na resposta.<br/><br/>**OBSERVAÇÃO**: **CreateItem** não dá suporte ao acesso de representante quando a opção SendOnly é usada porque uma pasta de destino não pode ser especificada com essa opção. A solução alternativa é criar o item, obter o identificador de item e, em seguida, usar a operação SendItem para enviar o item.           |
|SendAndSaveCopy  <br/> |O item é enviado e uma cópia é salva na pasta identificada pelo [elemento SavedItemFolderId.](saveditemfolderid.md) Um identificador de item não é retornado na resposta.<br/><br/>**OBSERVAÇÃO**: As solicitações de reunião não são salvas na pasta identificada pela [propriedade SavedItemFolderId.](saveditemfolderid.md) Para o calendário, somente o local de salvar itens de calendário pode ser especificado pela **propriedade SavedItemFolderId.** Não é possível controlar onde um item de solicitação de reunião é salvo. Somente os itens de calendário associados são copiados e salvos na pasta identificada pela **propriedade SavedItemFolderId.**           |
   
#### <a name="sendmeetinginvitations-attribute"></a>Atributo SendMeetingInvitations

|Valor|Descrição|
|:-----|:-----|
|SendToNone  <br/> |Se o item for uma solicitação de reunião, ele será salvo como um item de calendário, mas não enviado.  <br/> |
|SendOnlyToAll  <br/> |A solicitação de reunião é enviada a todos os participantes, mas não é salva na pasta Itens Enviados.  <br/> |
|SendToAllAndSaveCopy  <br/> |A solicitação de reunião é enviada a todos os participantes e uma cópia é salva na pasta identificada pelo [elemento SavedItemFolderId.](saveditemfolderid.md)  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|Elemento|Descrição|
|:-----|:-----|
|[SavedItemFolderId](saveditemfolderid.md) <br/> |Identifica a pasta de destino onde um novo item pode ser criado. Se o **atributo MessageDisposition** estiver definido como SendOnly, uma mensagem criada será enviada apenas. A mensagem não será colocada na pasta identificada pelo [elemento SavedItemFolderId.](saveditemfolderid.md)  <br/> |
|[Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Contém uma matriz de itens a ser criado na pasta identificada pelo [elemento SavedItemFolderId.](saveditemfolderid.md)  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [CreateItemResponse](createitemresponse.md)  
- [Operação CreateItem](createitem-operation.md)
- [Criando mensagens de email](https://msdn.microsoft.com/library/05bfb83c-2866-427d-a9fe-14ba3cb02793%28Office.15%29.aspx) 
- [Criando contatos (Exchange Web Services)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [Criando tarefas](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx) 
- [Criando compromissos](https://msdn.microsoft.com/library/2385391e-c9e7-4d45-b803-c4ff94d5c94e%28Office.15%29.aspx)

