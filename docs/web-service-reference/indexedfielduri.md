---
title: IndexedFieldURI
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IndexedFieldURI
api_type:
- schema
ms.assetid: 5c9cd0b5-7eca-480a-8730-fe98b1779afa
description: O elemento IndexedFieldURI identifica membros individuais de um dicionário.
ms.openlocfilehash: 851d0d4296e926ab21e5bd1b842d5a215c27308a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539623"
---
# <a name="indexedfielduri"></a>IndexedFieldURI

O **elemento IndexedFieldURI** identifica membros individuais de um dicionário. 
  
```xml
<IndexedFieldURI FieldURI="" FieldIndex="" />
```

 **PathToIndexedFieldType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**FieldURI** <br/> |Identifica o dicionário que contém o membro a ser retornado. Esse atributo é necessário.  <br/> |
|**FieldIndex** <br/> |Identifica o membro do dicionário a ser retornado. Esse atributo é necessário.  <br/> |
   
#### <a name="fielduri-attribute"></a>Atributo FieldURI

|**Valor**|**Descrição**|
|:-----|:-----|
|item:InternetMessageHeader  <br/> |Representa o header de mensagem de um item.  <br/> |
|contacts:ImAddress  <br/> |Representa o endereço de mensagens instantâneas de um contato.  <br/> |
|contacts:PhysicalAddress:Street  <br/> |Representa o endereço de rua de um contato.  <br/> |
|contacts:PhysicalAddress:City  <br/> |Representa a cidade de um contato.  <br/> |
|contacts:PhysicalAddress:State  <br/> |Representa o estado de um contato.  <br/> |
|contacts:PhysicalAddress:Country  <br/> |Representa o país/região de um contato.  <br/> |
|contacts:PhysicalAddress:PostalCode  <br/> |Representa o código postal de um contato.  <br/> |
|contacts:PhoneNumber  <br/> |Representa o número de telefone de um contato.  <br/> |
|contacts:EmailAddress  <br/> |Representa o endereço de email de um contato.  <br/> |
|distributionlist:Members:Member  <br/> |Representa um membro de uma lista de distribuição.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AdditionalProperties](additionalproperties.md) <br/> |Identifica propriedades adicionais para obter, definir ou criar.  <br/> |
|[AggregateOn](aggregateon.md) <br/> |Representa a propriedade usada para determinar a ordem de itens agrupados para um conjunto de resultados FindItem agrupado.  <br/> |
|[GroupBy](groupby.md) <br/> |Especifica um grupo arbitrário para consultas FindItem.  <br/> |
   
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

