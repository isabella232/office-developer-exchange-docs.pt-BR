---
title: ExtendedFieldURI
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ExtendedFieldURI
api_type:
- schema
ms.assetid: b3c6ea3a-9ead-44b9-9d99-64ecf12bde23
description: O elemento ExtendedFieldURI identifica uma propriedade MAPI estendida.
ms.openlocfilehash: 0cf3926c900e1b1f35018c6706cfe99ebefbe76f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542313"
---
# <a name="extendedfielduri"></a>ExtendedFieldURI

O **elemento ExtendedFieldURI** identifica uma propriedade MAPI estendida. 
  
```xml
<ExtendedFieldURI DistinguishedPropertySetId="" PropertySetId="" PropertyTag="" PropertyName="" PropertyId="" PropertyType="" />
```

**PathToExtendedFieldType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

|**Atributo**|**Descrição**|
|:-----|:-----|
|**DistinguishedPropertySetId** <br/> |Define as IDs de conjunto de propriedades conhecidas para propriedades MAPI estendidas.<br/><br/>Se esse atributo for usado, os **atributos PropertySetId** e **PropertyTag** não poderão ser usados. Esse atributo deve ser usado com o **atributo PropertyId** ou **PropertyName** e **o atributo PropertyType.**<br/><br/>A **tabela Atributo DistinguishedPropertySetId** mais adiante neste tópico lista os valores possíveis para esse atributo.<br/><br/>Esse atributo é opcional.  <br/> |
|**PropertySetId** <br/> |Identifica um conjunto de propriedades estendidas MAPI ou namespace por seu GUID de identificação.<br/><br/>Se esse atributo for usado, o **atributo DistinguishedPropertySetId** e **PropertyTag** não poderá ser usado. Esse atributo deve ser usado com o **atributo PropertyId** ou **PropertyName** e **o atributo PropertyType.**<br/><br/>Esse atributo é opcional.  <br/> |
|**PropertyTag** <br/> |Identifica a marca de propriedade sem a parte do tipo da marca. A **PropertyTag** pode ser representada como um hexadecimal ou um inteiro curto.<br/><br/>O intervalo entre 0x8000 e 0xFFFE representa o intervalo personalizado de propriedades. Quando um banco de dados de caixa de correio encontra uma propriedade personalizada pela primeira vez, ele atribui a essa propriedade personalizada uma marca de propriedade dentro do intervalo de propriedades personalizadas de 0x8000-0xFFFE. Uma determinada marca de propriedade personalizada provavelmente será diferente entre bancos de dados. Portanto, uma solicitação de propriedade personalizada por marca de propriedade pode retornar propriedades diferentes em bancos de dados diferentes. O uso do atributo **PropertyTag** é proibido para propriedades personalizadas. Em vez disso, use **o atributo PropertySetId** e **o atributo PropertyName** ou **PropertyId.**<br/><br/>**IMPORTANTE**: acesse qualquer propriedade personalizada entre 0x8000 e 0xFFFE usando o GUID + nome/ID. Se o **atributo PropertyTag** for usado, os atributos **DistinguishedPropertySetId,** **PropertySetId,** **PropertyName** e **PropertyId** não poderão ser usados.<br/><br/>Esse atributo é opcional.<br/><br/>**OBSERVAÇÃO**: Não é possível usar um atributo de marca de propriedade para propriedades dentro do intervalo personalizado 0x8000-0xFFFE. Você deve usar uma propriedade nomeada nesse caso.           |
|**PropertyName** <br/> |Identifica uma propriedade estendida pelo nome. Essa propriedade deve ser juntada a **DistinguishedPropertySetId** ou **PropertySetId**.<br/><br/>Se esse atributo for usado, os **atributos PropertyId** e **PropertyTag** não poderão ser usados.<br/><br/>Esse atributo é opcional.  <br/> |
|**PropertyId** <br/> |Identifica uma propriedade estendida por sua ID de expedição. A ID de expedição pode ser identificada em formatos decimais ou hexadecimais. Essa propriedade deve ser juntada a **DistinguishedPropertySetId** ou **PropertySetId**.<br/><br/>Se esse atributo for usado, os atributos **PropertyName** e **PropertyTag** não poderão ser usados.<br/><br/>Esse atributo é opcional.  <br/> |
|**PropertyType** <br/> |Representa o tipo de propriedade de uma marca de propriedade. Isso corresponde à palavra menos significativa em uma marca de propriedade.<br/><br/>A tabela Atributo PropertyType posteriormente neste tópico contém os valores possíveis para esse atributo.<br/><br/>Esse atributo é necessário.  <br/> |
   
#### <a name="distinguishedpropertysetid-attribute"></a>Atributo DistinguishedPropertySetId

