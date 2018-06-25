---
title: SizeRequested
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e86f98b6-83b5-4530-80eb-dc5df42e2c62
description: O elemento SizeRequested contém o tamanho da foto solicitada para uma operação de GetUserPhoto.
ms.openlocfilehash: 43e422512b1e8f06e410e533e9ae1dc49283d5f6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825504"
---
# <a name="sizerequested"></a>SizeRequested

O elemento **SizeRequested** contém o tamanho da foto solicitada para uma operação de **GetUserPhoto** . 
  
```XML
<SizeRequested>HR48x48 | HR64x64 | HR96X96 | HR120X120 | HR240X240 | HR360X360 | HR432X432 | HR504X504 | HR648X648</SizeRequested>
```

 **UserPhotoSizeType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[GetUserPhoto](getuserphoto.md)
  
## <a name="text-value"></a>Text value

O valor de texto do elemento **SizeRequested** é o tamanho da foto solicitados de uma imagem digital retornada do servidor. A tabela a seguir identifica os valores de texto para o elemento **SizeRequested** . 
  
|**Valor**|**Significado**|
|:-----|:-----|
|HR48x48  <br/> |A imagem é 48 pixels de altura e 48 pixels de largura.  <br/> |
|HR64x64  <br/> |A imagem é 64 pixels de altura e 64 pixels de largura.  <br/> |
|HR96x96  <br/> |A imagem é 96 pixels de altura e 96 pixels de largura.  <br/> |
|HR120x120  <br/> |A imagem é 120 pixels de altura e largura em 120 pixels.  <br/> |
|HR240x240  <br/> |A imagem é 240 pixels de altura e 240 pixels de largura.  <br/> |
|HR360x360  <br/> |A imagem é 360 pixels de altura e largura de 360 pixels.  <br/> |
|HR432x432  <br/> |A imagem é 432 pixels de altura e largura em 432 pixels.  <br/> |
|HR504x504  <br/> |A imagem é 504 pixels de altura e largura 504 pixels.  <br/> |
|HR648x648  <br/> |A imagem é 648 pixels de altura e 648 pixels de largura.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

