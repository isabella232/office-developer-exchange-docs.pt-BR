---
title: ConvertHtmlCodePageToUTF8
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f02c8331-0a4e-4d01-adc2-2b93ed838a42
description: O elemento ConvertHtmlCodePageToUTF8 indica se o item do corpo em HTML é convertido em UTF8.
ms.openlocfilehash: aff6579835097a273101188c02a9919003b71b58
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751541"
---
# <a name="converthtmlcodepagetoutf8"></a>ConvertHtmlCodePageToUTF8

O elemento **ConvertHtmlCodePageToUTF8** indica se o item do corpo em HTML é convertido em UTF8. 
  
```XML
<ConvertHtmlCodePageToUTF8/>
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
|[ItemShape](itemshape.md) <br/> |Identifica um conjunto de propriedades para retornar em uma resposta.  <br/> |
   
## <a name="text-value"></a>Text value

Um valor de texto de **true** para o elemento **ConvertHtmlCodePageToUTF8** indica que o corpo HTML é convertido em UTF8. Um valor de texto de **false** indica que o corpo HTML não é convertido em UTF8. 
  
## <a name="remarks"></a>Comentários

O valor padrão **True** é usado se o elemento **ConvertHtmlCodePageToUTF8** não for especificado em uma solicitação. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

