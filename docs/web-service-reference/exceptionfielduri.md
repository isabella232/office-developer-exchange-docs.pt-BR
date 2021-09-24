---
title: ExceptionFieldURI
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ExceptionFieldURI
api_type:
- schema
ms.assetid: 7afda93a-0f8c-4c9e-8e09-f1b0bfc928bf
description: O elemento ExceptionFieldURI identifica erros específicos em uma solicitação. Esse elemento é usado apenas como parte de uma resposta de erro no nó MessageXml.
ms.openlocfilehash: 7368fd51e8eca2081b1fd50c86bce9ffa469c6b1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524326"
---
# <a name="exceptionfielduri"></a>ExceptionFieldURI

O **elemento ExceptionFieldURI** identifica erros específicos em uma solicitação. Esse elemento é usado apenas como parte de uma resposta de erro no [nó MessageXml.](messagexml.md) 
  
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
|attachment:Name  <br/> |Identifica o nome do anexo como contendo um erro.  <br/> |
|attachment:ContentType  <br/> |Identifica o tipo de conteúdo como contendo um erro.  <br/> |
|attachment:Content  <br/> |Identifica o conteúdo como contendo um erro.  <br/> |
|recorrência:Month  <br/> |Identifica o campo mês como contendo um erro.  <br/> |
|recurrence:DayOfWeekIndex  <br/> |Identifica o índice do dia da semana como contendo um erro.  <br/> |
|recurrence:DaysOfWeek  <br/> |Identifica a propriedade DaysOfWeek como contendo um erro.  <br/> |
|recurrence:DayOfMonth  <br/> |Identifica DayOfMonth como contendo um erro.  <br/> |
|recorrência:Interval  <br/> |Identifica o intervalo como contendo um erro.  <br/> |
|recorrência:NumberOfOccurrences  <br/> |Identifica o número de ocorrências como contendo um erro.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[MessageXml](messagexml.md) <br/> |Fornece informações adicionais de resposta a erros.  <br/> |
   
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

