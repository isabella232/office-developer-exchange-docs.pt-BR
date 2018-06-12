---
title: ExtendedFieldURI
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExtendedFieldURI
api_type:
- schema
ms.assetid: b3c6ea3a-9ead-44b9-9d99-64ecf12bde23
description: O elemento ExtendedFieldURI identifica uma propriedade MAPI estendida.
ms.openlocfilehash: 8d946aec8ae2c5e6bb4ca3f1d8ee74250262d373
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752171"
---
# <a name="extendedfielduri"></a>ExtendedFieldURI

O elemento **ExtendedFieldURI** identifica uma propriedade MAPI estendida. 
  
```xml
<ExtendedFieldURI DistinguishedPropertySetId="" PropertySetId="" PropertyTag="" PropertyName="" PropertyId="" PropertyType="" />
```

 **PathToExtendedFieldType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

|**Attribute**|**Descrição**|
|:-----|:-----|
|**DistinguishedPropertySetId** <br/> |Define o conhecido propriedade definida IDs para propriedades estendidas de MAPI.  <br/> Se este atributo é usado, os atributos **PropertySetId** e **PropertyTag não** não podem ser usados. Este atributo deve ser usado com o **PropertyId** **PropertyName** atributo ou e o atributo **PropertyType** .  <br/> A tabela de atributo **DistinguishedPropertySetId** neste tópico lista os valores possíveis para este atributo.  <br/> Este atributo é opcional.  <br/> |
|**PropertySetId** <br/> |Identifica um MAPI estendido namespace ou conjunto de propriedades por sua identificação GUID.  <br/> Se este atributo é usado, o atributo **DistinguishedPropertySetId** e **PropertyTag não** não pode ser usado. Este atributo deve ser usado com o **PropertyId** **PropertyName** atributo ou e o atributo **PropertyType** .  <br/> Este atributo é opcional.  <br/> |
|**PropertyTag não** <br/> |Identifica a marca de propriedade sem a parte do tipo da marca. O **PropertyTag não** pode ser representado como um hexadecimal ou um inteiro curto.  <br/> O intervalo entre 0x8000 e 0xFFFE representa o intervalo personalizado das propriedades. Quando um banco de dados de caixa de correio encontra uma propriedade personalizada pela primeira vez, ele atribui essa propriedade personalizada uma marca de propriedade dentro do intervalo de propriedade personalizada de 0x8000-0xFFFE. Uma marca de propriedade personalizada determinado provavelmente serão diferentes entre bancos de dados. Portanto, uma solicitação de propriedade personalizada por marca de propriedade pode retornar propriedades diferentes em bancos de dados diferentes. O uso do atributo **PropertyTag não** é proibido para propriedades personalizadas. Em vez disso, use o atributo **PropertySetId** e o atributo **PropertyName** ou **PropertyId** .  <br/> > [!IMPORTANT]> Acessar qualquer propriedade personalizada entre 0x8000 e 0xFFFE usando-se o GUID + nome/ID.           Se o atributo **PropertyTag não** for usado, os atributos **DistinguishedPropertySetId**, **PropertySetId**, **PropertyName**e **PropertyId** não podem ser usados.  <br/> Este atributo é opcional.  <br/> > [!NOTE]> Você não pode usar um atributo de marca de propriedade para as propriedades dentro do intervalo personalizado 0x8000-0xFFFE. Você deve usar uma propriedade nomeada nesse caso.           |
|**PropertyName** <br/> |Identifica uma propriedade estendida por seu nome. Esta propriedade deve ser associada **DistinguishedPropertySetId** ou **PropertySetId**.  <br/> Se este atributo é usado, os atributos **PropertyId** e **PropertyTag não** não podem ser usados.  <br/> Este atributo é opcional.  <br/> |
|**PropertyId** <br/> |Identifica uma propriedade estendida por sua ID de expedição. A ID de expedição pode ser identificada nos formatos de decimais ou hexadecimais. Esta propriedade deve ser associada **DistinguishedPropertySetId** ou **PropertySetId**.  <br/> Se este atributo é usado, os atributos **PropertyName** e **PropertyTag não** não podem ser usados.  <br/> Este atributo é opcional.  <br/> |
|**PropertyType** <br/> |Representa o tipo de propriedade de uma marca de propriedade. Isso corresponde à palavra menos significativa em uma marca de propriedade.  <br/> A tabela de atributo PropertyType neste tópico contém os valores possíveis para este atributo.  <br/> Este atributo é necessário.  <br/> |
   
#### <a name="distinguishedpropertysetid-attribute"></a>Atributo DistinguishedPropertySetId