|**Valor**|**Descrição**|
|:-----|:-----|
|Endereço  <br/> |Identifica a ID do conjunto de endereços pelo nome.  <br/> |
|Compromisso  <br/> |Identifica a ID do conjunto de propriedades de compromisso pelo nome.  <br/> |
|CalendarAssistant  <br/> |Identifica a ID do conjunto de propriedades do assistente de calendário pelo nome.  <br/> |
|Comum  <br/> |Identifica a ID de conjunto de propriedades comuns pelo nome.  <br/> |
|InternetHeaders  <br/> |Identifica a ID do conjunto de propriedades de headers da Internet pelo nome.  <br/> |
|Reunião  <br/> |Identifica a ID do conjunto de propriedades de reunião pelo nome.  <br/> |
|Compartilhamento  <br/> | <br/> |
|PublicStrings  <br/> |Identifica a ID do conjunto de cadeias de caracteres públicas pelo nome.  <br/> |
|Tarefa  <br/> |Identifica a ID do conjunto de propriedades de tarefas pelo nome.  <br/> |
|UnifiedMessaging  <br/> |Identifica a ID do conjunto de propriedades de unificação de mensagens pelo nome.  <br/> |
   
#### <a name="propertytype-attribute"></a>Atributo PropertyType

|**Valor**|**Descrição**|
|:-----|:-----|
|ApplicationTime  <br/> |Um valor duplo que é interpretado como uma data e hora. A parte inteiro é a data e a parte fracionada é a hora.  <br/> |
|ApplicationTimeArray  <br/> |Uma matriz de valores duplos que são interpretados como data e hora.  <br/> |
|Binário  <br/> |Um valor binário codificado em Base64.  <br/> |
|BinaryArray  <br/> |Uma matriz de valores binários codificados por Base64.  <br/> |
|Boolean  <br/> |Um **booleano verdadeiro** ou **falso.**  <br/> |
|CLSID  <br/> |Uma cadeia de caracteres GUID.  <br/> |
|CLSIDArray  <br/> |Uma matriz de cadeias de caracteres GUID.  <br/> |
|Moeda  <br/> |Um inteiro de 64 bits que é interpretado como o número de cêntimos.  <br/> |
|CurrencyArray  <br/> |Uma matriz de inteiros de 64 bits que são interpretados como o número de centavos.  <br/> |
|Duplo  <br/> |Um valor de ponto flutuante de 64 bits.  <br/> |
|DoubleArray  <br/> |Uma matriz de valores de ponto flutuante de 64 bits.  <br/> |
|Erro  <br/> |Valor SCODE; Inteiro não assinado de 32 bits.  <br/> Não usado para restrições ou para obter/definir valores. Isso existe apenas para relatórios.  <br/> |
|Flutuação  <br/> |Um valor de ponto flutuante de 32 bits.  <br/> |
|FloatArray  <br/> |Uma matriz de valores de ponto flutuante de 32 bits.  <br/> |
|Número inteiro  <br/> |Um inteiro assinado de 32 bits (Int32).  <br/> |
|IntegerArray  <br/> |Uma matriz de inteiros assinados de 32 bits (Int32).  <br/> |
|Longo  <br/> |Um inteiro de 64 bits assinado ou não assinado (Int64).  <br/> |
|LongArray  <br/> |Uma matriz de inteiros de 64 bits assinados ou não assinados (Int64).  <br/> |
|Nulo  <br/> |Indica nenhum valor de propriedade.  <br/> Não usado para restrições ou para obter/definir valores. Isso existe apenas para relatórios.  <br/> |
|Objeto  <br/> |Um ponteiro para um objeto que implementa a interface IUnknown.  <br/> Não usado para restrições ou para obter/definir valores. Isso existe apenas para relatórios.  <br/> |
|ObjectArray  <br/> |Uma matriz de ponteiros para objetos que implementam a interface IUnknown.  <br/> Não usado para restrições ou para obter/definir valores. Isso existe apenas para relatórios.  <br/> |
|Curto  <br/> |Um inteiro de 16 bits assinado.  <br/> |
|ShortArray  <br/> |Uma matriz de inteiros de 16 bits assinados.  <br/> |
|SystemTime  <br/> |Um valor de tempo e dados inteiros de 64 bits na forma de uma estrutura FILETIME.  <br/> |
|SystemTimeArray  <br/> |Uma matriz de dados inteiros de 64 bits e valores de tempo na forma de uma estrutura FILETIME.  <br/> |
|Cadeia de caracteres  <br/> |Uma cadeia de caracteres Unicode.  <br/> |
|StringArray  <br/> |Uma matriz de cadeias de caracteres Unicode.  <br/> |
   
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[ExtendedProperty](extendedproperty.md) <br/> |Identifica propriedades estendidas em pastas e itens.  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> | Identifica propriedades adicionais.<br/><br/>Veja a seguir as expressões XPath para este elemento:<br/><br/>`/FindFolder/FolderShape/AdditionalProperties` <br/>  `/GetFolder/FolderShape/AdditionalProperties` <br/>  `/SyncFolderHierarchy/FolderShape/AdditionalProperties` <br/>  `/GetItem/ItemShape/AdditionalProperties` <br/>  `/FindItem/ItemShape/AdditionalProperties` <br/>  `/SyncFolderItems/ItemShape/AdditionalProperties` <br/>  `/GetAttachment/AttachmentShape/AdditionalProperties` <br/> |
|[SetItemField](setitemfield.md) <br/> |Representa uma atualização para uma única propriedade de um item em uma [operação UpdateItem](updateitem-operation.md).  <br/> |
|[SetFolderField](setfolderfield.md) <br/> |Representa uma atualização para uma única propriedade em uma pasta em uma [operação UpdateFolder](updatefolder-operation.md).  <br/> |
|[DeleteItemField](deleteitemfield.md) <br/> |Representa uma operação de exclusão para excluir uma determinada propriedade de um item durante uma [operação UpdateItem](updateitem-operation.md).  <br/> |
|[DeleteFolderField](deletefolderfield.md) <br/> |Representa uma operação de exclusão para excluir uma determinada propriedade de uma pasta durante uma chamada UpdateFolder.  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |Identifica dados a ser anexados a uma única propriedade de um item durante uma [operação UpdateItem.](updateitem-operation.md)  <br/> |
|[AppendToFolderField](appendtofolderfield.md) <br/> |Especifica dados a ser anexados a uma propriedade de pasta durante uma [operação UpdateFolder.](updatefolder-operation.md)  <br/> |
|[Existe](exists.md) <br/> |Representa uma expressão de pesquisa que retorna **true** se a propriedade fornecida existir em um item.  <br/> |
|[FieldURIOrConstant](fielduriorconstant.md) <br/> |Representa uma propriedade ou um valor constante a ser usado ao comparar com outra propriedade.  <br/> |
|[IsEqualTo](isequalto.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com um valor constante ou outra propriedade e é avaliada como **true** se for igual.  <br/> |
|[IsGreaterThan](isgreaterthan.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com um valor constante ou outra propriedade e retorna **true** se a primeira propriedade for maior.  <br/> |
|[IsGreaterThanOrEqualTo](isgreaterthanorequalto.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com um valor constante ou outra propriedade e retorna **true** se a primeira propriedade for maior ou igual à segunda.  <br/> |
|[IsLessThan](islessthan.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com um valor constante ou outra propriedade e retorna **true** se a primeira propriedade for menor que a segunda.  <br/> |
|[IsLessThanOrEqualTo](islessthanorequalto.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com um valor constante ou outra propriedade e retorna **true** se a primeira propriedade for menor que a segunda.  <br/> |
|[IsNotEqualTo](isnotequalto.md) <br/> |Representa uma expressão de pesquisa que compara uma propriedade com um valor constante ou outra propriedade e retorna **true** se os valores não são os mesmos.  <br/> |
|[Exclui](excludes.md) <br/> |Executa uma máscara de bit das propriedades.  <br/> |
|[Contém](contains.md) <br/> |Representa uma expressão de pesquisa que determina se uma determinada propriedade contém o valor da cadeia de caracteres constante fornecida.  <br/> |
|[FieldOrder](fieldorder.md) <br/> |Representa um único campo pelo qual classificar resultados e indica a direção da classificação.  <br/> |
   
## <a name="remarks"></a>Comentários

Alguns atributos não podem ser usados em combinação com outros atributos. Qualquer solicitação que venha com uma combinação inválida de atributos de propriedade estendida gerará uma mensagem de erro.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
> [!NOTE]
> No Microsoft .NET, um Long é um inteiro assinado de 64 bits, enquanto em MAPI e COM, um Long é um inteiro de 32 bits. A maioria dos desenvolvedores usará o Microsoft.NET Framework para desenvolver Exchange aplicativos cliente de Serviços Web. Portanto, o nome .NET é usado em vez do nome MAPI.
> 
> Por exemplo, a PR_MESSAGE_FLAGS MAPI, 0x0E07, é um tipo PT \_ LONG. No .NET, isso é considerado um inteiro. Uma propriedade estendida para PR_MESSAGE_FLAGS é definida como `<t:ExtendedFieldURI PropertyTag="0x0E07" PropertyType="Integer"/>` . 
  
## <a name="example"></a>Exemplo

O exemplo a seguir de uma solicitação cria um item que tem duas propriedades personalizadas. A primeira propriedade personalizada é chamada **IsMyHouse** com um valor Boolean definido como **true**. A segunda propriedade estendida personalizada é chamada **HousePrices**. Ele contém uma matriz de Conversor de Moedas valores. 
  
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
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [FieldURI](fielduri.md)
- [IndexedFieldURI](indexedfielduri.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

