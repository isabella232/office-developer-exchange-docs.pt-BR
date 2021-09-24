---
title: ReturnNewItemIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: aeef79e4-31e1-4213-b627-9bac676be018
description: O elemento ReturnNewItemIds indica se os identificadores de item de novos itens são retornados na resposta.
ms.openlocfilehash: 93ff4e37c56c3583e81711ba7e3582706d9ef940
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512377"
---
# <a name="returnnewitemids"></a>ReturnNewItemIds

O **elemento ReturnNewItemIds** indica se os identificadores de item de novos itens são retornados na resposta. 
  
```XML
<ReturnNewItemIds/>
```

 **xs:boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CopyItem](copyitem.md) <br/> |Define uma solicitação para copiar um item em uma caixa de correio no Exchange store.  <br/> |
|[MoveItem](moveitem.md) <br/> |Define uma solicitação para mover um item no Exchange store.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto **true** para **o elemento ReturnNewItemIds** indica que os novos identificadores de item são retornados na resposta. Um valor **false** indica que os novos identificadores de item não são retornados na resposta. 
  
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services. Esse elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Falso  <br/> |
   

