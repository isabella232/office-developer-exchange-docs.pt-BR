---
title: SendItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SendItem
api_type:
- schema
ms.assetid: a966da19-b05a-4504-ac98-91acc1667b9a
description: O elemento SendItem é o elemento raiz em uma solicitação para enviar um item no Exchange store.
ms.openlocfilehash: 2d1613451e7f876f0b612a3249570412e40b4764
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521617"
---
# <a name="senditem"></a>SendItem

O **elemento SendItem** é o elemento raiz em uma solicitação para enviar um item no Exchange store. 
  
```xml
<SendItem SaveItemToFolder="">
   <ItemIds/>
   <SavedItemFolderId/>
</SendItem>
```

 **SendItemType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**SaveItemToFolder** <br/> |Identifica se uma cópia do item enviado está salva. A ação salvar depende do valor **de SaveItemToFolder** e se um [elemento SavedItemFolderId](saveditemfolderid.md) está presente na solicitação. Este elemento é obrigatório.  <br/> |
   
#### <a name="saveitemtofolder-attribute"></a>Atributo SaveItemToFolder

|**Valor**|**Descrição**|
|:-----|:-----|
|**true** <br/> |Se o [elemento SavedItemFolderId](saveditemfolderid.md) não estiver presente, o item será salvo na pasta Itens Enviados. Se o [elemento SavedItemFolderId](saveditemfolderid.md) estiver presente, o item será salvo na pasta especificada pelo [elemento SavedItemFolderId.](saveditemfolderid.md)  <br/> |
|**false** <br/> |Se o [elemento SavedItemFolderId](saveditemfolderid.md) não estiver presente, o item não será salvo. Se o [elemento SavedItemFolderId](saveditemfolderid.md) estiver presente, uma resposta de erro será retornada com um elemento [ResponseCode](responsecode.md) que contém o **valor ErrorInvalidSendItemSaveSettings.**  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ItemIds](itemids.md) <br/> |Contém as identidades exclusivas de itens, itens de ocorrência e itens mestras recorrentes que são usados para excluir, enviar, obter, mover ou copiar itens no Exchange store.  <br/> |
|[SavedItemFolderId](saveditemfolderid.md) <br/> |Identifica a pasta de destino para operações que atualizem, enviem e criem itens no Exchange store.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="remarks"></a>Comentários

Se um item na pasta Itens Enviados for enviado, o item enviado será excluído e uma cópia dele será colocada na pasta Itens Enviados.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação SendItem](senditem-operation.md)

