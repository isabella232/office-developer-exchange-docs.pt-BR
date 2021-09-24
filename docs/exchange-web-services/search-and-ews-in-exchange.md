---
title: Pesquisa e EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 9fa5b836-857e-401d-9450-51e7dbc69104
description: Descubra como pesquisar itens em Exchange usando a API gerenciada do EWS ou o EWS.
ms.openlocfilehash: f78f4625880480e4f0d1ebb683c6e7c2c7fa83e0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524431"
---
# <a name="search-and-ews-in-exchange"></a>Pesquisa e EWS no Exchange

Descubra como pesquisar itens em Exchange usando a API gerenciada do EWS ou o EWS.

Significa este som está familiarizado? Você finalmente está iniciando o projeto que está adiando há semanas e precisa de informações sobre o projeto que seu gerente enviou por email semanas atrás. Sua Caixa de Entrada tem centenas ou talvez milhares de mensagens. O que você faz? Você rola seu email digitalizando cada assunto e remetente até encontrá-lo? Ou você usa o recurso de pesquisa em seu cliente de email favorito para fazer logo zero no que você precisa?

A pesquisa é, sem dúvida, um recurso necessário para qualquer cliente de email. Mas a pesquisa pode ser usada para muito mais do que apenas permitir que os usuários pesquisem suas caixas de correio. Seu aplicativo precisa processar compromissos que se enquadram em janelas de tempo específicas? Talvez você precise relatar todos os itens de tarefa com um status específico ou mover todos os contatos com um nome específico da empresa para uma pasta diferente. A pesquisa pode ajudar com todos esses requisitos.

## <a name="search-basics"></a>Noções básicas de pesquisa
<a name="bk_SearchBasics"> </a>

A API Gerenciada EWS e o EWS oferecem dois métodos básicos para especificar uma pesquisa. Você pode usar um [filtro de pesquisa](how-to-use-search-filters-with-ews-in-exchange.md) ou uma cadeia de [caracteres de consulta](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md). O método usado depende da intenção por trás da pesquisa.

**Tabela 1. Cenários para filtros de pesquisa e consultas de pesquisa**

|**Se você quiser...**|**Use um...**|**Observações**|
|:-----|:-----|:-----|
|Limitar sua pesquisa a uma propriedade específica ou conjunto de propriedades  <br/> |Filtro de pesquisa  <br/> |Os filtros de pesquisa fornecem o melhor nível de controle sobre quais propriedades são pesquisadas. Embora as cadeias de caracteres de consulta possam direcionar um conjunto limitado de propriedades usando a Sintaxe de Consulta Avançada (AQS), os filtros de pesquisa podem direcionar qualquer propriedade.  <br/> |
|Criar pesquisas com vários critérios  <br/> |Filtro de pesquisa  <br/> |Com os filtros de pesquisa, vários critérios de pesquisa podem ser unidos com ANDs lógicos ou ORs, permitindo pesquisas como "subject contains 'Meeting Notes' AND sender igual a 'Sadie Daniels'". Embora as cadeias de caracteres de consulta também possam ingressar em vários critérios de pesquisa, elas estão limitadas ao conjunto de propriedades suportadas por cadeias de caracteres de consulta.  <br/> |
|Pesquisar propriedades personalizadas  <br/> |Filtro de pesquisa  <br/> |Os filtros de pesquisa podem direcionar propriedades personalizadas. As cadeias de caracteres de consulta não pesquisam propriedades personalizadas.  <br/> |
|Executar uma pesquisa de minúsculas confidenciais de propriedades de cadeia de caracteres  <br/> |Filtro de pesquisa  <br/> |As pesquisas de cadeia de caracteres de consulta não são sensíveis a minúsculas.  <br/> |
|Controlar o modo de contenção ao pesquisar propriedades de cadeia de caracteres  <br/> |Filtro de pesquisa  <br/> |Pesquisas de cadeia de caracteres de consulta são sempre pesquisas de substring. Se você precisar pesquisar prefixos específicos ou exigir combinações exatas, um filtro de pesquisa é a melhor opção.  <br/> |
|Pesquisar pastas  <br/> |Filtro de pesquisa  <br/> |O EWS não dá suporte à pesquisa de pastas com uma cadeia de caracteres de consulta.  <br/> |
|Criar uma pasta de pesquisa  <br/> |Filtro de pesquisa  <br/> |O EWS não dá suporte à criação de pastas de pesquisa com uma cadeia de caracteres de consulta.  <br/> |
|Pesquisar em todas as propriedades comumente usadas  <br/> |Cadeia de caracteres de consulta  <br/> |Cadeias de caracteres de consulta que não contêm AQS pesquisarão em todas as propriedades comumente usadas. Por exemplo, um valor de cadeia de caracteres de consulta "Mack Chaves" retornará todas as mensagens enviadas por Mack Chaves, bem como qualquer mensagem que tenha "Mack Chaves" no corpo ou no assunto.  <br/> |
|Construir uma pesquisa com base na entrada de usuário simples  <br/> |Cadeia de caracteres de consulta  <br/> |Uma cadeia de caracteres de consulta é uma ótima opção para permitir que um usuário final faça uma pesquisa rápida digitando em uma cadeia de caracteres simples. Como uma pesquisa de cadeia de caracteres de consulta inclui todas as propriedades comumente usadas, os resultados conterão todos os itens que contenham os termos de pesquisa do usuário.  <br/> |

