---
title: BlockExternalImages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 5c754dfc-a9e9-4272-9b5f-5fe3db537e62
description: O elemento BlockExternalImages especifica se as imagens externas são bloqueadas em corpos de texto HTML.
ms.openlocfilehash: 82ddb7e53f351324783fa39e3b76c9c0534b8193
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543580"
---
# <a name="blockexternalimages"></a>BlockExternalImages

O **elemento BlockExternalImages** especifica se as imagens externas são bloqueadas em corpos de texto HTML. 
  
```XML
<BlockExternalImages> true | false </BlockExternalImages>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> |Identifica as propriedades de pasta a incluir na resposta GetFolder, FindFolder ou SyncFolderHierarchy.  <br/> |
|[ItemShape](itemshape.md) <br/> |Identifica as propriedades do item e o conteúdo a ser incluído em uma resposta GetItem, FindItem ou SyncFolderItems.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto **true para** o **elemento BlockExternalImages** indica que as imagens externas são bloqueadas em corpos HTML. Um valor **false** indica que imagens externas são permitidas. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Tipo de esquema  <br/> |
|Arquivo de validação  <br/> |types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

