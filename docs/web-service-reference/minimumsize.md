---
title: MinimumSize
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 841d229c-140c-48bd-b3a7-21478fcea2fb
description: O elemento MinimumSize representa o tamanho mínimo que uma mensagem deve ser em ordem para a condição ou uma exceção a ser aplicado.
ms.openlocfilehash: 4f80bac3b9226019ec3d726cd2d6430e02cac423
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824480"
---
# <a name="minimumsize"></a>MinimumSize

O elemento **MinimumSize** representa o tamanho mínimo que uma mensagem deve ser em ordem para a condição ou uma exceção a ser aplicado. 
  
```XML
<MinimumSize/>
```

 **int**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[WithinSizeRange](withinsizerange.md) <br/> |Especifica os tamanhos mínimos e máximo que as mensagens recebidas devem estar na ordem para a condição ou uma exceção a ser aplicado.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto é um inteiro que identifica o tamanho mínimo da mensagem em bytes.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Ver também



[MaximumSize](maximumsize.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