### <a name="using-a-search-filter"></a>Usando um filtro de pesquisa

Os filtros de pesquisa dão a você uma ampla variedade de opções de pesquisa e o maior grau de controle sobre como a pesquisa é realizada. Você pode usar filtros de pesquisa para executar pesquisas básicas de igualdade e comparação, mas também pode pesquisar no conteúdo das propriedades de cadeia de caracteres ou fazer comparações de bitmask.

Por exemplo, você pode pesquisar o conteúdo do assunto dos itens usando a classe [SearchFilter.ContainsSubstring](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) na API Gerenciada do EWS. Neste exemplo, um filtro de pesquisa é criado para pesquisar o assunto para a substring "meeting notes", ignorando o caso.

```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
```

Você também pode pesquisar propriedades personalizadas. Neste exemplo, a propriedade **personalizada ItemIndex** é pesquisada por valores maiores que 3.

```cs
Guid MyAppGuid = new Guid("{AA3DF801-4FC7-401F-BBC1-7C93D6498C2E}");
ExtendedPropertyDefinition customPropDefinition =
    new ExtendedPropertyDefinition(MyAppGuid, "ItemIndex", MapiPropertyType.Integer);
SearchFilter.IsGreaterThan customPropFilter =
    new SearchFilter.IsGreaterThan(customPropDefinition, 3);
```

Você também pode combinar vários filtros de pesquisa para criar pesquisas mais complexas. Por exemplo, você pode combinar os dois filtros anteriores com um E lógico usando a [classe SearchFilter.SearchFilterCollection.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx)

```cs
SearchFilter.SearchFilterCollection compoundFilter =
    new SearchFilter.SearchFilterCollection(LogicalOperator.And, subjectFilter, customPropFilter);
```

### <a name="using-a-query-string"></a>Usando uma cadeia de caracteres de consulta

Cadeias de caracteres de consulta fornecem uma abordagem diferente para a pesquisa. Você tem menos controle sobre os campos pesquisados e como a pesquisa é executada quando você usa uma pesquisa de cadeia de caracteres de consulta. Não que isso seja uma coisa ruim! Em alguns casos, talvez você queira lançar uma rede mais ampla, por assim dizer.

