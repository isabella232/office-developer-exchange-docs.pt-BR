---
title: Pesquisar e EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 9fa5b836-857e-401d-9450-51e7dbc69104
description: Descubra como pesquisar itens no Exchange usando a API gerenciada do EWS ou o EWS.
ms.openlocfilehash: d35cc74ab2fa79530ac09256e315a780023d833b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463829"
---
# <a name="search-and-ews-in-exchange"></a>Pesquisar e EWS no Exchange

Descubra como pesquisar itens no Exchange usando a API gerenciada do EWS ou o EWS.

Significa este som está familiarizado? Por fim, você está iniciando o projeto que está sendo desligado por semanas e precisa de informações sobre o projeto enviado por seu gerente por email semanas atrás. Sua caixa de entrada tem centenas ou milhares de mensagens. O que você faz? Você rola pela verificação de email cada assunto e remetente até encontrá-lo? Ou você usa o recurso de pesquisa no seu cliente de email favorito para rapidamente zero no que precisa?

A pesquisa é, supostamente, um recurso necessário para qualquer cliente de email. Mas a pesquisa pode ser usada para muito mais do que apenas permitir que os usuários pesquisem suas caixas de correio. Seu aplicativo precisa processar compromissos que estejam dentro de janelas de tempo específicas? Talvez você precise relatar todos os itens de tarefa com um status específico ou mover todos os contatos com um nome de empresa específico para uma pasta diferente. A pesquisa pode ajudar com todos esses requisitos.

## <a name="search-basics"></a>Noções básicas de pesquisa
<a name="bk_SearchBasics"> </a>

A API gerenciada do EWS e o EWS oferecem dois métodos básicos para especificar uma pesquisa. Você pode usar um [filtro de pesquisa](how-to-use-search-filters-with-ews-in-exchange.md) ou uma [cadeia de caracteres de consulta](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md). O método que você usa depende do intuito por trás da pesquisa.

**Tabela 1. Cenários para filtros de pesquisa e consultas de pesquisa**

|**Se você quiser...**|**Use um...**|**Anotações**|
|:-----|:-----|:-----|
|Limitar a pesquisa a uma propriedade específica ou a um conjunto de propriedades  <br/> |Filtro de pesquisa  <br/> |Os filtros de pesquisa fornecem o melhor nível de controle sobre quais propriedades são pesquisadas. Embora as cadeias de caracteres de consulta possam direcionar um conjunto limitado de propriedades usando a sintaxe de consulta avançada (AQS), os filtros de pesquisa podem direcionar qualquer propriedade.  <br/> |
|Criar pesquisas com vários critérios  <br/> |Filtro de pesquisa  <br/> |Com os filtros de pesquisa, vários critérios de pesquisa podem ser agrupados com o es lógico ou o ORs, permitindo pesquisas como "as anotações da reunião" e o remetente são iguais a "Sadie Daniels" ". Embora as cadeias de caracteres de consulta também possam ingressar em vários critérios de pesquisa, elas estão limitadas ao conjunto de propriedades suportado por cadeias de caracteres de consulta  <br/> |
|Propriedades personalizadas de pesquisa  <br/> |Filtro de pesquisa  <br/> |Os filtros de pesquisa podem direcionar Propriedades personalizadas. As cadeias de caracteres de consulta não pesquisam propriedades personalizadas.  <br/> |
|Executar uma pesquisa sensível ao caso de propriedades de cadeia de caracteres  <br/> |Filtro de pesquisa  <br/> |Pesquisas de sequências de consulta não diferenciam maiúsculas de minúsculas.  <br/> |
|Controlar o modo de contenção ao pesquisar Propriedades de cadeia de caracteres  <br/> |Filtro de pesquisa  <br/> |Pesquisas de cadeia de caracteres de consulta sempre são pesquisas de subcadeias. Se você precisar pesquisar por prefixos específicos ou exigir correspondências exatas, um filtro de pesquisa será a melhor opção.  <br/> |
|Procurar pastas  <br/> |Filtro de pesquisa  <br/> |O EWS não oferece suporte à pesquisa de pastas com uma cadeia de caracteres de consulta.  <br/> |
|Criar uma pasta de pesquisa  <br/> |Filtro de pesquisa  <br/> |O EWS não oferece suporte à criação de pastas de pesquisa com uma cadeia de caracteres de consulta.  <br/> |
|Pesquisar em todas as propriedades usadas com frequência  <br/> |Cadeia de caracteres de consulta  <br/> |As cadeias de caracteres de consulta que não contenham AQS pesquisará em todas as propriedades usadas com frequência. Por exemplo, um valor de cadeia de caracteres de consulta de "chaves Mack" retornará todas as mensagens enviadas por chaves do Mack, bem como qualquer mensagem que tenha "chaves Mack" no corpo ou no assunto.  <br/> |
|Criar uma pesquisa com base na entrada simples do usuário  <br/> |Cadeia de caracteres de consulta  <br/> |Uma cadeia de caracteres de consulta é uma ótima escolha para permitir que um usuário final faça uma pesquisa rápida digitando em uma cadeia de caracteres simples. Como uma pesquisa de cadeia de caracteres de consulta inclui todas as propriedades comumente usadas, os resultados conterá qualquer item que contenha os termos de pesquisa do usuário.  <br/> |

