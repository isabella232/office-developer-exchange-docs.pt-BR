---
title: MovedItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7d5425ab-1e75-43d1-b801-802ff5139df6
description: O elemento MovedItemId especifica o identificador do item que foi movido pela operação MarkAsJunk.
ms.openlocfilehash: 5cf8800ec672278691348bbcd8c6c8cc7a12905b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468611"
---
# <a name="moveditemid"></a>MovedItemId

O elemento **MovedItemId** especifica o identificador do item que foi movido pela operação **MarkAsJunk** . 
  
```XML
<MovedItemId Id="" ChangeKey=""/>
```

 **ItemIdtype**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|Id  <br/> |O valor do atributo **ID** é o identificador do item que é movido pela operação **MarkAsJunk** . O identificador de item permanecerá o mesmo após a movimentação.  <br/> |
|ChangeKey  <br/> |O valor do atributo **ChangeKey** é a chave de alteração do item movido. A chave Change muda após o item ser movido pela operação **MarkAsJunk** .  <br/> |
   
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
|Arquivo de validação  <br/> |messages. xsd  <br/> |
|Pode estar vazio  <br/> ||
   

