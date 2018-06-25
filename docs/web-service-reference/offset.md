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
description: O elemento de deslocamento descreve o deslocamento, desde o BaseOffset. Em conjunto com o elemento BaseOffset, o elemento de deslocamento identifica se o tempo é standard ou o horário de verão.
ms.openlocfilehash: d85fef0d67633733f6aa1943d70413ea70a528d6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824642"
---
# <a name="offset"></a>Deslocamento

O elemento de **deslocamento** descreve o deslocamento, desde o [BaseOffset](baseoffset.md). Em conjunto com o elemento **BaseOffset** , o elemento de **deslocamento** identifica se o tempo é standard ou o horário de verão. 
  
```xml
<Offset/>
```

 **duration**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Horário de verão](daylight.md) <br/> |Representa a data e hora de quando o tempo é alterado de horário de verão para a hora padrão.  <br/> |
|[Standard](standard.md) <br/> |Representa a data e hora de quando o tempo é alterado de horário de verão para a hora padrão.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto representa o deslocamento do tempo Universal Coordenado (UTC).
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

