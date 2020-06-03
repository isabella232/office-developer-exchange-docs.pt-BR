---
title: BlockExternalImages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c754dfc-a9e9-4272-9b5f-5fe3db537e62
description: O elemento BlockExternalImages especifica se as imagens externas são bloqueadas em corpos de texto HTML.
ms.openlocfilehash: 73342316024ebe476a0e35f14157befc80edcf83
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527401"
---
# <a name="blockexternalimages"></a>BlockExternalImages

O elemento **BlockExternalImages** especifica se as imagens externas são bloqueadas em corpos de texto HTML. 
  
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
|[FolderShape](foldershape.md) <br/> |Identifica as propriedades da pasta a serem incluídas na resposta GetFolder, FindFolder ou SyncFolderHierarchy.  <br/> |
|[Shape](itemshape.md) <br/> |Identifica as propriedades e o conteúdo do item que serão incluídos em uma resposta GetItem, FindItem ou SyncFolderItems.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto **true** para o elemento **BlockExternalImages** indica que as imagens externas são bloqueadas em corpos de HTML. Um valor **false** indica que as imagens externas são permitidas. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipo  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

