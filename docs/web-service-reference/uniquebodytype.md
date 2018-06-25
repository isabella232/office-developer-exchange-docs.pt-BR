---
title: UniqueBodyType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8f7276aa-e354-40e4-b9cb-950fad46ac93
description: O elemento UniqueBodyType Especifica se o corpo exclusivo é retornado no formato HTML ou texto.
ms.openlocfilehash: c6eb4ec4e39a0c5355775a635db4c63efc666820
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837844"
---
# <a name="uniquebodytype"></a>UniqueBodyType

O elemento **UniqueBodyType** Especifica se o corpo exclusivo é retornado no formato HTML ou texto. 
  
```XML
<UniqueBodyType> Best | HTML | Text </UniqueBodyType>
```

 **BodyTypeResponseType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[ItemShape](itemshape.md)
  
## <a name="text-value"></a>Text value

O valor de texto do elemento **UniqueBodyType** indica o formato do corpo exclusivo é retornado em tempo. A tabela a seguir lista os valores possíveis para esse elemento. 
  
****

|**Valor**|**Descrição**|
|:-----|:-----|
|Melhor  <br/> |A resposta retornará o conteúdo disponível mais sofisticado de corpo de texto. Isso é útil se for desconhecido se o conteúdo é o texto ou HTML.  <br/> O corpo retornado será o texto se o corpo armazenado for texto sem formatação. Caso contrário, a resposta retornará HTML, se o corpo armazenado está no formato HTML ou RTF.  <br/> Este é o valor padrão.  <br/> |
|HTML  <br/> |A resposta retornará um único corpo como HTML.  <br/> |
|Texto  <br/> |A resposta retornará um único corpo como texto sem formatação.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Ver também



[ItemShape](itemshape.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

