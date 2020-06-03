---
title: Usar filtros de pesquisa com o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 20fc6d2d-41c2-4490-98b8-c52513977fef
description: Descubra como usar filtros de pesquisa com a API gerenciada do EWS ou o EWS no Exchange.
localization_priority: Priority
ms.openlocfilehash: 04a74ec92d4bced8abd58d164a1c186d6405e679
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455832"
---
# <a name="use-search-filters-with-ews-in-exchange"></a>Usar filtros de pesquisa com o EWS no Exchange

Descubra como usar filtros de pesquisa com a API gerenciada do EWS ou o EWS no Exchange.
  
Os filtros de pesquisa são a principal ferramenta para expressar os critérios de pesquisa na API gerenciada do EWS ou no aplicativo EWS. Recomendamos que você use os filtros de pesquisa, em oposição às [cadeias de caracteres de consulta](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md), para fazer o seguinte:
  
- Pesquisar em uma propriedade específica ou em um conjunto de propriedades.  
- Pesquisa usando vários critérios de pesquisa.
    
Os filtros de pesquisa são sua única opção se você estiver fazendo um dos seguintes:
  
- Pesquisando Propriedades personalizadas.  
- Executar pesquisas de cadeia de caracteres que diferencia maiúsculas de minúsculas.  
- Executando pesquisas de cadeia de caracteres de correspondência exata ou prefixo. 
- Executando pesquisas de bitmask.
- Pesquisa de itens que tenham um conjunto de propriedades específico, independentemente do valor.
- Pesquisando pastas.
- Criar pastas de pesquisa.
    
## <a name="determine-what-type-of-search-filter-you-need"></a>Determinar que tipo de filtro de pesquisa você precisa
<a name="bk_SelectFilter"> </a>