### <a name="using-a-search-filter"></a>Usando um filtro de pesquisa

Os filtros de pesquisa oferecem uma ampla variedade de opções de pesquisa e o maior grau de controle sobre como a pesquisa é realizada. Você pode usar filtros de pesquisa para executar pesquisas básicas de igualdade e comparação, mas você também pode pesquisar dentro do conteúdo das propriedades de cadeia de caracteres ou fazer comparações de bitmask.

Por exemplo, você pode pesquisar o conteúdo do assunto de itens usando a classe [SearchFilter. ContainsSubstring](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) na API gerenciada do EWS. Neste exemplo, um filtro de pesquisa é criado para pesquisar o assunto da subcadeia de caracteres "anotações da reunião", ignorando maiúsculas e minúsculas.

```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
```

Você também pode pesquisar em Propriedades personalizadas. Neste exemplo, a propriedade personalizada **ItemIndex** é pesquisada por valores maiores que 3.

```cs
Guid MyAppGuid = new Guid("{AA3DF801-4FC7-401F-BBC1-7C93D6498C2E}");
ExtendedPropertyDefinition customPropDefinition =
    new ExtendedPropertyDefinition(MyAppGuid, "ItemIndex", MapiPropertyType.Integer);
SearchFilter.IsGreaterThan customPropFilter =
    new SearchFilter.IsGreaterThan(customPropDefinition, 3);
```

Você também pode combinar vários filtros de pesquisa para criar pesquisas mais complexas. Por exemplo, você pode combinar os dois filtros anteriores com um lógica e usando a classe [SearchFilter. SearchFilterCollection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) .

```cs
SearchFilter.SearchFilterCollection compoundFilter =
    new SearchFilter.SearchFilterCollection(LogicalOperator.And, subjectFilter, customPropFilter);
```

### <a name="using-a-query-string"></a>Usando uma cadeia de caracteres de consulta

As cadeias de caracteres de consulta oferecem uma abordagem diferente à pesquisa. Você tem menos controle sobre os campos pesquisados e como a pesquisa é realizada quando você usa uma pesquisa de cadeia de caracteres de consulta. Isso não é nada ruim! Em alguns casos, você pode querer transmitir uma rede mais ampla, portanto, para falar.

