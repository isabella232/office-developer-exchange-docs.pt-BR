---
title: UniqueBodyType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8f7276aa-e354-40e4-b9cb-950fad46ac93
description: O elemento UniqueBodyType especifica se o corpo exclusivo é retornado no formato de texto ou HTML.
ms.openlocfilehash: 7e6c4631ef589555ce4d5da747c200ffe956f3a1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459437"
---
# <a name="uniquebodytype"></a>UniqueBodyType

O elemento **UniqueBodyType** especifica se o corpo exclusivo é retornado no formato de texto ou HTML. 
  
```XML
<UniqueBodyType> Best | HTML | Text </UniqueBodyType>
```

 **BodyTypeResponseType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

[Shape](itemshape.md)
  
## <a name="text-value"></a>Valor de texto

O valor de texto do elemento **UniqueBodyType** indica o formato em que o corpo exclusivo é retornado. A tabela a seguir lista os valores possíveis para este elemento. 
  
****

|**Valor**|**Descrição**|
|:-----|:-----|
|Melhor  <br/> |A resposta retornará o conteúdo mais avançado disponível do corpo de texto. Isso é útil se for desconhecido se o conteúdo for texto ou HTML.  <br/> O corpo retornado será texto se o corpo armazenado for texto sem formatação. Caso contrário, a resposta retornará HTML se o corpo armazenado estiver em formato HTML ou RTF.  <br/> Esse é o valor padrão.  <br/> |
|HTML  <br/> |A resposta retornará um corpo exclusivo como HTML.  <br/> |
|Texto  <br/> |A resposta retornará um corpo exclusivo como texto sem formatação.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013 Service Pack 1 (SP1).
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |Verdadeiro  <br/> |
   
## <a name="see-also"></a>Também consulte



[Shape](itemshape.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

