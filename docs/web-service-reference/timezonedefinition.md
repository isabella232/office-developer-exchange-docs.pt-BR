---
title: TimeZoneDefinition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- TimeZoneDefinition
api_type:
- schema
ms.assetid: b005a80c-addb-4409-beff-e5162076752c
description: O elemento TimeZoneDefinition especifica os períodos e transições que definem um fuso horário.
ms.openlocfilehash: 6f2b580d2c3e31826ca74034cfda938cff71ee53
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538811"
---
# <a name="timezonedefinition"></a>TimeZoneDefinition

O **elemento TimeZoneDefinition** especifica os períodos e transições que definem um fuso horário. 
  
```XML
<TimeZoneDefinition Id="" Name="">
   <Periods/>
   <TransitionsGroups/>
   <Transitions/>
</TimeZoneDefinition>

```

 **TimeZoneDefinitionType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|Id  <br/> |Representa o identificador exclusivo do fuso horário.  <br/> |
|Name  <br/> |Representa o nome descritivo do fuso horário.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Periods](periods.md) <br/> |Representa uma matriz de [elementos Period](period.md) que definem o deslocamento de tempo em diferentes estágios do fuso horário.  <br/> |
|[TransitionsGroups](transitionsgroups.md) <br/> |Representa uma matriz de elementos [TransitionsGroup](transitionsgroup.md) que especificam transições de fuso horário.  <br/> |
|[Transitions](transitions.md) <br/> |Representa uma matriz de transições de fuso horário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[TimeZoneDefinitions](timezonedefinitions.md) <br/> |Representa uma matriz de definições de fuso horário.  <br/> |
|[TimeZoneContext](timezonecontext.md) <br/> |Representa a definição de fuso horário padrão que deve ser usada para o scoping das propriedades DateTime de objetos criados, atualizados e recuperados usando o Exchange Web Services (EWS).  <br/> |
   
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

