---
title: MovedItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 7d5425ab-1e75-43d1-b801-802ff5139df6
description: O elemento MovedItemId especifica o identificador do item movido pela operação MarkAsJunk.
ms.openlocfilehash: 0775aaed119242fc2a2057fb20807d5be30692e5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509592"
---
# <a name="moveditemid"></a>MovedItemId

O **elemento MovedItemId** especifica o identificador do item movido pela **operação MarkAsJunk.** 
  
```XML
<MovedItemId Id="" ChangeKey=""/>
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|Id  <br/> |O valor do **atributo Id** é o identificador de item do item movido pela **operação MarkAsJunk.** O identificador de item permanecerá o mesmo após a movimentação.  <br/> |
|ChangeKey  <br/> |O valor do atributo **ChangeKey** é a chave de alteração do item movido. A chave de alteração muda depois que o item é movido pela **operação MarkAsJunk.**  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[MarkAsJunkResponseMessage](markasjunkresponsemessage.md)
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |messages.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

