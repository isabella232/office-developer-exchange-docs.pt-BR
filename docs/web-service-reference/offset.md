---
title: Offset
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Offset
api_type:
- schema
ms.assetid: dcbb9d85-d90c-4363-b4c9-d081ad03f407
description: O elemento Offset descreve o deslocamento do BaseOffset. Juntamente com o elemento BaseOffset, o elemento Offset identifica se a hora é padrão ou horário de verão.
ms.openlocfilehash: af9a2f7a94ae0cd736a4fe6f11b8a5a77673bbe3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515387"
---
# <a name="offset"></a>Offset

O **elemento Offset** descreve o deslocamento do [BaseOffset](baseoffset.md). Juntamente com o **elemento BaseOffset,** o elemento **Offset** identifica se a hora é padrão ou horário de verão. 
  
```xml
<Offset/>
```

 **duration**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Daylight](daylight.md) <br/> |Representa a data e a hora em que a hora muda do horário de verão para a hora padrão.  <br/> |
|[Standard](standard.md) <br/> |Representa a data e a hora em que a hora muda do horário de verão para a hora padrão.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa o deslocamento de Tempo Universal Coordenado (UTC).
  
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do EWS do computador que está executando Microsoft Exchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

