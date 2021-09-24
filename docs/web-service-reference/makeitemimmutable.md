---
title: MakeItemImmutable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: de1d2a60-aeeb-4625-8b11-23c42e1e7bae
description: O elemento MakeItemImmutable especifica um valor Boolean que indica se um item deve ser feito somente leitura.
ms.openlocfilehash: 0e1d28f19492bb6dc013957aa5957b59e791b24b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524823"
---
# <a name="makeitemimmutable"></a>MakeItemImmutable

O **elemento MakeItemImmutable** especifica um valor Boolean que indica se um item deve ser feito somente leitura. 
  
```XML
<MakeItemImmutable>true | false</MakeItemImmutable>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[UpdateItemInRecoverableItems](updateiteminrecoverableitems.md)
  
## <a name="text-value"></a>Valor de texto

Um valor de texto **true** para o **elemento MakeItemImmutable** indica que o item deve ser feito somente leitura. Um valor **false** indica que o item permite acesso de leitura e gravação. 
  
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
   

