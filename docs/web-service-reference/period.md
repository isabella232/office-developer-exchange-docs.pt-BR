---
title: Period
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Period
api_type:
- schema
ms.assetid: 2f9cf6af-c531-4d7d-90c9-1a1db504d890
description: O elemento Period define o nome, o deslocamento de tempo e o identificador exclusivo para um estágio específico do fuso horário.
ms.openlocfilehash: 7fa5bca6547f4e3120c60c2e2b69139f7bb12e93
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59534732"
---
# <a name="period"></a>Period

O **elemento Period** define o nome, o deslocamento de tempo e o identificador exclusivo para um estágio específico do fuso horário. 
  
```xml
<Period Bias="" Name="" Id=""/>
```

 **PeriodType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|Bias  <br/> |Um valor xs:duration que representa o deslocamento de tempo de UTC (Tempo Universal Coordenado) para o período.  <br/> |
|Nome  <br/> |Um valor de cadeia de caracteres que representa o nome descritivo do período.  <br/> |
|Id  <br/> |Um valor de cadeia de caracteres que representa o identificador do período.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Periods](periods.md) <br/> |Representa uma matriz de períodos que definem o deslocamento de tempo em diferentes estágios do fuso horário.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

