---
title: ConvertHtmlCodePageToUTF8
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f02c8331-0a4e-4d01-adc2-2b93ed838a42
description: O elemento ConvertHtmlCodePageToUTF8 indica se o corpo HTML do item é convertido em UTF8.
ms.openlocfilehash: e43de22b6d8050c14eb18d0fdd5a72f463335189
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545570"
---
# <a name="converthtmlcodepagetoutf8"></a>ConvertHtmlCodePageToUTF8

O **elemento ConvertHtmlCodePageToUTF8** indica se o corpo HTML do item é convertido em UTF8. 
  
```XML
<ConvertHtmlCodePageToUTF8/>
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
|[ItemShape](itemshape.md) <br/> |Identifica um conjunto de propriedades a ser retornada em uma resposta.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto **true para** o **elemento ConvertHtmlCodePageToUTF8** indica que o corpo HTML é convertido em UTF8. Um valor de texto **false** indica que o corpo HTML não é convertido em UTF8. 
  
## <a name="remarks"></a>Comentários

O valor padrão de **true** será usado se **o elemento ConvertHtmlCodePageToUTF8** não for especificado em uma solicitação. 
  
O esquema que descreve esse elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services. Esse elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

