---
title: SavedItemFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SavedItemFolderId
api_type:
- schema
ms.assetid: 4b8b475c-9ca5-48c9-acb0-8848b53be1ce
description: O elemento SavedItemFolderId identifica a pasta de destino para operações que atualizar, enviar e criar itens em uma caixa de correio.
ms.openlocfilehash: c57a7fb4abc2f7ee7b599f56f016811d6ff2c21c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825277"
---
# <a name="saveditemfolderid"></a>SavedItemFolderId

O elemento **SavedItemFolderId** identifica a pasta de destino para operações que atualizar, enviar e criar itens em uma caixa de correio. 
  
```xml
<SavedItemFolderId>
   <FolderId/>
</SavedItemFolderId>
```

 **TargetFolderIdType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contém o identificador e alterar a chave de uma pasta de destino para operações de atualização, enviar e crie itens no armazenamento do Exchange.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Identifica uma pasta de destino por um identificador nomeado nas operações que atualizar, enviar e criar itens no armazenamento do Exchange.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CreateItem](createitem.md) <br/> |Define uma solicitação para criar um item no armazenamento do Exchange.  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/CreateItem` <br/> |
|[UpdateItem](updateitem.md) <br/> |Define uma solicitação de atualização de um item no armazenamento do Exchange.  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/UpdateItem` <br/> |
|[SendItem](senditem.md) <br/> |Define uma solicitação para enviar um item no armazenamento do Exchange.  <br/> Este é a expressão XPath para esse elemento:  <br/>  `/SendItem` <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   

