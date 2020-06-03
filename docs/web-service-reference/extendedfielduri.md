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
description: O elemento ExtendedFieldURI identifica uma propriedade MAPI Estendida.
ms.openlocfilehash: fd365010016c68236107991717ed538c97dc0d50
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526029"
---
# <a name="extendedfielduri"></a>ExtendedFieldURI

O elemento **ExtendedFieldURI** identifica uma propriedade MAPI Estendida. 
  
```xml
<ExtendedFieldURI DistinguishedPropertySetId="" PropertySetId="" PropertyTag="" PropertyName="" PropertyId="" PropertyType="" />
```

**PathToExtendedFieldType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**DistinguishedPropertySetId** <br/> |Define as IDs de conjunto de propriedades conhecidas para propriedades MAPI estendidas.<br/><br/>Se esse atributo for usado, os atributos **PropertySetId** e **PropertyTag** não poderão ser usados. Esse atributo deve ser usado com o atributo **PropertyId** ou **PropertyName** e o atributo **recordtypepropriedade** .<br/><br/>A tabela de atributos **DistinguishedPropertySetId** posteriormente neste tópico lista os valores possíveis para este atributo.<br/><br/>Esse atributo é opcional.  <br/> |
|**PropertySetId** <br/> |Identifica um conjunto de propriedades estendidas de MAPI ou namespace por seu GUID de identificação.<br/><br/>Se esse atributo for usado, o atributo **DistinguishedPropertySetId** e **PropertyTag** não poderá ser usado. Esse atributo deve ser usado com o atributo **PropertyId** ou **PropertyName** e o atributo **recordtypepropriedade** .<br/><br/>Esse atributo é opcional.  <br/> |
|**PropertyTag** <br/> |Identifica a marca de propriedade sem o tipo parte da marca. O **PropertyTag** pode ser representado como um inteiro hexadecimal ou curto.<br/><br/>O intervalo entre 0x8000 e 0xFFFE representa o intervalo de propriedades personalizado. Quando um banco de dados de caixa de correio encontra uma propriedade personalizada pela primeira vez, ele atribui a propriedade personalizada uma marca de propriedade dentro do intervalo de propriedades personalizadas de 0x8000-0xFFFE. Uma determinada marca de propriedade personalizada provavelmente será diferente em bancos de dados. Por esse motivo, uma marca de propriedade personalizada de solicitação de propriedade pode retornar propriedades diferentes em bancos de dados diferentes. O uso do atributo **PropertyTag** é proibido para propriedades personalizadas. Em vez disso, use o atributo **PropertySetId** e o atributo **PropertyName** ou **PropertyId** .<br/><br/>**Importante**: acessar qualquer propriedade personalizada entre o 0x8000 e o 0xFFFE usando o GUID + nome/ID. Se o atributo **PropertyTag** for usado, os **atributos DistinguishedPropertySetId**, **PropertySetId**, **PropertyName**e **PropertyId** não poderão ser usados.<br/><br/>Esse atributo é opcional.<br/><br/>**Observação**: não é possível usar um atributo de marca de propriedade para as propriedades dentro do intervalo personalizado 0X8000-0xFFFE. Você deve usar uma propriedade nomeada nesse caso.           |
|**PropertyName** <br/> |Identifica uma propriedade estendida pelo nome. Essa propriedade deve ser associada a **DistinguishedPropertySetId** ou **PropertySetId**.<br/><br/>Se esse atributo for usado, os atributos **PropertyId** e **PropertyTag** não poderão ser usados.<br/><br/>Esse atributo é opcional.  <br/> |
|**PropertyId** <br/> |Identifica uma propriedade estendida por sua ID de expedição. A ID de expedição pode ser identificada em formatos decimais ou hexadecimais. Essa propriedade deve ser associada a **DistinguishedPropertySetId** ou **PropertySetId**.<br/><br/>Se esse atributo for usado, os atributos **PropertyName** e **PropertyTag** não poderão ser usados.<br/><br/>Esse atributo é opcional.  <br/> |
|**Recordtypepropriedade** <br/> |Representa o tipo de propriedade de uma marca de propriedade. Isso corresponde à palavra menos significativa em uma marca de propriedade.<br/><br/>A tabela de atributos Recordtypepropriedade posteriormente neste tópico contém os valores possíveis para este atributo.<br/><br/>Esse atributo é necessário.  <br/> |
   
#### <a name="distinguishedpropertysetid-attribute"></a>Atributo DistinguishedPropertySetId

