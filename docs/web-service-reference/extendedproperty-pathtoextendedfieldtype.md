---
title: ExtendedProperty (PathToExtendedFieldType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: fa620b48-2ce3-437d-b51e-541247eea1d9
description: O elemento ExtendedProperty especifica uma propriedade estendida para o Unified Contact Store.
ms.openlocfilehash: 5cb320e15d3a01c542907048357d1ef0cc78f96a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530756"
---
# <a name="extendedproperty-pathtoextendedfieldtype"></a>ExtendedProperty (PathToExtendedFieldType)

O **elemento ExtendedProperty** especifica uma propriedade estendida para o Unified Contact Store. 
  
```xml
<ExtendedProperty DistinguishedPropertySetId="" PropertySetId="" PropertyTag="" PropertyName="" PropertyId="" PropertyType="" FieldURI="">
</ExtendedProperty>
```

**PathToExtendedFieldType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|DistinguishedPropertySetId  <br/> |Indica o identificador de conjunto de propriedades diferenciado. Esse atributo é opcional.  <br/> |
|PropertySetId  <br/> |Indica o identificador de conjunto de propriedades GUID. Esse atributo é opcional.  <br/> |
|PropertyTag  <br/> | Representa a marca de propriedade menos a parte de tipo.<br/><br/>Há duas opções para representação:  <br/><br/>- Hexadecimal: 0x3fa4  <br/>- Decimal: 0-65535<br/><br/>  Esse atributo é opcional.  <br/> |
|PropertyName  <br/> |Cadeia de caracteres que indica o nome da propriedade. Esse atributo é opcional.  <br/> |
|PropertyId  <br/> |Integer que indica o identificador de propriedade. Esse atributo é opcional.  <br/> |
|PropertyType  <br/> |Indica o tipo de propriedade. Esse atributo é necessário.  <br/> |
|FieldURI  <br/> |Indica o campo Uniform Resource Identifier (URI). Esse atributo é necessário. Para valores possíveis, consulte o [elemento FieldURI.](fielduri.md)  <br/> |
   
#### <a name="distinguishedpropertysetid"></a>DistinguishedPropertySetId

|**Valor**|**Descrição**|
|:-----|:-----|
|Reunião  <br/> |Indica uma reunião.  <br/> |
|Compromisso  <br/> |Indica um compromisso.  <br/> |
|Comum  <br/> |Indica o conjunto de propriedades comuns.  <br/> |
|PublicStrings  <br/> |Indica cadeias de caracteres públicas.  <br/> |
|Endereço  <br/> |Indica um endereço.  <br/> |
|InternetHeaders  <br/> |Indica os headers da Internet.  <br/> |
|CalendarAssistant  <br/> |Indica o Assistente de Calendário.  <br/> |
|UnifiedMessaging  <br/> |Indica Unificação de Mensagens.  <br/> |
|Tarefa  <br/> |Indica uma tarefa.  <br/> |
   
#### <a name="propertytype"></a>PropertyType

|**Valor**|**Descrição**|
|:-----|:-----|
|ApplicationTime  <br/> |Indica a hora do aplicativo.  <br/> |
|ApplicationTimeArray  <br/> |Indica uma matriz de tempos de aplicativo.  <br/> |
|Binário  <br/> |Indica um valor binário.  <br/> |
|BinaryArray  <br/> |Indica uma matriz de valores binários.  <br/> |
|Booliano  <br/> |Indica um valor Boolean.  <br/> |
|CLSID  <br/> |Indica um CLSID.  <br/> |
|CLSIDArray  <br/> |Indica uma matriz de CLSIDs.  <br/> |
|Moeda  <br/> |Indica um valor de moeda.  <br/> |
|CurrencyArray  <br/> |Indica uma matriz de valores de moeda.  <br/> |
|Duplo  <br/> |Indica **um** duplo .  <br/> |
|DoubleArray  <br/> |Indica uma matriz de **valores duplos.**  <br/> |
|Erro  <br/> |Indica um erro. Isso é para fins de relatório de erros. Ele não pode ser usado em restrições ou para obter ou definir valores.  <br/> |
|Flutuação  <br/> |Indica um **float**.  <br/> |
|FloatArray  <br/> |Indica uma matriz de valores **flutuantes.**  <br/> |
|Número inteiro  <br/> |Indica um inteiro.  <br/> |
|IntegerArray  <br/> |Indica uma matriz de inteiros.  <br/> |
|Longo  <br/> |Indica um **longo**.  <br/> |
|LongArray  <br/> |Indica uma matriz de **valores longos.**  <br/> |
|Nulo  <br/> |Indica um valor nulo. Isso é para fins de relatório de erros. Ele não pode ser usado em restrições ou para obter ou definir valores.  <br/> |
|Objeto  <br/> |Indica um objeto. Isso é para fins de relatório de erros. Ele não pode ser usado em restrições ou para obter ou definir valores.  <br/> |
|ObjectArray  <br/> |Indica uma matriz de objetos. Isso é para fins de relatório de erros. Ele não pode ser usado em restrições ou para obter ou definir valores.  <br/> |
|Curto  <br/> |Indica um **curto**.  <br/> |
|ShortArray  <br/> |Indica uma matriz de **valores curtos.**  <br/> |
|SystemTime  <br/> |Indica um valor de tempo do sistema.  <br/> |
|SystemTimeArray  <br/> |Indica uma matriz de valores de tempo do sistema.  <br/> |
|Cadeia de caracteres  <br/> |Indica uma cadeia de caracteres.  <br/> |
|StringArray  <br/> |Indica uma matriz de cadeias de caracteres.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifica uma propriedade MAPI estendida.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Tipo de esquema  <br/> |
|Arquivo de validação  <br/> |types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

