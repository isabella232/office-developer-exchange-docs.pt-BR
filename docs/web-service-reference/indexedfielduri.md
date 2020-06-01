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
ms.openlocfilehash: f794d9970590417d916925f7258b28d4f0920d0e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467015"
---
# <a name="indexedfielduri"></a>IndexedFieldURI

O elemento **IndexedFieldURI** identifica membros individuais de um dicionário. 
  
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
|item: InternetMessageHeader  <br/> |Representa o cabeçalho da mensagem de um item.  <br/> |
|contatos: imendereço  <br/> |Representa o endereço de mensagens instantâneas de um contato.  <br/> |
|contatos: PhysicalAddress: rua  <br/> |Representa o endereço de um contato.  <br/> |
|contatos: PhysicalAddress: cidade  <br/> |Representa a cidade de um contato.  <br/> |
|contatos: PhysicalAddress: State  <br/> |Representa o estado de um contato.  <br/> |
|contatos: PhysicalAddress: país  <br/> |Representa o país/região de um contato.  <br/> |
|contatos: PhysicalAddress: CEP  <br/> |Representa o código postal de um contato.  <br/> |
|contatos: PhoneNumber  <br/> |Representa o número de telefone de um contato.  <br/> |
|contatos: EmailAddress  <br/> |Representa o endereço de email de um contato.  <br/> |
|DistributionList: members: member  <br/> |Representa um membro de uma lista de distribuição.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[AdditionalProperties](additionalproperties.md) <br/> |Identifica propriedades adicionais a serem obtidas, definidas ou criadas.  <br/> |
|[Agregar](aggregateon.md) <br/> |Representa a propriedade que é usada para determinar a ordem dos itens agrupados para um conjunto de resultados de FindItem agrupado.  <br/> |
|[GroupBy](groupby.md) <br/> |Especifica um agrupamento arbitrário para consultas do FindItem.  <br/> |
   
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

