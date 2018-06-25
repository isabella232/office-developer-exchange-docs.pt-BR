---
title: ExtendedProperty (PathToExtendedFieldType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fa620b48-2ce3-437d-b51e-541247eea1d9
description: O elemento ExtendedProperty Especifica uma propriedade estendida para o repositório unificado de contatos.
ms.openlocfilehash: 7541fa6330ee96f7791febfabc672dbcf0e95b54
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752187"
---
# <a name="extendedproperty-pathtoextendedfieldtype"></a>ExtendedProperty (PathToExtendedFieldType)

O elemento **ExtendedProperty** Especifica uma propriedade estendida para o repositório unificado de contatos. 
  
```xml
<ExtendedProperty DistinguishedPropertySetId="" PropertySetId="" PropertyTag="" PropertyName="" PropertyId="" PropertyType="" FieldURI="">
</ExtendedProperty>
```

**PathToExtendedFieldType**

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|DistinguishedPropertySetId  <br/> |Indica o identificador de conjunto distinto de propriedade. Este atributo é opcional.  <br/> |
|PropertySetId  <br/> |Indica o identificador de conjunto de propriedade GUID. Este atributo é opcional.  <br/> |
|PropertyTag não  <br/> | Representa a marca de propriedade a menos que a parte do tipo.<br/><br/>Há duas opções para representação:  <br/><br/>-Hexadecimal: 0x3fa4  <br/>-Decimal: 0-65535<br/><br/>  Este atributo é opcional.  <br/> |
|PropertyName  <br/> |Cadeia de caracteres que indica o nome da propriedade. Este atributo é opcional.  <br/> |
|PropertyId  <br/> |Número inteiro que indica o identificador de propriedade. Este atributo é opcional.  <br/> |
|PropertyType  <br/> |Indica o tipo de propriedade. Este atributo é necessário.  <br/> |
|FieldURI  <br/> |Indica o identificador de recurso uniforme (URI) do campo. Este atributo é necessário. Para valores possíveis, consulte o elemento [FieldURI](fielduri.md) .  <br/> |
   
#### <a name="distinguishedpropertysetid"></a>DistinguishedPropertySetId

|**Valor**|**Descrição**|
|:-----|:-----|
|Reunião  <br/> |Indica uma reunião.  <br/> |
|Compromisso  <br/> |Indica um compromisso.  <br/> |
|Comuns  <br/> |Indica o conjunto de propriedades comuns.  <br/> |
|PublicStrings  <br/> |Indica as cadeias de caracteres públicas.  <br/> |
|Endereço  <br/> |Indica um endereço.  <br/> |
|InternetHeaders  <br/> |Indica os cabeçalhos da Internet.  <br/> |
|CalendarAssistant  <br/> |Indica o Assistente de calendário.  <br/> |
|UnifiedMessaging  <br/> |Indica a Unificação de mensagens.  <br/> |
|Tarefa  <br/> |Indica uma tarefa.  <br/> |
   
#### <a name="propertytype"></a>PropertyType

|**Valor**|**Descrição**|
|:-----|:-----|
|ApplicationTime  <br/> |Indica a hora de aplicativo.  <br/> |
|ApplicationTimeArray  <br/> |Indica uma matriz de tempos de aplicativos.  <br/> |
|Binário  <br/> |Indica um valor binário.  <br/> |
|BinaryArray  <br/> |Indica uma matriz de valores binários.  <br/> |
|Booliano  <br/> |Indica um valor booleano.  <br/> |
|CLSID  <br/> |Indica um CLSID.  <br/> |
|CLSIDArray  <br/> |Indica uma matriz de CLSIDs.  <br/> |
|Moeda  <br/> |Indica um valor de moeda.  <br/> |
|CurrencyArray  <br/> |Indica uma matriz de valores de moeda.  <br/> |
|Double  <br/> |Indica **duplo**.  <br/> |
|DoubleArray  <br/> |Indica uma matriz de valores **duplos** .  <br/> |
|Erro  <br/> |Indica um erro. Isso é para fins de relatório de erros. Ele não pode ser usado em restrições ou para obter ou definir valores.  <br/> |
|Flutuante  <br/> |Indica um **float**.  <br/> |
|FloatArray  <br/> |Indica uma matriz de valores **float** .  <br/> |
|Inteiro  <br/> |Indica um inteiro.  <br/> |
|IntegerArray  <br/> |Indica uma matriz de números inteiros.  <br/> |
|Long  <br/> |Indica um **longo**.  <br/> |
|LongArray  <br/> |Indica uma matriz de valores **longos** .  <br/> |
|Null  <br/> |Indica um valor nulo. Isso é para fins de relatório de erros. Ele não pode ser usado em restrições ou para obter ou definir valores.  <br/> |
|Objeto  <br/> |Indica um objeto. Isso é para fins de relatório de erros. Ele não pode ser usado em restrições ou para obter ou definir valores.  <br/> |
|ObjectArray  <br/> |Indica uma matriz de objetos. Isso é para fins de relatório de erros. Ele não pode ser usado em restrições ou para obter ou definir valores.  <br/> |
|Curto  <br/> |Indica um **curto**.  <br/> |
|ShortArray  <br/> |Indica uma matriz de valores **curta** .  <br/> |
|SystemTime  <br/> |Indica um valor de tempo do sistema.  <br/> |
|SystemTimeArray  <br/> |Indica uma matriz de valores de tempo do sistema.  <br/> |
|String  <br/> |Indica uma cadeia de caracteres.  <br/> |
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
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipo  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> ||
   
## <a name="see-also"></a>Confira também

- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