|**Valor**|**Descrição**|
|:-----|:-----|
|Reunião  <br/> |Identifica a reunião propriedade definida ID pelo nome.  <br/> |
|Compromisso  <br/> |Identifica a ID do conjunto de propriedade compromisso pelo nome.  <br/> |
|Comuns  <br/> |Identifica a ID do conjunto de propriedade comum pelo nome.  <br/> |
|PublicStrings  <br/> |Identifica a ID do conjunto de propriedade pública cadeias de caracteres pelo nome.  <br/> |
|Endereço  <br/> |Identifica a ID do conjunto de propriedade endereço pelo nome.  <br/> |
|InternetHeaders  <br/> |Identifica a identificação de conjunto de propriedade de cabeçalhos da Internet pelo nome.  <br/> |
|CalendarAssistant  <br/> |Identifica a identificação de conjunto de propriedade de Assistente de calendário pelo nome.  <br/> |
|UnifiedMessaging  <br/> |Identifica a ID do conjunto de propriedade mensagens unificadas pelo nome.  <br/> |
   
#### <a name="propertytype-attribute"></a>Atributo PropertyType

|**Valor**|**Descrição**|
|:-----|:-----|
|ApplicationTime  <br/> |Um valor double que será interpretado como uma data e hora. A parte inteira é a data e a parte de fração é a hora.  <br/> |
|ApplicationTimeArray  <br/> |Uma matriz de valores duplos que são interpretadas como uma data e hora.  <br/> |
|Binário  <br/> |Um valor binário codificado na Base64.  <br/> |
|BinaryArray  <br/> |Uma matriz de valores binários codificado na Base64.  <br/> |
|Booliano  <br/> |Um booleano **true** ou **false**.  <br/> |
|CLSID  <br/> |Uma cadeia de caracteres GUID.  <br/> |
|CLSIDArray  <br/> |Uma matriz de cadeias de caracteres GUID.  <br/> |
|Moeda  <br/> |Um inteiro de 64 bits que será interpretado como o número de centavos.  <br/> |
|CurrencyArray  <br/> |Uma matriz de números inteiros de 64 bits que são interpretadas como o número de centavos.  <br/> |
|Double  <br/> |Um valor de ponto flutuante de 64 bits.  <br/> |
|DoubleArray  <br/> |Uma matriz de valores de ponto flutuante de 64 bits.  <br/> |
|Erro  <br/> |Valor SCODE; inteiro não assinado de 32 bits.  <br/> Não é usado para restrições ou valores de obtenção/configuração. Isso existe apenas para relatório.  <br/> |
|Flutuante  <br/> |Um valor de ponto flutuante de 32 bits.  <br/> |
|FloatArray  <br/> |Uma matriz de valores de ponto flutuante de 32 bits.  <br/> |
|Inteiro  <br/> |Um inteiro assinado de (Int32) de 32 bits.  <br/> |
|IntegerArray  <br/> |Uma matriz de números inteiros (Int32) de 32 bits assinados.  <br/> |
|Long  <br/> |Um sinal ou 64 bits (Int64) inteiro.  <br/> |
|LongArray  <br/> |Uma matriz de sinal ou (Int64) de 64 bits inteiros.  <br/> |
|Null  <br/> |Não indica que nenhum valor de propriedade.  <br/> Não é usado para restrições ou valores de obtenção/configuração. Isso existe apenas para relatório.  <br/> |
|Objeto  <br/> |Um ponteiro para um objeto que implementa a interface IUnknown.  <br/> Não é usado para restrições ou valores de obtenção/configuração. Isso existe apenas para relatório.  <br/> |
|ObjectArray  <br/> |Uma matriz de ponteiros para objetos que implementem a interface IUnknown.  <br/> Não é usado para restrições ou valores de obtenção/configuração. Isso existe apenas para relatório.  <br/> |
|Curto  <br/> |Um inteiro assinado de 16 bits.  <br/> |
|ShortArray  <br/> |Uma matriz de números inteiros de 16 bits assinadas.  <br/> |
|SystemTime  <br/> |Um inteiro de 64 bits a data e hora valor na forma de uma estrutura FILETIME.  <br/> |
|SystemTimeArray  <br/> |Uma matriz de valores de data e hora de inteiro de 64 bits na forma de uma estrutura FILETIME.  <br/> |
|Cadeia de caracteres  <br/> |Uma cadeia de caracteres Unicode.  <br/> |
|StringArray  <br/> |Uma matriz de cadeias de caracteres Unicode.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ExtendedProperty](extendedproperty.md) <br/> |Identifica as propriedades estendidas em pastas e itens.  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> | Identifica as propriedades adicionais.  <br/>  A seguir estão as expressões XPath para esse elemento:  <br/>  `/FindFolder/FolderShape/AdditionalProperties` <br/>  `/GetFolder/FolderShape/AdditionalProperties` <br/>  `/SyncFolderHierarchy/FolderShape/AdditionalProperties` <br/>  `/GetItem/ItemShape/AdditionalProperties` <br/>  `/FindItem/ItemShape/AdditionalProperties` <br/>  `/SyncFolderItems/ItemShape/AdditionalProperties` <br/>  `/GetAttachment/AttachmentShape/AdditionalProperties` <br/> |
|[SetItemField](setitemfield.md) <br/> |Representa uma atualização para uma única propriedade de um item em uma [operação UpdateItem](updateitem-operation.md).  <br/> |
|[SetFolderField](setfolderfield.md) <br/> |Representa uma atualização para uma única propriedade em uma pasta em uma [operação UpdateFolder](updatefolder-operation.md).  <br/> |
|[DeleteItemField](deleteitemfield.md) <br/> |Representa uma operação de exclusão para excluir uma determinada propriedade de um item durante uma [operação UpdateItem](updateitem-operation.md).  <br/> |
|[DeleteFolderField](deletefolderfield.md) <br/> |Representa uma operação de exclusão para excluir uma determinada propriedade de uma pasta durante uma chamada de UpdateFolder.  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |Identifica os dados a serem acrescentados a uma única propriedade de um item durante uma [operação UpdateItem](updateitem-operation.md).  <br/> |
|[AppendToFolderField](appendtofolderfield.md) <br/> |Especifica os dados a serem acrescentados a uma propriedade de pasta durante uma [operação UpdateFolder](updatefolder-operation.md).  <br/> |
|[Existe](exists.md) <br/> |Representa uma expressão de pesquisa que retornará **true** se a propriedade fornecida existir em um item.  <br/> |
|[FieldURIOrConstant](fielduriorconstant.md) <br/> |Representa uma propriedade ou um valor de constante a ser usado ao comparar com outra propriedade.  <br/> |
|[IsEqualTo](isequalto.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com a um valor de constante ou outra propriedade e será avaliada como **true** , se eles forem iguais.  <br/> |
|[IsGreaterThan](isgreaterthan.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com um valor de constante ou outra propriedade e retorna **true** se a primeira propriedade for maior.  <br/> |
|[IsGreaterThanOrEqualTo](isgreaterthanorequalto.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com um valor de constante ou outra propriedade e retorna **true** se a propriedade primeira for maior que ou igual à segunda.  <br/> |
|[IsLessThan](islessthan.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com a um valor de constante ou outra propriedade e retorna **true** se a primeira propriedade for menor do que o segundo.  <br/> |
|[IsLessThanOrEqualTo](islessthanorequalto.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com a um valor de constante ou outra propriedade e retorna **true** se a primeira propriedade for menor do que o segundo.  <br/> |
|[IsNotEqualTo](isnotequalto.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com um valor de constante ou outra propriedade e retorna **true** se os valores não são iguais.  <br/> |
|[Exclui](excludes.md) <br/> |Executa uma máscara de bit a bit das propriedades.  <br/> |
|[Contém](contains.md) <br/> |Representa uma expressão de pesquisa que determina se uma determinada propriedade contém o valor de cadeia de caracteres constante fornecido.  <br/> |
|[FieldOrder](fieldorder.md) <br/> |Representa um único campo pelo qual fazer a classificação de resultados e indica a direção para a classificação.  <br/> |
   
## <a name="remarks"></a>Coment�rios

Alguns atributos não podem ser usados em combinação com outros atributos. Qualquer solicitação que vem com uma combinação de atributos de propriedade estendida inválida gerará uma mensagem de erro.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
> [!NOTE]
> No Microsoft .NET, um Long é um inteiro assinado de 64 bits, enquanto em MAPI e COM, um Long é um inteiro de 32 bits. A maioria dos desenvolvedores usará o Microsoft.NET Framework para desenvolver aplicativos de cliente de serviços Web do Exchange. Portanto, a nomenclatura do .NET é usada no lugar de MAPI nomenclatura. Por exemplo, a propriedade de MAPI PR_MESSAGE_FLAGS, 0x0E07, é um tipo PT_LONG. No .NET, isso é considerado um número inteiro. Uma propriedade estendida para PR_MESSAGE_FLAGS é definida como \<t:ExtendedFieldURI PropertyTag não = "0x0E07" PropertyType = "Inteiro" /\>. 
  
## <a name="example"></a>Example

O exemplo a seguir de uma solicitação cria um item que possui duas propriedades personalizadas. A primeira propriedade personalizada é nomeada **IsMyHouse** com um valor Boolean que defina como **true**. A segunda propriedade estendida personalizada é nomeada **HousePrices**. Ele contém uma matriz de valores de moeda. 
  
```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
    MessageDisposition="SaveOnly">
      <SavedItemFolderId>
        <t:DistinguishedFolderId Id="inbox"/>
      </SavedItemFolderId>
      <Items>
        <t:Item>
          <t:ItemClass>IPM.Note</t:ItemClass>
          <t:Subject>Create an extended property</t:Subject>
          <t:Body BodyType="Text">Added info to extended props</t:Body>
          <t:ExtendedProperty>
            <t:ExtendedFieldURI DistinguishedPropertySetId="PublicStrings" 
                                PropertyName="IsMyHouse" 
                                PropertyType="Boolean"/>
            <t:Value>true</t:Value>
          </t:ExtendedProperty>
          <t:ExtendedProperty>
            <t:ExtendedFieldURI DistinguishedPropertySetId="PublicStrings" 
                                PropertyName="HousePrices" 
                                PropertyType="CurrencyArray"/>
            <t:Values>
              <t:Value>30000000</t:Value>
              <t:Value>40000000</t:Value>
              <t:Value>50000000</t:Value>
            </t:Values>
          </t:ExtendedProperty>
        </t:Item>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[FieldURI](fielduri.md)
  
[IndexedFieldURI](indexedfielduri.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

