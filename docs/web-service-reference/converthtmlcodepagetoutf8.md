---
title: ConvertHtmlCodePageToUTF8
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f02c8331-0a4e-4d01-adc2-2b93ed838a42
description: O elemento ConvertHtmlCodePageToUTF8 indica se o corpo de HTML do item é convertido em UTF8.
ms.openlocfilehash: a714eacd8cc105146a1471f062ec35dc16730d61
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457589"
---
# <a name="converthtmlcodepagetoutf8"></a>ConvertHtmlCodePageToUTF8

O elemento **ConvertHtmlCodePageToUTF8** indica se o corpo de HTML do item é convertido em UTF8. 
  
```XML
<ConvertHtmlCodePageToUTF8/>
```

 **xs: Boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Shape](itemshape.md) <br/> |Identifica um conjunto de propriedades a serem retornadas em uma resposta.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto **true** para o elemento **ConvertHtmlCodePageToUTF8** indica que o corpo de HTML é convertido em UTF8. Um valor **false** indica que o corpo HTML não é convertido em UTF8. 
  
## <a name="remarks"></a>Comentários

O valor padrão **true** é usado se o elemento **ConvertHtmlCodePageToUTF8** não for especificado em uma solicitação. 
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

