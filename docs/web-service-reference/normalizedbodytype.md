---
title: NormalizedBodyType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: c6973aee-ec7b-44c1-b328-f2204d9de5d1
description: O elemento NormalizedBodyType especifica se o corpo normalizado é retornado em formato HTML ou texto.
ms.openlocfilehash: 69ce440e30d921b052782af60057fff2d9e9d68f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59537563"
---
# <a name="normalizedbodytype"></a>NormalizedBodyType

O **elemento NormalizedBodyType** especifica se o corpo normalizado é retornado em formato HTML ou texto. 
  
```XML
<NormalizedBodyType> Best | HTML | Text </NormalizedBodyType>
```

 **BodyTypeResponseType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[ItemShape](itemshape.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do **elemento NormalizedBodyType** indica o formato em que o corpo normalizado é retornado. A tabela a seguir lista os valores possíveis para esse elemento. 
  
****

|**Valor**|**Descrição**|
|:-----|:-----|
|Melhor  <br/> |A resposta retornará o conteúdo disponível mais rico do corpo de texto. Isso é útil se não se sabe se o conteúdo é texto ou HTML.  <br/> O corpo retornado será texto se o corpo armazenado for texto sem texto. Caso contrário, a resposta retornará HTML se o corpo armazenado estiver no formato HTML ou RTF.  <br/> Esse é o valor padrão.  <br/> |
|HTML  <br/> |A resposta retornará um corpo normalizado como HTML.  <br/> |
|Texto  <br/> |A resposta retornará um corpo normalizado como texto sem texto.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Confira também



[ItemShape](itemshape.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

