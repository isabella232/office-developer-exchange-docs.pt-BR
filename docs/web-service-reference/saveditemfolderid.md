---
title: SavedItemFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SavedItemFolderId
api_type:
- schema
ms.assetid: 4b8b475c-9ca5-48c9-acb0-8848b53be1ce
description: O elemento SavedItemFolderId identifica a pasta de destino para operações que atualizam, enviam e criam itens em uma caixa de correio.
ms.openlocfilehash: 75245cf842336621aa098c115d62a7802711dd54
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546116"
---
# <a name="saveditemfolderid"></a>SavedItemFolderId

O **elemento SavedItemFolderId** identifica a pasta de destino para operações que atualizam, enviam e criam itens em uma caixa de correio. 
  
```xml
<SavedItemFolderId>
   <FolderId/>
</SavedItemFolderId>
```

```xml
<SavedItemFolderId>
   <DistinguishedFolderId/>
</SavedItemFolderId>
```

**TargetFolderIdType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contém o identificador e a chave de alteração de uma pasta de destino para operações que atualizam, enviam e criam itens no Exchange store.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Identifica uma pasta de destino por um identificador nomeado para operações que atualizem, enviem e criem itens no Exchange store.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CreateItem](createitem.md) <br/> |Define uma solicitação para criar um item no Exchange store.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/CreateItem` <br/> |
|[UpdateItem](updateitem.md) <br/> |Define uma solicitação para atualizar um item no Exchange store.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/UpdateItem` <br/> |
|[SendItem](senditem.md) <br/> |Define uma solicitação para enviar um item no Exchange store.  <br/> Veja a seguir a expressão XPath para este elemento:  <br/>  `/SendItem` <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Falso  <br/> |
   

