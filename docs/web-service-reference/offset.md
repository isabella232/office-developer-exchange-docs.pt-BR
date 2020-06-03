---
title: Deslocamento
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Offset
api_type:
- schema
ms.assetid: dcbb9d85-d90c-4363-b4c9-d081ad03f407
description: O elemento offset descreve o deslocamento do BaseOffset. Junto com o elemento BaseOffset, o elemento offset identifica se o horário é padrão ou horário de verão.
ms.openlocfilehash: 74ad87026c2cb89f3b0c35218c91f81380029963
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459753"
---
# <a name="offset"></a>Deslocamento

O elemento **offset** descreve o deslocamento do [BaseOffset](baseoffset.md). Junto com o elemento **BaseOffset** , o elemento **offset** identifica se o horário é padrão ou horário de verão. 
  
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
|[Norte](daylight.md) <br/> |Representa a data e a hora em que o horário muda do horário de verão para o horário padrão.  <br/> |
|[Standard](standard.md) <br/> |Representa a data e a hora em que o horário muda do horário de verão para o horário padrão.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa o deslocamento do tempo universal coordenado (UTC).
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

