---
title: Timezonedefinition pela última vez
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeZoneDefinition
api_type:
- schema
ms.assetid: b005a80c-addb-4409-beff-e5162076752c
description: O elemento timezonedefinition pela última vez Especifica os períodos e transições que definem um fuso horário.
ms.openlocfilehash: ffd5ed0c862af794e4aff2387f508849b1d5fd5d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837760"
---
# <a name="timezonedefinition"></a>Timezonedefinition pela última vez

O elemento **timezonedefinition pela última vez** Especifica os períodos e transições que definem um fuso horário. 
  
```XML
<TimeZoneDefinition Id="" Name="">
   <Periods/>
   <TransitionsGroups/>
   <Transitions/>
</TimeZoneDefinition>

```

 **TimeZoneDefinitionType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|Id  <br/> |Representa o identificador exclusivo do fuso horário.  <br/> |
|Nome  <br/> |Representa o nome descritivo do fuso horário.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Períodos](periods.md) <br/> |Representa uma matriz de elementos do [período](period.md) que definem o deslocamento de tempo em fases diferentes do fuso horário.  <br/> |
|[TransitionsGroups](transitionsgroups.md) <br/> |Representa uma matriz de elementos de [TransitionsGroup](transitionsgroup.md) que especificam as transições do fuso horário.  <br/> |
|[Transições](transitions.md) <br/> |Representa uma matriz de transições de fuso horário.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[TimeZoneDefinitions](timezonedefinitions.md) <br/> |Representa uma matriz de definições de fuso horário.  <br/> |
|[TimeZoneContext](timezonecontext.md) <br/> |Representa a definição de fuso horário padrão que será usado para as propriedades de data/hora dos objetos que são criados, atualizados e recuperadas usando serviços Web do Exchange (EWS) de escopo.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