|**Valor**|**Descrição**|
|:-----|:-----|
|Endereço  <br/> |Identifica o ID do conjunto de propriedades de endereço por nome.  <br/> |
|Compromisso  <br/> |Identifica o ID do conjunto de propriedades de compromisso por nome.  <br/> |
|CalendarAssistant  <br/> |Identifica a propriedade do assistente de calendário ID definida por nome.  <br/> |
|Comum  <br/> |Identifica a ID do conjunto de propriedades comuns por nome.  <br/> |
|InternetHeaders  <br/> |Identifica a ID do conjunto de propriedades de cabeçalhos da Internet por nome.  <br/> |
|Atenda  <br/> |Identifica a ID do conjunto de propriedades da reunião por nome.  <br/> |
|Compartilhamento  <br/> | <br/> |
|PublicStrings  <br/> |Identifica a ID do conjunto de propriedades de cadeia de caracteres pública por nome.  <br/> |
|Tarefa  <br/> |Identifica o ID do conjunto de propriedades da tarefa por nome.  <br/> |
|UnifiedMessaging  <br/> |Identifica o ID do conjunto de propriedades da Unificação de mensagens por nome.  <br/> |
   
#### <a name="propertytype-attribute"></a>Atributo Recordtypepropriedade

|**Valor**|**Descrição**|
|:-----|:-----|
|Applicationtime  <br/> |Um valor Double que é interpretado como data e hora. A parte inteira é a data e a parte fracionária é a hora.  <br/> |
|ApplicationTimeArray  <br/> |Uma matriz de valores double interpretados como data e hora.  <br/> |
|Binária  <br/> |Um valor binário codificado em base64.  <br/> |
|BinaryArray  <br/> |Uma matriz de valores binários codificados em base64.  <br/> |
|Booliano  <br/> |Um booliano **true** ou **false**.  <br/> |
|CLSID  <br/> |Uma cadeia de caracteres GUID.  <br/> |
|CLSIDArray  <br/> |Uma matriz de cadeias de caracteres GUID.  <br/> |
|Moeda  <br/> |Um inteiro de 64 bits interpretado como o número de centavos.  <br/> |
|CurrencyArray  <br/> |Uma matriz de inteiros de 64 bits interpretados como o número de centavos.  <br/> |
|Duplo  <br/> |Um valor de ponto flutuante de 64 bits.  <br/> |
|DoubleArray  <br/> |Uma matriz de valores de ponto flutuante de 64 bits.  <br/> |
|Erro  <br/> |Valor SCODE; número inteiro não assinado de 32 bits.  <br/> Não é usado para restrições ou para obter/definir valores. Isso existe somente para relatórios.  <br/> |
|Flutuação  <br/> |Um valor de ponto flutuante de 32 bits.  <br/> |
|FloatArray  <br/> |Uma matriz de valores de ponto flutuante de 32 bits.  <br/> |
|Número inteiro  <br/> |Um inteiro de 32 bits assinado (Int32).  <br/> |
|IntegerArray  <br/> |Uma matriz de inteiros assinados de 32 bits (Int32).  <br/> |
|Longo  <br/> |Um inteiro de 64 bits assinado ou não assinado (Int64).  <br/> |
|LongArray  <br/> |Uma matriz de inteiros assinados ou não assinados de 64 bits (Int64).  <br/> |
|Nulo  <br/> |Indica nenhum valor de propriedade.  <br/> Não é usado para restrições ou para obter/definir valores. Isso existe somente para relatórios.  <br/> |
|Objeto  <br/> |Um ponteiro para um objeto que implementa a interface IUnknown.  <br/> Não é usado para restrições ou para obter/definir valores. Isso existe somente para relatórios.  <br/> |
|Objectarray  <br/> |Uma matriz de ponteiros para objetos que implementam a interface IUnknown.  <br/> Não é usado para restrições ou para obter/definir valores. Isso existe somente para relatórios.  <br/> |
|Curto  <br/> |Um inteiro de 16 bits assinado.  <br/> |
|ShortArray  <br/> |Uma matriz de inteiros de 16 bits assinados.  <br/> |
|SystemTime  <br/> |Um valor de data e hora inteiro de 64 bits na forma de uma estrutura FILETIME.  <br/> |
|SystemTimeArray  <br/> |Uma matriz de dados inteiros de 64 bits e valores de tempo na forma de uma estrutura FILETIME.  <br/> |
|String  <br/> |Uma cadeia de caracteres Unicode.  <br/> |
|StringArray  <br/> |Uma matriz de cadeias de caracteres Unicode.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ExtendedProperty](extendedproperty.md) <br/> |Identifica as propriedades estendidas em pastas e itens.  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> | Identifica propriedades adicionais.<br/><br/>A seguir estão as expressões XPath para este elemento:<br/><br/>`/FindFolder/FolderShape/AdditionalProperties` <br/>  `/GetFolder/FolderShape/AdditionalProperties` <br/>  `/SyncFolderHierarchy/FolderShape/AdditionalProperties` <br/>  `/GetItem/ItemShape/AdditionalProperties` <br/>  `/FindItem/ItemShape/AdditionalProperties` <br/>  `/SyncFolderItems/ItemShape/AdditionalProperties` <br/>  `/GetAttachment/AttachmentShape/AdditionalProperties` <br/> |
|[Setitemfield](setitemfield.md) <br/> |Representa uma atualização de uma única propriedade de um item em uma [operação UpdateItem](updateitem-operation.md).  <br/> |
|[Setfolderfield](setfolderfield.md) <br/> |Representa uma atualização de uma única propriedade em uma pasta em uma [operação UpdateFolder](updatefolder-operation.md).  <br/> |
|[DeleteItemField](deleteitemfield.md) <br/> |Representa uma operação de exclusão para excluir uma determinada propriedade de um item durante uma [operação UpdateItem](updateitem-operation.md).  <br/> |
|[DeleteFolderField](deletefolderfield.md) <br/> |Representa uma operação de exclusão para excluir uma determinada propriedade de uma pasta durante uma chamada UpdateFolder.  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |Identifica os dados a serem acrescentados a uma única propriedade de um item durante uma [operação UpdateItem](updateitem-operation.md).  <br/> |
|[AppendToFolderField](appendtofolderfield.md) <br/> |Especifica os dados a serem acrescentados a uma propriedade de pasta durante uma [operação UpdateFolder](updatefolder-operation.md).  <br/> |
|[Existe](exists.md) <br/> |Representa uma expressão de pesquisa que retorna **true** se a propriedade fornecida existir em um item.  <br/> |
|[FieldURIOrConstant](fielduriorconstant.md) <br/> |Representa uma propriedade ou um valor de constante a ser usado ao comparar com outra propriedade.  <br/> |
|[IsEqualTo](isequalto.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com um valor constante ou outra propriedade e é avaliada como **true** se elas forem iguais.  <br/> |
|[IsGreaterThan](isgreaterthan.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com um valor constante ou outra propriedade e retorna **true** se a primeira propriedade é maior.  <br/> |
|[IsGreaterThanOrEqualTo](isgreaterthanorequalto.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com um valor constante ou outra propriedade e retorna **true** se a primeira propriedade for maior ou igual à segunda.  <br/> |
|[IsLessThan](islessthan.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com um valor constante ou outra propriedade e retorna **true** se a primeira propriedade for menor do que o segundo.  <br/> |
|[IsLessThanOrEqualTo](islessthanorequalto.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com um valor constante ou outra propriedade e retorna **true** se a primeira propriedade for menor do que o segundo.  <br/> |
|[IsNotEqualTo](isnotequalto.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com um valor constante ou outra propriedade e retorna **true** se os valores não forem iguais.  <br/> |
|[Exclui](excludes.md) <br/> |Executa uma máscara de bits bit das propriedades.  <br/> |
|[Contém](contains.md) <br/> |Representa uma expressão de pesquisa que determina se uma determinada propriedade contém o valor de cadeia de caracteres constante fornecido.  <br/> |
|[FieldOrder](fieldorder.md) <br/> |Representa um único campo pelo qual classificar os resultados e indica a direção da classificação.  <br/> |
   
## <a name="remarks"></a>Comentários

Alguns atributos não podem ser usados em combinação com outros atributos. Qualquer solicitação que vier com uma combinação inválida de atributos de propriedade estendida irá gerar uma mensagem de erro.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
> [!NOTE]
> No Microsoft .NET, um Long é um inteiro assinado de 64 bits, enquanto em MAPI e COM, um Long é um inteiro de bit 32. A maioria dos desenvolvedores usará a estrutura do Microsoft.NET para desenvolver aplicativos clientes de serviços Web do Exchange. Portanto, o nome do .NET é usado em vez do nome do MAPI.
> 
> Por exemplo, a propriedade PR_MESSAGE_FLAGS MAPI, 0x0E07, é um \_ tipo pt Long. No .NET, isso é considerado um inteiro. Uma propriedade estendida para PR_MESSAGE_FLAGS é definida como `<t:ExtendedFieldURI PropertyTag="0x0E07" PropertyType="Integer"/>` . 
  
## <a name="example"></a>Exemplo

O exemplo a seguir de uma solicitação cria um item que tem duas propriedades personalizadas. A primeira propriedade personalizada é denominada **IsMyHouse** com um valor booliano definido como **true**. A segunda propriedade estendida personalizada é denominada **HousePrices**. Ele contém uma matriz de valores de moeda. 
  
```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
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

## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [FieldURI](fielduri.md)
- [IndexedFieldURI](indexedfielduri.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