Por exemplo, você pode pesquisar por "anotações da reunião" usando o método de API gerenciada do EWS [ExchangeService. FindItems](https://msdn.microsoft.com/library/jj223808%28v=exchg.80%29.aspx) .

```cs
FindItemsResults<Item> results = service.FindItems(folder, "meeting notes", view);
```

Se você comparar os resultados da pesquisa com os resultados do exemplo de pesquisa **SearchFilter. ContainsSubstring** anteriormente, essa pesquisa conterá mais resultados. A pesquisa de filtro de pesquisa retornará apenas os itens que têm "anotações da reunião" no assunto, enquanto esta pesquisa retornará itens que têm "anotações da reunião" no assunto, corpo e outros campos.

Vamos dar uma olhada em como você pode refinar a cadeia de caracteres de consulta para se aproximar dos resultados que vê do filtro de pesquisa. Usando o AQS, você pode limitar a pesquisa ao assunto.

```cs
FindItemsResults<Item> results = service.FindItems(folder, "subject:meeting notes", view);
```

Isso é mais próximo, mas os resultados ainda não são exatamente os mesmos. Quando você usa uma cadeia de caracteres de consulta com várias palavras, você obtém correspondências mesmo se as palavras não estiverem na ordem especificada ou mesmo se não estiverem adjacentes entre si. Com a cadeia de caracteres de consulta "assunto: anotações da reunião", você receberá correspondências para "anotações da reunião", "anotações da reunião" e assim por diante. Para refinar ainda mais, você pode quebrar os termos de pesquisa em aspas duplas para indicar que você deseja apenas essa frase.

```cs
FindItemsResults<Item> results = service.FindItems(folder, "subject:\"meeting notes\"", view);
```

## <a name="requesting-specific-properties-in-search-results"></a>Solicitando propriedades específicas nos resultados da pesquisa
<a name="bk_RequestSpecific"> </a>

Por padrão, os resultados da pesquisa conterá todas as propriedades dos itens que correspondem à pesquisa. Em alguns casos, pode ser o que você deseja, mas, na maioria dos casos, seu aplicativo requer apenas um conjunto discreto de propriedades. Nesse caso, você deve limitar o conjunto de propriedades que são retornadas somente para as propriedades que seu aplicativo precisa. No exemplo a seguir, a classe item [View](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) é usada para limitar as propriedades retornadas ao assunto, data/hora recebidas e ID dos itens.

```cs
ItemView view = new ItemView(10);
// Creating a new PropertySet with this constructor includes
// ItemSchema.Id.
view.PropertySet = new PropertySet(ItemSchema.Subject, ItemSchema.DateTimeReceived);
```

## <a name="controlling-search-depth"></a>Controle da profundidade da pesquisa
<a name="bk_SearchDepth"> </a>

Definir a passagem no modo de exibição controla a profundidade e o escopo da pesquisa.

**Tabela 2. Valores de passagem de pesquisa**

|**Valor de passagem**|**Aplica-se a**|**Descrição**|
|:-----|:-----|:-----|
|Superficial  <br/> |Itens e pastas  <br/> |Pesquisas superficiais limitam-se aos filhos diretos da pasta que está sendo pesquisada.  <br/> |
|Detalhadas  <br/> |Itens (somente com pastas de pesquisa) e pastas  <br/> |Pesquisas profundas pesquisa recursivamente a pasta que está sendo pesquisada e as subpastas.  <br/> |
|Ao  <br/> |Itens  <br/> |As pesquisas associadas incluem apenas itens associados da pasta que está sendo pesquisada. Os itens associados são itens ocultos dentro da pasta.  <br/> |
|SoftDeleted  <br/> |Itens e pastas  <br/> |Esse tipo de passagem é preterido. As pesquisas do SoftDeleted incluem apenas itens que estão no dumpster. O dumpster foi substituído pela [pasta itens recuperáveis](https://docs.microsoft.com/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder) no Exchange Online, Exchange Online como parte do Office 365 e versões do Exchange a partir do Exchange 2010.  <br/> |

## <a name="managing-search-results"></a>Gerenciar resultados de pesquisa
<a name="bk_ManageSearchResults"> </a>

A API gerenciada do EWS e o EWS também permitem que você altere como os resultados da pesquisa são retornados. Você pode usar modos de exibição para especificar quais propriedades são incluídas nos resultados, classificar resultados e paginar os resultados para obter apenas um número definido de resultados por resposta. Você também pode agrupar resultados por valores de campo específicos e controlar a profundidade de uma pesquisa especificando um tipo de passagem. Por fim, você pode usar pastas de pesquisa para criar pesquisas persistentes que são atualizadas dinamicamente à medida que novos itens chegam.

### <a name="sorting"></a>Classificação

Você pode obter o servidor para retornar os resultados classificados, o que pode facilitar a exibição ou o processamento de itens na ordem. Neste exemplo, os resultados serão classificados pela data/hora de recebimento, com os itens mais recentes em primeiro lugar.

```cs
view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
```

### <a name="paging"></a>Paginação

Ao enviar uma solicitação de pesquisa usando a API gerenciada do EWS ou o EWS, você especifica um tamanho de exibição, que controla o número máximo de itens retornados. No entanto, o número de itens no servidor que correspondem à sua pesquisa pode ser maior do que o tamanho do modo de exibição. Nesse caso, o servidor indica que há mais itens disponíveis. Você pode [usar paginação para repetir sua pesquisa](how-to-perform-paged-searches-by-using-ews-in-exchange.md) e obter o próximo conjunto de resultados.

Por exemplo, você pode enviar uma solicitação de pesquisa com um tamanho de exibição de 10. Pode haver 15 itens no servidor que correspondam à sua pesquisa, mas você só receberá as primeiras 10, juntamente com um indicador (o [FindItemsResults \<TItem\> . Propriedade MoreAvailable](https://msdn.microsoft.com/library/dd635477%28v=exchg.80%29.aspx) se você estiver usando a API gerenciada do EWS) que há mais resultados no servidor. Você pode então enviar a mesma pesquisa com um deslocamento de 10 para solicitar os dez próximos itens que correspondam à sua pesquisa. O servidor retornará os cinco itens restantes.

**Figura 1. Exemplo de pesquisa paginável**

![Uma ilustração que mostra uma pesquisa paginada. Uma solicitação inicial é enviada para 10 itens. Uma segunda solicitação é enviada para os próximos 10 itens.](media/Ex15_Search_PagedSearch.png)

### <a name="grouping"></a>Agrupamento

 O Exchange permite que você agrupe os resultados da pesquisa por um campo específico. Isso pode ajudar a dividir os resultados da pesquisa em conjuntos mais gerenciáveis. Por exemplo, você pode pesquisar por "anotações da reunião" e agrupar os resultados por remetente. Como mostra a figura a seguir, os itens retornados serão separados em grupos, com todos os itens que correspondam aos critérios do mesmo remetente em um grupo, todos os itens correspondentes de outro remetente em outro grupo e assim por diante.

**Figura 2. Resultados de pesquisa agrupados por remetente**

![Uma ilustração que mostra os resultados da pesquisa agrupados por remetente.](media/Ex15_Search_GroupedResults.png)

## <a name="search-folders"></a>Pastas de pesquisa
<a name="bk_SearchFolders"> </a>

Com uma pesquisa regular, a pesquisa é executada, os resultados são retornados ao aplicativo para processamento e a pesquisa deixa de existir. As pastas de pesquisa fornecem uma maneira de fazer uma pesquisa persistente. Essa é uma ótima opção para pesquisas que você sabe que deseja executar várias vezes. Em vez de executar a mesma pesquisa repetidamente, fazendo com que o servidor avalie a pesquisa do zero a cada vez, uma pasta de pesquisa faz uma pesquisa sempre ativa, permitindo que o servidor atualize o conjunto de resultados existente à medida que os itens são adicionados ou removidos do escopo de pesquisa. As pastas de pesquisa atuam como pastas regulares, pois elas aparecem como pastas com itens. A diferença é que os únicos itens contidos na pasta são aqueles que correspondem aos critérios de pesquisa associados à pasta. Depois que uma pasta de pesquisa é criada, seu aplicativo pode obter resultados atualizados da pesquisa apenas verificando o conteúdo da pasta.

A criação de uma pasta de pesquisa é simples quando você cria filtros de pesquisa. No exemplo a seguir, uma pasta de pesquisa é criada para mostrar todos os emails com um assunto que contém "notas da reunião".

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

- [Usar filtros de pesquisa com o EWS no Exchange](how-to-use-search-filters-with-ews-in-exchange.md)

- [Executar uma pesquisa do AQS usando o EWS no Exchange](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md)

- [Executar pesquisas paginadas usando o EWS no Exchange](how-to-perform-paged-searches-by-using-ews-in-exchange.md)

- [Executar pesquisas agrupadas usando o EWS no Exchange](how-to-perform-grouped-searches-by-using-ews-in-exchange.md)

- [Trabalhar com pastas de pesquisa usando o EWS no Exchange](how-to-work-with-search-folders-by-using-ews-in-exchange.md)

## <a name="see-also"></a>Confira também


- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)

- [Pasta itens recuperáveis](https://docs.microsoft.com/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder)

- [ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)

- [Limitação de parâmetros de política que afetam as operações de pesquisa do EWS](ews-throttling-in-exchange.md#throttling-policy-parameters-that-affect-ews-search-operations)
