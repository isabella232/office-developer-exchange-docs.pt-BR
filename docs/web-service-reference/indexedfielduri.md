---
title: IndexedFieldURI
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IndexedFieldURI
api_type:
- schema
ms.assetid: 5c9cd0b5-7eca-480a-8730-fe98b1779afa
description: O elemento IndexedFieldURI identifica membros individuais de um dicionário.
ms.openlocfilehash: 6a75e8855ecabf15ca31bb1e05d569c258a43b0b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823909"
---
# <a name="indexedfielduri"></a>IndexedFieldURI

O elemento **IndexedFieldURI** identifica membros individuais de um dicionário. 
  
```xml
<IndexedFieldURI FieldURI="" FieldIndex="" />
```

 **PathToIndexedFieldType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**FieldURI** <br/> |Identifica o dicionário que contém o membro para retornar. Este atributo é necessário.  <br/> |
|**FieldIndex** <br/> |Identifica o membro do dicionário para retornar. Este atributo é necessário.  <br/> |
   
#### <a name="fielduri-attribute"></a>Atributo FieldURI

|**Valor**|**Descrição**|
|:-----|:-----|
|item: InternetMessageHeader  <br/> |Representa o cabeçalho da mensagem de um item.  <br/> |
|Contatos: ImAddress  <br/> |Representa o endereço de um contato de mensagens instantâneas.  <br/> |
|Contatos: PhysicalAddress:Street  <br/> |Representa o endereço de um contato.  <br/> |
|Contatos: PhysicalAddress:City  <br/> |Representa a cidade de um contato.  <br/> |
|Contatos: PhysicalAddress:State  <br/> |Representa o estado de um contato.  <br/> |
|Contatos: PhysicalAddress:Country  <br/> |Representa o país/região de um contato.  <br/> |
|Contatos: PhysicalAddress:PostalCode  <br/> |Representa o código postal de um contato.  <br/> |
|Contatos: PhoneNumber  <br/> |Representa o número de telefone de um contato.  <br/> |
|Contatos: EmailAddress  <br/> |Representa o endereço de email de um contato.  <br/> |
|DistributionList:Members:Member  <br/> |Representa um membro de uma lista de distribuição.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AdditionalProperties](additionalproperties.md) <br/> |Identifica as propriedades adicionais para obter, definir ou criar.  <br/> |
|[AggregateOn](aggregateon.md) <br/> |Representa a propriedade que é usada para determinar a ordem dos itens agrupados para um conjunto de resultados FindItem agrupada.  <br/> |
|[GroupBy](groupby.md) <br/> |Especifica um agrupamento arbitrário para consultas FindItem.  <br/> |
   
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