Por exemplo, você pode pesquisar "notas de reunião" usando o [método exchangeService.FindItems](https://msdn.microsoft.com/library/jj223808%28v=exchg.80%29.aspx) EWS Managed API.

```cs
FindItemsResults<Item> results = service.FindItems(folder, "meeting notes", view);
```

Se você comparar os resultados dessa pesquisa com os resultados do exemplo de pesquisa **SearchFilter.ContainsSubstring** anteriormente, essa pesquisa conterá mais resultados. A pesquisa de filtro de pesquisa retornará apenas itens que tenham "notas de reunião" no assunto, enquanto essa pesquisa retornará itens que tenham "anotações de reunião" no assunto, corpo e outros campos.

Vamos dar uma olhada em como você pode refinar a cadeia de caracteres de consulta para se aproximar dos resultados que você vê no filtro de pesquisa. Usando a AQS, você pode limitar sua pesquisa ao assunto.

```cs
FindItemsResults<Item> results = service.FindItems(folder, "subject:meeting notes", view);
```

Isso é mais próximo, mas os resultados ainda não são os mesmos. Quando você usa uma cadeia de caracteres de consulta com várias palavras, você receberá combinações mesmo se as palavras não estão na ordem especificada ou mesmo se elas não estão adjacentes umas às outras. Com a cadeia de caracteres de consulta "subject:meeting notes", você receberá as combinações de "notas de reunião", "anotações da reunião" e assim por diante. Para refinar ainda mais, você pode quebrar os termos de pesquisa entre aspas duplas para indicar que deseja apenas essa frase.

```cs
FindItemsResults<Item> results = service.FindItems(folder, "subject:\"meeting notes\"", view);
```

## <a name="requesting-specific-properties-in-search-results"></a>Solicitando propriedades específicas nos resultados da pesquisa
<a name="bk_RequestSpecific"> </a>

Por padrão, os resultados da pesquisa conterão todas as propriedades nos itens que corresponderem à pesquisa. Em alguns casos, isso pode ser o que você deseja, mas, na maioria dos casos, seu aplicativo requer apenas um conjunto discreto de propriedades. Nesse caso, você deve limitar o conjunto de propriedades que são retornadas apenas às propriedades que seu aplicativo precisa. No exemplo a seguir, a [classe ItemView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) é usada para limitar as propriedades retornadas ao assunto, data/hora recebida e ID dos itens.

```cs
ItemView view = new ItemView(10);
// Creating a new PropertySet with this constructor includes
// ItemSchema.Id.
view.PropertySet = new PropertySet(ItemSchema.Subject, ItemSchema.DateTimeReceived);
```

## <a name="controlling-search-depth"></a>Controlando a profundidade da pesquisa
<a name="bk_SearchDepth"> </a>

A definição da rotação no exibição controla a profundidade e o escopo da pesquisa.

**Tabela 2. Valores de pesquisa transnacionais**

|**Valor percorrido**|**Aplica-se a**|**Descrição**|
|:-----|:-----|:-----|
|Superficial  <br/> |Itens e Pastas  <br/> |Pesquisas rasas são limitadas aos filhos diretos da pasta que está sendo pesquisada.  <br/> |
|Deep  <br/> |Itens (somente com pastas de pesquisa) e Pastas  <br/> |Pesquisas profundas pesquisam recursivamente a pasta que está sendo pesquisada e subpastas.  <br/> |
|Associado  <br/> |Itens  <br/> |As pesquisas associadas incluem apenas itens associados da pasta que está sendo pesquisada. Os itens associados são itens ocultos dentro da pasta.  <br/> |
|SoftDeleted  <br/> |Itens e Pastas  <br/> |Esse tipo de atravessamento é preterido. As pesquisas SoftDeleted incluem apenas itens que estão na lixeira. A lixeira foi substituída [](https://docs.microsoft.com/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder) pela Pasta de Itens Recuperáveis no Exchange Online, Exchange Online como parte do Office 365 e versões do Exchange a partir do Exchange 2010.  <br/> |

## <a name="managing-search-results"></a>Gerenciando resultados da pesquisa
<a name="bk_ManageSearchResults"> </a>

A API Gerenciada EWS e o EWS também permitem alterar como os resultados da pesquisa são retornados. Você pode usar exibições para especificar quais propriedades estão incluídas nos resultados, classificar resultados e página seus resultados para obter apenas um número definido de resultados por resposta. Você também pode agrupar resultados por valores de campo específicos e controlar a profundidade de uma pesquisa especificando um tipo atravessado. Por fim, você pode usar pastas de pesquisa para criar pesquisas persistentes que são atualizadas dinamicamente à medida que novos itens chegam.

### <a name="sorting"></a>Classificação

Você pode fazer com que o servidor retorne resultados organizados, o que pode facilitar a exibição ou o processamento de itens em ordem. Neste exemplo, os resultados serão organizados pela data/hora recebida, com os itens mais recentes sendo os primeiros.

```cs
view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
```

### <a name="paging"></a>Paginação

Quando você envia uma solicitação de pesquisa usando a API Gerenciada do EWS ou o EWS, especifica um tamanho de exibição, que controla o número máximo de itens retornados. No entanto, o número de itens no servidor que corresponderem à sua pesquisa pode ser maior do que o tamanho do visualização. Nesse caso, o servidor indica que mais itens estão disponíveis. Você pode [usar a paja para repetir sua pesquisa](how-to-perform-paged-searches-by-using-ews-in-exchange.md) e obter o próximo conjunto de resultados.

Por exemplo, você pode enviar uma solicitação de pesquisa com um tamanho de exibição de 10. Pode haver 15 itens no servidor que corresponderem à sua pesquisa, mas você só retornará os primeiros 10, juntamente com um indicador [(FindItemsResults \<TItem\> . Propriedade MoreAvailable](https://msdn.microsoft.com/library/dd635477%28v=exchg.80%29.aspx) se você estiver usando a API Gerenciada do EWS) que há mais resultados no servidor. Em seguida, você pode enviar a mesma pesquisa com um deslocamento de 10 para solicitar os próximos 10 itens que corresponderem à sua pesquisa. O servidor retornará os cinco itens restantes.

**Figura 1. Exemplo de pesquisa com página**

![Uma ilustração que mostra uma pesquisa paginada. Uma solicitação inicial é enviada para 10 itens. Uma segunda solicitação é enviada para os próximos 10 itens.](media/Ex15_Search_PagedSearch.png)

### <a name="grouping"></a>Agrupamento

 Exchange permite agrupar resultados de pesquisa por um campo específico. Isso pode ajudar a separar os resultados da pesquisa em conjuntos mais gerenciáveis. Por exemplo, você pode pesquisar por "notas de reunião" e agrupar os resultados por remetente. Conforme mostrado na figura a seguir, os itens retornados serão separados em grupos, com todos os itens que corresponderem aos critérios do mesmo remetente em um grupo, todos os itens correspondentes de outro remetente em outro grupo e assim por diante.

**Figura 2. Resultados da pesquisa agrupados por remetente**

![Uma ilustração que mostra os resultados da pesquisa agrupados por remetente.](media/Ex15_Search_GroupedResults.png)

## <a name="search-folders"></a>Pastas de pesquisa
<a name="bk_SearchFolders"> </a>

Com uma pesquisa regular, a pesquisa é executada, os resultados são retornados ao seu aplicativo para processamento e a pesquisa deixa de existir. As pastas de pesquisa fornecem uma maneira de tornar uma pesquisa persistente. Essa é uma ótima opção para pesquisas que você sabe que deseja executar várias vezes. Em vez de executar a mesma pesquisa repetidamente, fazendo com que o servidor avalie a pesquisa do zero sempre, uma pasta de pesquisa faz uma pesquisa sempre em, permitindo que o servidor atualize o conjunto de resultados existente à medida que os itens são adicionados ou removidos do escopo de pesquisa. As pastas de pesquisa agem como pastas regulares, pois elas aparecem como pastas que têm itens neles. A diferença é que os únicos itens contidos na pasta são aqueles que corresponderem aos critérios de pesquisa associados à pasta. Depois que uma pasta de pesquisa é criada, seu aplicativo pode obter resultados atualizados da pesquisa apenas verificando o conteúdo da pasta.

A criação de uma pasta de pesquisa é simples quando você domina a criação de filtros de pesquisa. No exemplo a seguir, uma pasta de pesquisa é criada para mostrar todos os emails com um assunto que contém "notas de reunião".

```cs
static void CreateSearchFolder(ExchangeService service)
{
    SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
        "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
    SearchFolder searchFolder = new SearchFolder(service);
    searchFolder.DisplayName = "Meeting Notes";
    searchFolder.SearchParameters.RootFolderIds.Add(WellKnownFolderName.Inbox);
    searchFolder.SearchParameters.Traversal = SearchFolderTraversal.Deep;
    searchFolder.SearchParameters.SearchFilter = subjectFilter;
    searchFolder.Save(WellKnownFolderName.SearchFolders);
}
```

## <a name="in-this-section"></a>Nesta seção
<a name="bk_InThisSection"> </a>

- [Usar filtros de pesquisa com EWS em Exchange](how-to-use-search-filters-with-ews-in-exchange.md)

- [Executar uma pesquisa AQS usando o EWS no Exchange](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md)

- [Executar pesquisas paginadas usando o EWS no Exchange](how-to-perform-paged-searches-by-using-ews-in-exchange.md)

- [Executar pesquisas agrupadas usando o EWS em Exchange](how-to-perform-grouped-searches-by-using-ews-in-exchange.md)

- [Trabalhar com pastas de pesquisa usando o EWS no Exchange](how-to-work-with-search-folders-by-using-ews-in-exchange.md)

## <a name="see-also"></a>Confira também


- [Desenvolver clientes do serviço Web para o Exchange](develop-web-service-clients-for-exchange.md)

- [Pasta Itens Recuperáveis](https://docs.microsoft.com/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder)

- [ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)

- [Parâmetros de política de throttling que afetam as operações de pesquisa do EWS](ews-throttling-in-exchange.md#throttling-policy-parameters-that-affect-ews-search-operations)
