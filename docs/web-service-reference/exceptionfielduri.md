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
description: O elemento ExceptionFieldURI identifica erros específicos em uma solicitação. Este elemento é usado apenas como parte de uma resposta de erro no nó MessageXml.
ms.openlocfilehash: a47d44098f85d8bacb1e7a2c48a33e478e56c7ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44454341"
---
# <a name="exceptionfielduri"></a>ExceptionFieldURI

O elemento **ExceptionFieldURI** identifica erros específicos em uma solicitação. Este elemento é usado apenas como parte de uma resposta de erro no nó [MessageXml](messagexml.md) . 
  
```xml
<ExceptionFieldURI FieldURI="" />
```

 **ExceptionPropertyURIType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**FieldURI** <br/> |Identifica uma propriedade de uma ocorrência de um item recorrente. Esse atributo é necessário.  <br/> |
   
#### <a name="fielduri-attribute"></a>Atributo FieldURI

|**Valor**|**Descrição**|
|:-----|:-----|
|Anexo: nome  <br/> |Identifica o nome do anexo como contendo um erro.  <br/> |
|Anexo: ContentType  <br/> |Identifica o tipo de conteúdo como contendo um erro.  <br/> |
|Anexo: conteúdo  <br/> |Identifica o conteúdo como contendo um erro.  <br/> |
|recorrência: mês  <br/> |Identifica o campo month como contendo um erro.  <br/> |
|recorrência: DayOfWeekIndex  <br/> |Identifica o índice de dia da semana como contendo um erro.  <br/> |
|recorrência: DaysOfWeek  <br/> |Identifica a Propriedade DaysOfWeek como contendo um erro.  <br/> |
|recorrência: DayOfMonth  <br/> |Identifica o DayOfMonth como contendo um erro.  <br/> |
|recorrência: intervalo  <br/> |Identifica o intervalo como contendo um erro.  <br/> |
|recorrência: NumberOfOccurrences  <br/> |Identifica o número de ocorrências como contendo um erro.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MessageXml](messagexml.md) <br/> |Fornece informações adicionais de resposta de erro.  <br/> |
   
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

