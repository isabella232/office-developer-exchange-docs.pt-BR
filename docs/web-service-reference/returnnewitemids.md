---
title: ReturnNewItemIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: aeef79e4-31e1-4213-b627-9bac676be018
description: O elemento ReturnNewItemIds indica se os identificadores de item de novos itens são retornados na resposta.
ms.openlocfilehash: 6d3bc83c05a82d6e448041167676f41c2620dcd4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825232"
---
# <a name="returnnewitemids"></a>ReturnNewItemIds

O elemento **ReturnNewItemIds** indica se os identificadores de item de novos itens são retornados na resposta. 
  
```XML
<ReturnNewItemIds/>
```

 **xs:Boolean**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[CopyItem](copyitem.md) <br/> |Define uma solicitação para copiar um item em uma caixa de correio no armazenamento do Exchange.  <br/> |
|[MoveItem](moveitem.md) <br/> |Define uma solicitação para mover um item no armazenamento do Exchange.  <br/> |
   
## <a name="text-value"></a>Text value

Um valor de texto de **true** para o elemento **ReturnNewItemIds** indica se os identificadores de item novo são retornados na resposta. Um valor **false** indica se os identificadores de item novo não são retornados na resposta. 
  
## <a name="remarks"></a>Coment�rios

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagem  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   

