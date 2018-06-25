---
title: ErrorCode (int)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 65537d96-edf9-41ee-9ad5-91ffe37e2269
description: O elemento ErrorCode Especifica o código de erro de uma pesquisa com falha realizada em uma caixa de correio.
ms.openlocfilehash: ed8a7771376f921303ea093f4be727c4146faa76
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752087"
---
# <a name="errorcode-int"></a>ErrorCode (int)

O elemento **ErrorCode** Especifica o código de erro de uma pesquisa com falha realizada em uma caixa de correio. 
  
```XML
<ErrorCode></ErrorCode>
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
|[FailedMailbox](failedmailbox.md) <br/> |Especifica o status de retenção da caixa de correio.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto do elemento **ErrorCode** é o código de erro retornado para uma pesquisa com falha realizada em uma caixa de correio. 
  
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipo  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