Antes de criar um filtro de pesquisa, determine primeiro qual tipo de filtro você precisa. Os tipos de filtro são implementados como classes descendentes da classe [SearchFilter](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) na API gerenciada do EWS e como elementos filho do elemento [Restriction](https://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) no EWS. 
  
**Tabela 1. Tipos de filtros de pesquisa**

|**Tipo de filtro**|**Classe de API gerenciada do EWS**|**Elemento do EWS**|**Descrição**|
|:-----|:-----|:-----|:-----|
|Contém filtro  <br/> |[ContainsSubstring](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) <br/> |[Contém](https://msdn.microsoft.com/library/476d059d-c243-43e9-b475-319fc413ade2%28Office.15%29.aspx) <br/> |O melhor tipo de filtro a ser usado para comparações de cadeia de caracteres. Ele permite controlar a diferenciação entre maiúsculas e minúsculas, se deve ignorar o espaço em branco e definir o modo de confinamento.  <br/> |
|Filtro de bitmask  <br/> |[ExcludesBitmask](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.excludesbitmask%28v=exchg.80%29.aspx) <br/> |[Exclui](https://msdn.microsoft.com/library/bbaeddf6-9a67-4ee0-af99-7a7a5bbdc0e1%28Office.15%29.aspx) <br/> |Permite pesquisar Propriedades de inteiros como bitmasks e retornar apenas resultados que tenham bits correspondentes à desdefinição de bitmask especificada.  <br/> |
|Filtro existe  <br/> |[Existe](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.exists%28v=exchg.80%29.aspx) <br/> |[Existe](https://msdn.microsoft.com/library/55d568bd-8dbc-4d50-b9d7-54b74a54d4b5%28Office.15%29.aspx) <br/> |Retorna todos os itens que têm a propriedade especificada presente, independentemente do valor.  <br/> |
|Filtro de igualdade  <br/> |[IsEqualTo](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.isequalto%28v=exchg.80%29.aspx) <br/> [IsNotEqualTo](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.isnotequalto%28v=exchg.80%29.aspx) <br/> |[IsEqualTo](https://msdn.microsoft.com/library/48e7e067-049c-4184-8026-071e6f558e8a%28Office.15%29.aspx) <br/> [IsNotEqualTo](https://msdn.microsoft.com/library/e2eff26c-3403-45cd-bb74-1eb98c7dbfcd%28Office.15%29.aspx) <br/> |Compara o valor da propriedade especificada com um valor de constante especificado ou o valor de outra propriedade e retorna todos os itens que têm um valor igual (no caso de um filtro **IsEqualTo** ) ou um valor não igual (no caso de um filtro **IsNotEqualTo** ).  <br/> |
|Filtro de teste relacional  <br/> |[IsGreaterThan](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.isgreaterthan%28v=exchg.80%29.aspx) <br/> [IsGreaterThanOrEqualTo](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.isgreaterthanorequalto%28v=exchg.80%29.aspx) <br/> [IsLessThan](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.islessthan%28v=exchg.80%29.aspx) <br/> [IsLessThanOrEqualTo](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.islessthanorequalto%28v=exchg.80%29.aspx) <br/> |[IsGreaterThan](https://msdn.microsoft.com/library/a6e9d462-cfa7-40ec-903e-128c95050352%28Office.15%29.aspx) <br/> [IsGreaterThanOrEqualTo](https://msdn.microsoft.com/library/373cc954-314d-40e2-be03-cc08aefc0d5b%28Office.15%29.aspx) <br/> [IsLessThan](https://msdn.microsoft.com/library/2550469b-6e5d-45a5-9ecc-090d1b409296%28Office.15%29.aspx) <br/> [IsLessThanOrEqualTo](https://msdn.microsoft.com/library/b5d85eb2-5e15-4d01-ad49-6289e735ad8a%28Office.15%29.aspx) <br/> |Retorna todos os itens que têm um valor para a propriedade especificada na relação apropriada para um valor de constante especificado ou outra propriedade. Por exemplo, um filtro **IsGreaterThan** retorna todos os itens que têm um valor maior do que o valor especificado na propriedade especificada.  <br/> |
|Negando filtro  <br/> |[Not](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.not%28v=exchg.80%29.aspx) <br/> |[Not](https://msdn.microsoft.com/library/1aa16318-7e90-4b19-bce8-dd1a20a66223%28Office.15%29.aspx) <br/> |Nega o resultado dos outros filtros.  <br/> |
|Filtro composto  <br/> |[SearchFilterCollection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) <br/> |[And](https://msdn.microsoft.com/library/790246c2-37ad-49a8-91b9-6186d743b011%28Office.15%29.aspx) <br/> [Or](https://msdn.microsoft.com/library/4876d83a-73a3-4953-9d95-3048e6b76ccb%28Office.15%29.aspx) <br/> |Combina vários filtros, permitindo critérios de pesquisa mais complexos.  <br/> |
   
### <a name="contains-filter"></a>Contém filtro

Um filtro contém é a melhor opção para pesquisar Propriedades de cadeia de caracteres. Com um filtro Contains, você pode controlar os aspectos da correspondência de cadeia de caracteres, como diferenciação de maiúsculas e minúsculas e como o espaço em branco é tratado, definindo o modo de confinamento e o modo de comparação.
  
#### <a name="contains-filter-in-the-ews-managed-api"></a>Contém o filtro na API gerenciada do EWS
<a name="bk_ContainsEWSMA"> </a>

Se você estiver usando a API gerenciada do EWS, defina o modo de contenção usando a propriedade [ContainmentMode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.containmentmode%28v=exchg.80%29.aspx) da classe [ContainsSubstring](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) e defina o modo de comparação usando a propriedade [comparisonmode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.comparisonmode%28v=exchg.80%29.aspx) da classe **ContainsSubstring** . O exemplo a seguir mostra como criar um filtro de pesquisa que pesquisa o campo de assunto de itens da subcadeia de caracteres "anotações da reunião". Este exemplo ignora maiúsculas e minúsculas, mas não ignora espaço em branco. 
  
```cs
// Find all items with a subject that contain the substring
// "meeting notes", regardless of case.
// Matches include:
//   - meeting notes
//   - Meeting Notes
//   - Here are my meeting notes
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
```

#### <a name="contains-filter-in-ews"></a>Contém o filtro no EWS
<a name="bk_ContainsEWSMA"> </a>

No EWS, você define o modo de contenção usando o atributo **ContainmentMode** no elemento [Contains](https://msdn.microsoft.com/library/476d059d-c243-43e9-b475-319fc413ade2%28Office.15%29.aspx) e define o modo de comparação usando o atributo **ContainmentComparison** no elemento **Contains** . O exemplo a seguir mostra como criar um filtro de pesquisa para pesquisar o campo de assunto de itens da subcadeia de caracteres "anotações da reunião". Este exemplo ignora maiúsculas e minúsculas, mas não ignora espaço em branco. 
  
```XML
<t:Contains ContainmentMode="Substring" ContainmentComparison="IgnoreCase">
  <t:FieldURI FieldURI="item:Subject" />
  <t:Constant Value="meeting notes" />
</t:Contains>
```

### <a name="bitmask-filter"></a>Filtro de bitmask

Um filtro de bitmask permite que você pesquise Propriedades de inteiros como bitmasks e retorne resultados em que os bits específicos não são definidos no valor da propriedade especificada.
  
#### <a name="bitmask-filter-in-the-ews-managed-api"></a>Filtro de bitmask na API gerenciada do EWS

O exemplo a seguir mostra como usar a API gerenciada do EWS para criar um filtro de pesquisa para retornar todos os itens que têm um valor na propriedade personalizada **ItemIndex** (definido no [exemplo: localizar itens usando um filtro de pesquisa e a seção de API gerenciada do EWS](#bk_ExampleEWSMA) deste artigo) que não têm o segundo conjunto (10 em binário) definido. 
  
```cs
// Find all items with a value of the custom property that does not
// have the second bit (0010) set.
// Matches include:
//   - Property not set
//   - 1 (0001)
//   - 4 (0100)
//   - 5 (0101)
//   - 8 (1000)
SearchFilter.ExcludesBitmask bit2NotSetFilter = 
    new SearchFilter.ExcludesBitmask(customPropDefinition, 2);
```

#### <a name="bitmask-filter-in-ews"></a>Filtro de bitmask no EWS

O exemplo a seguir mostra como usar o EWS para criar um filtro de pesquisa para retornar todos os itens que têm um valor na propriedade personalizada **ItemIndex** (definida no [exemplo: localizar itens usando um filtro de pesquisa e a seção de API gerenciada do EWS](#bk_ExampleEWSMA) deste artigo) que não têm o segundo conjunto (10 em binário) definido. 
  
```XML
<t:Excludes>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:Bitmask Value="2" />
</t:Excludes>
```

### <a name="exists-filter"></a>Filtro existe

Um filtro Exists permite pesquisar itens que tenham uma propriedade específica definida, independentemente do valor.
  
#### <a name="exists-filter-in-the-ews-managed-api"></a>Existe filtro na API gerenciada do EWS

O exemplo a seguir mostra como criar um filtro de pesquisa para retornar todos os itens que têm a propriedade personalizada **ItemIndex** definida. 
  
```cs
// Find all items that have the custom property set.
SearchFilter.Exists customPropSetFilter =
    new SearchFilter.Exists(customPropDefinition);
```

#### <a name="exists-filter-in-ews"></a>Existe filtro no EWS

O exemplo a seguir mostra como criar um filtro de pesquisa para retornar todos os itens que têm a propriedade personalizada **ItemIndex** definida. 
  
```XML
<t:Exists>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
</t:Exists>
```

### <a name="equality-filter"></a>Filtro de igualdade

Os filtros de igualdade permitem pesquisar todos os itens que têm um valor para a propriedade especificada que seja igual a um valor específico ou não é igual a um valor específico. O valor com o qual comparar pode ser um valor constante ou o valor de outra propriedade em cada item.
  
#### <a name="equality-filter-in-the-ews-managed-api"></a>Filtro de igualdade na API gerenciada do EWS

O exemplo a seguir mostra como usar a API gerenciada do EWS para criar um filtro de pesquisa para retornar todos os itens que não tenham sido lidos.
  
```cs
// Find all items that are not marked as read.
SearchFilter.IsEqualTo unreadFilter =
    new SearchFilter.IsEqualTo(EmailMessageSchema.IsRead, false);
```

O exemplo a seguir mostra como criar um filtro de pesquisa para retornar todos os itens que têm um valor na propriedade **ItemIndex** que não seja igual ao tamanho do item. 
  
```cs
// Find all items that are marked as read.
SearchFilter.IsNotEqualTo indexNotEqualToSizeFilter =
    new SearchFilter.IsNotEqualTo(customPropDefinition, ItemSchema.Size);
```

#### <a name="equality-filter-in-ews"></a>Filtro de igualdade no EWS

O exemplo a seguir mostra como usar o EWS para criar um filtro de pesquisa para retornar todos os itens que não tenham sido lidos.
  
```XML
<t:IsEqualTo>
  <t:FieldURI FieldURI="message:IsRead" />
  <t:FieldURIOrConstant>
    <t:Constant Value="false" />
  </t:FieldURIOrConstant>
</t:IsEqualTo>
```

O exemplo a seguir mostra como criar um filtro de pesquisa para retornar todos os itens que têm um valor na propriedade **ItemIndex** que não seja igual ao tamanho do item. 
  
```XML
<t:IsNotEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:FieldURI FieldURI="item:Size" />
  </t:FieldURIOrConstant>
</t:IsNotEqualTo>
```

### <a name="relational-testing-filter"></a>Filtro de teste relacional

Os filtros de teste relacionais permitem pesquisar todos os itens que têm um valor na propriedade especificada que seja maior que ( \> ), maior ou igual a ( \> =), menor que ( \< ) ou menor que ou igual a ( \< =) um valor especificado. O valor com o qual comparar pode ser um valor constante ou o valor de outra propriedade em cada item.
  
#### <a name="relational-testing-filter-in-the-ews-managed-api"></a>Filtro de teste relacional na API gerenciada do EWS

O exemplo a seguir mostra como usar a API gerenciada do EWS para criar filtros de pesquisa para retornar todos os itens com um valor na propriedade **ItemIndex** que tenha a relação especificada com o valor 3 da constante. 
  
```cs
// Find all items where the custom property value is > 3.
SearchFilter.IsGreaterThan greaterThanFilter =
    new SearchFilter.IsGreaterThan(customPropDefinition, 3);
// Find all items where the custom property value is >= 3.
SearchFilter.IsGreaterThanOrEqualTo greaterThanOrEqualFilter =
    new SearchFilter.IsGreaterThanOrEqualTo(customPropDefinition, ItemSchema.Size);
// Find all items where the custom property value is < 3.
SearchFilter.IsLessThan lessThanFilter =
    new SearchFilter.IsLessThan(customPropDefinition, 3);
// Find all items where the custom property value is <= 3.
SearchFilter.IsLessThanOrEqualTo lessThanOrEqualFilter =
    new SearchFilter.IsLessThanOrEqualTo(customPropDefinition, 3);
```

#### <a name="relational-testing-filter-in-ews"></a>Filtro de teste relacional no EWS

O exemplo a seguir mostra como usar o EWS para criar um filtro de pesquisa para retornar todos os itens com um valor na propriedade **ItemIndex** que seja maior do que o valor de constante 3. 
  
```XML
<t:IsGreaterThan>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsGreaterThan>
```

O exemplo a seguir mostra como criar um filtro de pesquisa para retornar todos os itens com um valor na propriedade **ItemIndex** que seja maior ou igual ao valor de constante 3. 
  
```XML
<t:IsGreaterThanOrEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsGreaterThanOrEqualTo>
```

O exemplo a seguir mostra como criar um filtro de pesquisa para retornar todos os itens com um valor na propriedade **ItemIndex** que seja menor do que o valor de constante 3. 
  
```XML
<t:IsLessThan>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsLessThan>
```

O exemplo a seguir mostra como criar um filtro de pesquisa para retornar todos os itens com um valor na propriedade **ItemIndex** que seja menor ou igual ao valor de constante 3. 
  
```XML
<t:IsLessThanOrEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsLessThanOrEqualTo>
```

### <a name="negating-filter"></a>Negando filtro

Um filtro de negação permite que você retenha outro filtro e obtenha os resultados opostos da pesquisa. Enquanto outros filtros retornam resultados que correspondam a critérios específicos, um filtro de negação retorna resultados que não coincidem com os critérios especificados pelo filtro ao qual é aplicado.
  
#### <a name="negating-filter-in-the-ews-managed-api"></a>Negando o filtro na API gerenciada do EWS

O exemplo a seguir mostra como usar a API gerenciada do EWS para criar um filtro de pesquisa para retornar todos os itens que não têm a subcadeia de caracteres "anotações da reunião" no assunto.
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
SearchFilter.Not subjectNotFilter =
    new SearchFilter.Not(subjectFilter);
```

#### <a name="negating-filter-in-ews"></a>Negando filtro no EWS

O exemplo a seguir mostra como criar um filtro de pesquisa para retornar todos os itens que não têm a subcadeia de caracteres "anotações da reunião" no assunto.
  
```XML
<t:Not>
  <t:Contains ContainmentMode="ExactPhrase" ContainmentComparison="IgnoreCase">
    <t:FieldURI FieldURI="item:Subject" />
    <t:Constant Value="meeting notes" />
  </t:Contains>
</t:Not>
```

### <a name="compound-filter"></a>Filtro composto

Um filtro composto permite combinar vários filtros para criar critérios de pesquisa mais complexos. Você pode combinar critérios usando os operadores lógicos e ou. Dessa forma, você pode realizar pesquisas como "todos os emails do Sadie Daniels que contêm" notas da reunião "no assunto".
  
#### <a name="compound-filter-in-the-ews-managed-api"></a>Filtro composto na API gerenciada do EWS

O exemplo a seguir mostra como usar a API gerenciada do EWS para criar um filtro de pesquisa que retorna todos os itens enviados do Sadie Daniels e que contêm "notas da reunião" no assunto.
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
EmailAddress manager = new EmailAddress("sadie@contoso.com");
SearchFilter.IsEqualTo fromManagerFilter =
    new SearchFilter.IsEqualTo(EmailMessageSchema.Sender, manager);
SearchFilter.SearchFilterCollection compoundFilter =
    new SearchFilter.SearchFilterCollection(LogicalOperator.And, subjectFilter, fromManagerFilter);
```

#### <a name="compound-filter-in-ews"></a>Filtro composto no EWS

O exemplo a seguir mostra como usar o EWS para criar um filtro de pesquisa que retorna todos os itens que são enviados do Sadie Daniels e que contêm "notas da reunião" no assunto.
  
```XML
<t:And>
  <t:Contains ContainmentMode="Substring" ContainmentComparison="IgnoreCase">
    <t:FieldURI FieldURI="item:Subject" />
    <t:Constant Value="meeting notes" />
  </t:Contains>
  <t:IsEqualTo>
    <t:FieldURI FieldURI="message:Sender" />
    <t:FieldURIOrConstant>
      <t:Constant Value="sadie@fourthcoffee.com" />
    </t:FieldURIOrConstant>
  </t:IsEqualTo>
</t:And>
```

## <a name="example-find-items-by-using-a-search-filter-and-the-ews-managed-api"></a>Exemplo: localizar itens usando um filtro de pesquisa e a API gerenciada do EWS
<a name="bk_ExampleEWSMA"> </a>

Os seguintes métodos de API gerenciada do EWS usam filtros de pesquisa:
  
- [ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
- [ExchangeService. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
- [Folder. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
- [Folder. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
O exemplo a seguir usa o método **ExchangeService. FindItems** ; no entanto, as mesmas regras e conceitos se aplicam a todos os métodos. Neste exemplo, um método chamado **SearchWithFilter** é definido. Ele usa um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , um objeto [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) e um objeto [SearchFilter](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) como parâmetros. Este exemplo pressupõe que o objeto **ExchangeService** tenha sido inicializado com valores válidos nas propriedades de [credenciais](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) e [URL](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) . A classe **SearchFilter** é a classe base para todos os diferentes filtros de pesquisa. 
  
```cs
using Microsoft.Exchange.WebServices.Data
private static Guid SearchTestGUID = new Guid("{AA3DF801-4FC7-401F-BBC1-7C93D6498C2E}");
private static ExtendedPropertyDefinition customPropDefinition =
        new ExtendedPropertyDefinition(SearchTestGUID, "ItemIndex", MapiPropertyType.Integer);
static void SearchWithFilter(ExchangeService service, WellKnownFolderName folder, SearchFilter filter)
{
    // Limit the result set to 10 items.
    ItemView view = new ItemView(10);
    view.PropertySet = new PropertySet(ItemSchema.Subject, 
                                       ItemSchema.DateTimeReceived,
                                       EmailMessageSchema.IsRead,
                                       customPropDefinition);
    // Item searches do not support Deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Sorting.
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    try
    {
        FindItemsResults<Item> results = service.FindItems(folder, filter, view);
        foreach (Item item in results.Items)
        {
            Console.WriteLine("Subject: {0}", item.Subject);
            Console.WriteLine("Id: {0}", item.Id.ToString());
            if (item.ExtendedProperties.Count > 0 &&
                 item.ExtendedProperties[0].PropertyDefinition == customPropDefinition)
            {
                Console.WriteLine("Search Index: {0}", item.ExtendedProperties[0].Value);
            }
            if (item is EmailMessage)
            {
                EmailMessage message = item as EmailMessage;
                Console.WriteLine("Read: {0}", message.IsRead.ToString());
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

Você pode usar essa função com qualquer um dos filtros de pesquisa mostrados nos exemplos deste artigo. Este exemplo usa um filtro composto para retornar todos os itens na caixa de entrada de Sadie Daniels com "notas da reunião" no assunto.
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
EmailAddress manager = new EmailAddress("sadie@contoso.com");
SearchFilter.IsEqualTo fromManagerFilter =
    new SearchFilter.IsEqualTo(EmailMessageSchema.Sender, manager);
SearchFilter.SearchFilterCollection compoundFilter =
    new SearchFilter.SearchFilterCollection(LogicalOperator.And, subjectFilter, greaterThanFilter);
SearchWithFilter(service, WellKnownFolderName.Inbox, compoundFilter);
```

## <a name="example-find-an-item-by-using-a-search-filter-and-ews"></a>Exemplo: localizar um item usando um filtro de pesquisa e o EWS
<a name="bk_ExampleEWS"> </a>

As operações do EWS a seguir usam filtros de pesquisa:
  
- [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
- [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
O exemplo a seguir usa a operação **FindItem** ; no entanto, as mesmas regras e conceitos se aplicam às duas operações. Os filtros de pesquisa estão contidos no elemento [Restriction](https://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) nas solicitações SOAP. Este exemplo envia uma solicitação SOAP equivalente à pesquisa mostrada no exemplo anterior de API gerenciada do EWS. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="item:DateTimeReceived" />
          <t:FieldURI FieldURI="message:IsRead" />
          <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="10" Offset="0" BasePoint="Beginning" />
      <m:Restriction>
        <t:And>
          <t:Contains ContainmentMode="Substring" ContainmentComparison="IgnoreCase">
            <t:FieldURI FieldURI="item:Subject" />
            <t:Constant Value="meeting notes" />
          </t:Contains>
          <t:IsEqualTo>
            <t:FieldURI FieldURI="message:Sender" />
            <t:FieldURIOrConstant>
              <t:Constant Value="sadie@contoso.com" />
            </t:FieldURIOrConstant>
          </t:IsEqualTo>
        </t:And>
      </m:Restriction>
      <m:SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:FieldOrder>
      </m:SortOrder>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

O exemplo a seguir mostra a resposta do servidor, incluindo os resultados da pesquisa.
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="3" TotalItemsInView="3" IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>meeting notes</t:Subject>
                <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
                  <t:Value>5</t:Value>
                </t:ExtendedProperty>
                <t:IsRead>true</t:IsRead>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Meeting Notes</t:Subject>
                <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
                  <t:Value>6</t:Value>
                </t:ExtendedProperty>
                <t:IsRead>true</t:IsRead>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Meeting notes</t:Subject>
                <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
                  <t:Value>7</t:Value>
                </t:ExtendedProperty>
                <t:IsRead>true</t:IsRead>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="next-steps"></a>Próximas etapas
<a name="bk_ExampleEWS"> </a>

Agora que você está familiarizado com o uso de filtros de pesquisa em pesquisas básicas, é possível passar para técnicas de pesquisa mais avançadas.
  
- [Executar pesquisas agrupadas usando o EWS no Exchange](how-to-perform-grouped-searches-by-using-ews-in-exchange.md)
    
- [Executar pesquisas paginadas usando o EWS no Exchange](how-to-perform-paged-searches-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>Confira também

- [Pesquisar e EWS no Exchange](search-and-ews-in-exchange.md)    
- [Executar uma pesquisa do AQS usando o EWS no Exchange](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md)   
- [ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [ExchangeService. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)    
- [Folder. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)    
- [Folder. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)    
- [Operação FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)   
- [Operação FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

