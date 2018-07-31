---
title: CreateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: c3707feb-3fd4-4b8a-a68f-2abadd455163
description: O elemento de CreateItem define uma solicitação para criar um item no armazenamento do Exchange.
ms.openlocfilehash: 9453323bff07749f5852dae75284c61c0895adb6
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353123"
---
# <a name="createitem"></a>CreateItem

O elemento de **CreateItem** define uma solicitação para criar um item no armazenamento do Exchange. 
  
```xml
<CreateItem MessageDisposition="" SendMeetingInvitations="">
   <SavedItemFolderId/>
   <Items/>
</CreateItem>
```

**CreateItemType**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|Atributo|Descrição|
|:-----|:-----|
|**MessageDisposition** <br/> |Descreve como o item será tratado após sua criação. O atributo é necessário para mensagens de email. Este atributo só é aplicável às mensagens de email.  <br/> |
|**SendMeetingInvitations** <br/> |Descreve como as solicitações de reunião são manipuladas depois que eles são criados. Este atributo é exigido para itens de calendário.  <br/> |
   
#### <a name="messagedisposition-attribute"></a>Atributo MessageDisposition

|Valor|Descrição|
|:-----|:-----|
|SaveOnly  <br/> |O item de mensagem é salvo na pasta especificada pelo elemento [SavedItemFolderId](saveditemfolderid.md) . Mensagens podem ser enviadas posteriormente usando a [operação SendItem](senditem-operation.md). Um identificador de item é retornado na resposta. Identificadores de item não são retornados para todos os tipos de item, exceto itens de mensagem. Isso inclui objetos de resposta.  <br/> |
|SendOnly  <br/> |O item é enviado, mas nenhuma cópia é salva na pasta Itens enviados. Um identificador de item não será retornado na resposta.<br/><br/>**Observação**: **CreateItem** não oferece suporte a acesso de representante quando a opção SendOnly é usada como uma pasta de destino não pode ser especificada com essa opção. A solução alternativa é criar o item, obtenha o identificador do item e, em seguida, use a operação SendItem para enviar o item.           |
|SendAndSaveCopy  <br/> |O item será enviado e uma cópia é salva na pasta que é identificada pelo elemento [SavedItemFolderId](saveditemfolderid.md) . Um identificador de item não será retornado na resposta.<br/><br/>**Observação**: solicitações de reunião não são salvas na pasta que é identificado pela propriedade [SavedItemFolderId](saveditemfolderid.md) . Para o calendário, somente o salvar local dos itens do calendário pode ser especificada pela propriedade **SavedItemFolderId** . Não é possível controlar onde uma solicitação de reunião item é salva. Apenas os itens de calendário associadas são copiados e salvo na pasta que é identificada pela propriedade **SavedItemFolderId** .           |
   
#### <a name="sendmeetinginvitations-attribute"></a>Atributo SendMeetingInvitations

|Valor|Descrição|
|:-----|:-----|
|SendToNone  <br/> |Se o item tem uma solicitação de reunião, ele é salvo como um item de calendário, mas não enviado.  <br/> |
|SendOnlyToAll  <br/> |A solicitação de reunião é enviada a todos os participantes, mas não é salvo na pasta Itens enviados.  <br/> |
|SendToAllAndSaveCopy  <br/> |A solicitação de reunião é enviada a todos os participantes e uma cópia é salva na pasta que é identificada pelo elemento [SavedItemFolderId](saveditemfolderid.md) .  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|Elemento|Descrição|
|:-----|:-----|
|[SavedItemFolderId](saveditemfolderid.md) <br/> |Identifica a pasta de destino onde um novo item pode ser criado. Se o atributo **MessageDisposition** é definido como SendOnly, uma mensagem criada só será enviada. A mensagem não será colocada na pasta que é identificada pelo elemento [SavedItemFolderId](saveditemfolderid.md) .  <br/> |
|[Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Contém uma matriz de itens para criar a pasta que é identificada pelo elemento [SavedItemFolderId](saveditemfolderid.md) .  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [CreateItemResponse](createitemresponse.md)  
- [Operação CreateItem](createitem-operation.md)
- [Criando mensagens de email](http://msdn.microsoft.com/library/05bfb83c-2866-427d-a9fe-14ba3cb02793%28Office.15%29.aspx) 
- [Criação de contatos (serviços Web do Exchange)](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [Criação de tarefas](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx) 
- [Criando compromissos](http://msdn.microsoft.com/library/2385391e-c9e7-4d45-b803-c4ff94d5c94e%28Office.15%29.aspx)

