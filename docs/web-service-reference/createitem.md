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
description: O elemento CreateItem define uma solicitação para criar um item no repositório do Exchange.
ms.openlocfilehash: 235664b7baeceeccb14135fd346123f0f7d99346
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527058"
---
# <a name="createitem"></a>CreateItem

O elemento **CreateItem** define uma solicitação para criar um item no repositório do Exchange. 
  
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
|**MessageDisposition** <br/> |Descreve como o item será manipulado após a criação. O atributo é necessário para mensagens de email. Este atributo só é aplicável a mensagens de email.  <br/> |
|**SendMeetingInvitations** <br/> |Descreve como as solicitações de reunião são tratadas após serem criadas. Este atributo é obrigatório para itens de calendário.  <br/> |
   
#### <a name="messagedisposition-attribute"></a>Atributo MessageDisposition

|Valor|Descrição|
|:-----|:-----|
|SaveOnly  <br/> |O item de mensagem é salvo na pasta que é especificada pelo elemento [SavedItemFolderId](saveditemfolderid.md) . As mensagens podem ser enviadas posteriormente usando a [operação SendItem](senditem-operation.md). Um identificador de item é retornado na resposta. Os identificadores de item não são retornados para qualquer tipo de item, exceto para itens de mensagem. Isso inclui objetos Response.  <br/> |
|SendOnly  <br/> |O item é enviado, mas nenhuma cópia é salva na pasta Itens enviados. Um identificador de item não é retornado na resposta.<br/><br/>**Observação**: **CreateItem** não é compatível com o acesso de representante quando a opção SendOnly é usada porque uma pasta de destino não pode ser especificada com essa opção. A solução alternativa é criar o item, obter o identificador de item e usar a operação SendItem para enviar o item.           |
|SendAndSaveCopy  <br/> |O item é enviado e uma cópia é salva na pasta identificada pelo elemento [SavedItemFolderId](saveditemfolderid.md) . Um identificador de item não é retornado na resposta.<br/><br/>**Observação**: as solicitações de reunião não são salvas na pasta identificada pela propriedade [SavedItemFolderId](saveditemfolderid.md) . Para o calendário, somente o local de salvamento dos itens de calendário pode ser especificado pela propriedade **SavedItemFolderId** . Você não pode controlar onde um item de solicitação de reunião é salvo. Somente os itens de calendário associados são copiados e salvos na pasta identificada pela propriedade **SavedItemFolderId** .           |
   
#### <a name="sendmeetinginvitations-attribute"></a>Atributo SendMeetingInvitations

|Valor|Descrição|
|:-----|:-----|
|SendToNone  <br/> |Se o item for uma solicitação de reunião, ele será salvo como um item de calendário, mas não será enviado.  <br/> |
|SendOnlyToAll  <br/> |A solicitação de reunião é enviada a todos os participantes, mas não é salva na pasta Itens enviados.  <br/> |
|SendToAllAndSaveCopy  <br/> |A solicitação de reunião é enviada a todos os participantes e uma cópia é salva na pasta identificada pelo elemento [SavedItemFolderId](saveditemfolderid.md) .  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|Elemento|Descrição|
|:-----|:-----|
|[SavedItemFolderId](saveditemfolderid.md) <br/> |Identifica a pasta de destino onde um novo item pode ser criado. Se o atributo **MessageDisposition** for definido como SendOnly, uma mensagem criada será enviada apenas. A mensagem não será colocada na pasta que é identificada pelo elemento [SavedItemFolderId](saveditemfolderid.md) .  <br/> |
|[Itens (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Contém uma matriz de itens a serem criados na pasta que é identificada pelo elemento [SavedItemFolderId](saveditemfolderid.md) .  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
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
- [Criar mensagens de email](https://msdn.microsoft.com/library/05bfb83c-2866-427d-a9fe-14ba3cb02793%28Office.15%29.aspx) 
- [Criando contatos (serviços Web do Exchange)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [Criando tarefas](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx) 
- [Criar compromissos](https://msdn.microsoft.com/library/2385391e-c9e7-4d45-b803-c4ff94d5c94e%28Office.15%29.aspx)

