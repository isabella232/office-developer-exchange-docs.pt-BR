---
title: Extended (PathToExtendedFieldType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fa620b48-2ce3-437d-b51e-541247eea1d9
description: O elemento Estendiproperty especifica uma propriedade estendida para o repositório unificado de contatos.
ms.openlocfilehash: f6c283d5cce3bc927662ad0d9c796c0589e7054c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460138"
---
# <a name="extendedproperty-pathtoextendedfieldtype"></a>Extended (PathToExtendedFieldType)

O elemento **estendiproperty** especifica uma propriedade estendida para o repositório unificado de contatos. 
  
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
|DistinguishedPropertySetId  <br/> |Indica o identificador do conjunto de propriedades diferenciado. Esse atributo é opcional.  <br/> |
|PropertySetId  <br/> |Indica o identificador do conjunto de propriedades GUID. Esse atributo é opcional.  <br/> |
|PropertyTag  <br/> | Representa a marca de propriedade menos a parte tipo.<br/><br/>Há duas opções para representação:  <br/><br/>-Hexadecimal: 0x3fa4  <br/>-Decimal: 0-65535<br/><br/>  Esse atributo é opcional.  <br/> |
|PropertyName  <br/> |Cadeia de caracteres que indica o nome da propriedade. Esse atributo é opcional.  <br/> |
|PropertyId  <br/> |Número inteiro que indica o identificador de propriedade. Esse atributo é opcional.  <br/> |
|Recordtypepropriedade  <br/> |Indica o tipo de propriedade. Esse atributo é necessário.  <br/> |
|FieldURI  <br/> |Indica o URI (Uniform Resource Identifier) do campo. Esse atributo é necessário. Para obter os valores possíveis, consulte o elemento [FieldURI](fielduri.md) .  <br/> |
   
#### <a name="distinguishedpropertysetid"></a>DistinguishedPropertySetId

|**Valor**|**Descrição**|
|:-----|:-----|
|Atenda  <br/> |Indica uma reunião.  <br/> |
|Compromisso  <br/> |Indica um compromisso.  <br/> |
|Comum  <br/> |Indica o conjunto de propriedades comuns.  <br/> |
|PublicStrings  <br/> |Indica cadeias de caracteres públicas.  <br/> |
|Endereço  <br/> |Indica um endereço.  <br/> |
|InternetHeaders  <br/> |Indica cabeçalhos de Internet.  <br/> |
|CalendarAssistant  <br/> |Indica o assistente de calendário.  <br/> |
|UnifiedMessaging  <br/> |Indica a Unificação de mensagens.  <br/> |
|Tarefa  <br/> |Indica uma tarefa.  <br/> |
   
#### <a name="propertytype"></a>Recordtypepropriedade

|**Valor**|**Descrição**|
|:-----|:-----|
|Applicationtime  <br/> |Indica o tempo do aplicativo.  <br/> |
|ApplicationTimeArray  <br/> |Indica uma matriz de horários de aplicativo.  <br/> |
|Binária  <br/> |Indica um valor binário.  <br/> |
|BinaryArray  <br/> |Indica uma matriz de valores binários.  <br/> |
|Booliano  <br/> |Indica um valor booliano.  <br/> |
|CLSID  <br/> |Indica um CLSID.  <br/> |
|CLSIDArray  <br/> |Indica uma matriz de CLSIDs.  <br/> |
|Moeda  <br/> |Indica um valor de moeda.  <br/> |
|CurrencyArray  <br/> |Indica uma matriz de valores de moeda.  <br/> |
|Duplo  <br/> |Indica um **duplo**.  <br/> |
|DoubleArray  <br/> |Indica uma matriz de valores **Double** .  <br/> |
|Erro  <br/> |Indica um erro. Isso é para fins de relatório de erros. Ele não pode ser usado em restrições ou para obter ou definir valores.  <br/> |
|Flutuação  <br/> |Indica um **float**.  <br/> |
|FloatArray  <br/> |Indica uma matriz de valores **float** .  <br/> |
|Número inteiro  <br/> |Indica um inteiro.  <br/> |
|IntegerArray  <br/> |Indica uma matriz de inteiros.  <br/> |
|Longo  <br/> |Indica um **Long**.  <br/> |
|LongArray  <br/> |Indica uma matriz de valores **Long** .  <br/> |
|Nulo  <br/> |Indica um valor nulo. Isso é para fins de relatório de erros. Ele não pode ser usado em restrições ou para obter ou definir valores.  <br/> |
|Objeto  <br/> |Indica um objeto. Isso é para fins de relatório de erros. Ele não pode ser usado em restrições ou para obter ou definir valores.  <br/> |
|Objectarray  <br/> |Indica uma matriz de objetos. Isso é para fins de relatório de erros. Ele não pode ser usado em restrições ou para obter ou definir valores.  <br/> |
|Curto  <br/> |Indica um **curto**.  <br/> |
|ShortArray  <br/> |Indica uma matriz de valores **curtos** .  <br/> |
|SystemTime  <br/> |Indica um valor de tempo do sistema.  <br/> |
|SystemTimeArray  <br/> |Indica uma matriz de valores de tempo do sistema.  <br/> |
|String  <br/> |Indica uma cadeia de caracteres.  <br/> |
|StringArray  <br/> |Indica uma matriz de cadeia de caracteres.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifica uma propriedade MAPI Estendida.  <br/> |
   
## <a name="remarks"></a>Comentários

Este elemento foi introduzido no Exchange Server 2013.
  
O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipo  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

