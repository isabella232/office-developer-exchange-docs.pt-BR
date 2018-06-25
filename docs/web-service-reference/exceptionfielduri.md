---
title: ExceptionFieldURI
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExceptionFieldURI
api_type:
- schema
ms.assetid: 7afda93a-0f8c-4c9e-8e09-f1b0bfc928bf
description: O elemento ExceptionFieldURI identifica erros específicos em uma solicitação. Esse elemento é usado apenas como parte de uma resposta de erro no nó MessageXml.
ms.openlocfilehash: 79909405179cec0d0b86ad12bf52031e1daeb790
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752118"
---
# <a name="exceptionfielduri"></a>ExceptionFieldURI

O elemento **ExceptionFieldURI** identifica erros específicos em uma solicitação. Esse elemento é usado apenas como parte de uma resposta de erro no nó [MessageXml](messagexml.md) . 
  
```xml
<ExceptionFieldURI FieldURI="" />
```

 **ExceptionPropertyURIType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**FieldURI** <br/> |Identifica uma propriedade de uma ocorrência de um item recorrente. Este atributo é necessário.  <br/> |
   
#### <a name="fielduri-attribute"></a>Atributo FieldURI

|**Valor**|**Descrição**|
|:-----|:-----|
|Nome do anexo:  <br/> |Identifica o nome do anexo como contendo um erro.  <br/> |
|anexo: ContentType  <br/> |Identifica o tipo de conteúdo como contendo um erro.  <br/> |
|Conteúdo de anexo:  <br/> |Identifica o conteúdo como contendo um erro.  <br/> |
|Recorrência: mês  <br/> |Identifica o campo de mês como contendo um erro.  <br/> |
|Recorrência: DayOfWeekIndex  <br/> |Identifica o dia do índice de semana como contendo um erro.  <br/> |
|Recorrência: DaysOfWeek  <br/> |Identifica a propriedade DaysOfWeek como contendo um erro.  <br/> |
|Recorrência: DayOfMonth  <br/> |Identifica o DayOfMonth como contendo um erro.  <br/> |
|Intervalo de recorrência:  <br/> |Identifica o intervalo como contendo um erro.  <br/> |
|Recorrência: NumberOfOccurrences  <br/> |Identifica o número de ocorrências como contendo um erro.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MessageXml](messagexml.md) <br/> |Fornece informações de resposta de erro adicionais.  <br/> |
   
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

