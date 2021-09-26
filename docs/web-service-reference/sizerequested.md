---
title: SizeRequested
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: e86f98b6-83b5-4530-80eb-dc5df42e2c62
description: O elemento SizeRequested contém o tamanho da foto solicitado para uma operação GetUserPhoto.
ms.openlocfilehash: 799869a85d7f72e79753a73f9c259388a2702bf5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545913"
---
# <a name="sizerequested"></a>SizeRequested

O **elemento SizeRequested** contém o tamanho da foto solicitado para uma **operação GetUserPhoto.** 
  
```XML
<SizeRequested>HR48x48 | HR64x64 | HR96X96 | HR120X120 | HR240X240 | HR360X360 | HR432X432 | HR504X504 | HR648X648</SizeRequested>
```

 **UserPhotoSizeType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[GetUserPhoto](getuserphoto.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do **elemento SizeRequested** é o tamanho da foto solicitada de uma imagem digital retornada do servidor. A tabela a seguir identifica os valores de texto do **elemento SizeRequested.** 
  
|**Valor**|**Significado**|
|:-----|:-----|
|HR48x48  <br/> |A imagem tem 48 pixels de altura e 48 pixels de largura.  <br/> |
|HR64x64  <br/> |A imagem tem 64 pixels de altura e 64 pixels de largura.  <br/> |
|HR96x96  <br/> |A imagem tem 96 pixels de altura e 96 pixels de largura.  <br/> |
|HR120x120  <br/> |A imagem tem 120 pixels de altura e 120 pixels de largura.  <br/> |
|HR240x240  <br/> |A imagem tem 240 pixels de altura e 240 pixels de largura.  <br/> |
|HR360x360  <br/> |A imagem tem 360 pixels de altura e 360 pixels de largura.  <br/> |
|HR432x432  <br/> |A imagem tem 432 pixels de altura e 432 pixels de largura.  <br/> |
|HR504x504  <br/> |A imagem tem 504 pixels de altura e 504 pixels de largura.  <br/> |
|HR648x648  <br/> |A imagem tem 648 pixels de altura e 648 pixels de largura.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode estar vazio  <br/> ||
   

