---
title: Pesquisa e EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 9fa5b836-857e-401d-9450-51e7dbc69104
description: Descubra como pesquisar por itens no Exchange usando a API gerenciada de EWS ou EWS.
ms.openlocfilehash: da24258ba94b842fa97fff92148620344c939f05
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750956"
---
# <a name="search-and-ews-in-exchange"></a>Pesquisa e EWS no Exchange

Descubra como pesquisar por itens no Exchange usando a API gerenciada de EWS ou EWS.
  
Significa este som está familiarizado? Você está iniciando finalmente desse projeto que você tiver sido colocando por semanas e você precisa de informações sobre o projeto que seu gerente enviado a você em semanas de email atrás. Sua caixa de entrada possui centenas ou talvez milhares de mensagens. O que você faz? Você percorrer seu email verificação cada assunto e o remetente até que você encontrá-lo? Ou, você usa o recurso de pesquisa em seu cliente de email favorito como zero rapidamente no que você precisa?
  
Pesquisa relativamente é um recurso de obrigatórios para qualquer cliente de email. Mas a pesquisa pode ser usada para habilitar muito mais do que apenas os usuários procurem suas caixas de correio. Seu aplicativo precisa processar compromissos que ocorram dentro de períodos de tempo específico? Talvez você precisa enviar relatórios sobre todos os itens de tarefa com um status específico ou mova todos os contatos com um nome de empresa específica para uma pasta diferente. Pesquisa pode ajudar com todos esses requisitos.
  
## <a name="search-basics"></a>Noções básicas da pesquisa
<a name="bk_SearchBasics"> </a>

A API gerenciada de EWS e o EWS oferecem dois métodos básicos para especificar uma pesquisa. Você pode usar um [filtro de pesquisa](how-to-use-search-filters-with-ews-in-exchange.md) ou uma [cadeia de caracteres de consulta](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md). O método usado depende do intuito da sua pesquisa.
  
**Tabela 1. Cenários para filtros de pesquisa e consultas de pesquisa**

|**Se você quiser …**|**Use um …**|**Notes**|
|:-----|:-----|:-----|
|Limitar a pesquisa a uma propriedade específica ou um conjunto de propriedades  <br/> |Filtro de pesquisa  <br/> |Os filtros de pesquisa fornecem o melhor nível de controle sobre quais propriedades são pesquisadas. Embora as cadeias de caracteres de consulta podem direcionar um conjunto limitado de propriedades usando a sintaxe de consulta avançada (AQS), filtros de pesquisa podem direcionar qualquer propriedade.  <br/> |
|Criar pesquisas com vários critérios  <br/> |Filtro de pesquisa  <br/> |Com os filtros de pesquisa, vários critérios de pesquisa podem ser Unidos junto com lógica ANDs ou ORs, permitindo pesquisas como "assunto contém 'Notas de reunião' e o remetente é igual a 'Sadie Daniels'". Embora as cadeias de caracteres de consulta também podem ingressar em vários critérios de pesquisa, eles são limitados ao conjunto de propriedades suportadas pelo cadeias de caracteres de consulta.  <br/> |
|Propriedades personalizadas de pesquisa  <br/> |Filtro de pesquisa  <br/> |Filtros de pesquisa podem direcionar propriedades personalizadas. Cadeias de caracteres de consulta de pesquisa não propriedades personalizadas.  <br/> |
|Realizar uma pesquisa diferencia maiusculas de minúsculas das propriedades de cadeia de caracteres  <br/> |Filtro de pesquisa  <br/> |As pesquisas de cadeia de caracteres de consulta não diferenciam maiusculas de minúsculas.  <br/> |
|O modo de contenção ao pesquisar propriedades de cadeia de caracteres de controle  <br/> |Filtro de pesquisa  <br/> |As pesquisas de cadeia de caracteres de consulta são sempre pesquisas de subsequência. Se você precisar procurar prefixos específicos ou exigem correspondências exatas, um filtro de pesquisa é a melhor opção.  <br/> |
|Procurar pastas  <br/> |Filtro de pesquisa  <br/> |EWS não suporta procurando pastas com uma cadeia de caracteres de consulta.  <br/> |
|Crie uma pasta de pesquisa  <br/> |Filtro de pesquisa  <br/> |EWS não oferece suporte a criação de pastas de pesquisa com uma cadeia de caracteres de consulta.  <br/> |
|Pesquisa em todas as propriedades normalmente utilizadas  <br/> |Cadeia de caracteres de consulta  <br/> |Cadeias de caracteres de consulta que não contêm AQS pesquisará entre todas as propriedades comumente usadas. Por exemplo, um valor de cadeia de caracteres de consulta de "Mack Chaves" retornará todas as mensagens enviadas por Mack Chaves, bem como todas as mensagens que tenham "Mack Chaves" no corpo ou no assunto.  <br/> |
|Construir uma pesquisa com base na entrada do usuário simples  <br/> |Cadeia de caracteres de consulta  <br/> |Uma cadeia de caracteres de consulta é uma excelente opção para permitir que um usuário final fazer uma pesquisa rápida, digitando em uma cadeia de caracteres simple. Como uma pesquisa de cadeia de caracteres de consulta inclui todas as propriedades comumente usadas, os resultados conterá todos os itens que contenham os termos de pesquisa do usuário.  <br/> |
   
### <a name="using-a-search-filter"></a>Usando um filtro de pesquisa

Filtros de pesquisa lhe oferece uma ampla gama de opções de pesquisa e o maior grau de controle sobre como a pesquisa é realizada. Você pode usar filtros de pesquisa para realizar pesquisas de comparação e de igualdade básica, mas você também pode pesquisar dentro o conteúdo das propriedades de cadeia de caracteres ou fazer comparações de bitmask.
  
Por exemplo, você pode pesquisar o conteúdo do assunto de itens usando a classe [SearchFilter.ContainsSubstring](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) na API gerenciada do EWS. Neste exemplo, um filtro de pesquisa é criado para pesquisar o assunto a subcadeia de caracteres "notas de reunião," ignora maiusculas / minúsculas. 
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
```

Você também pode pesquisar contra propriedades personalizadas. Neste exemplo, a propriedade personalizada **ItemIndex** é pesquisada para valores maiores que 3. 
  
```cs
Guid MyAppGuid = new Guid("{AA3DF801-4FC7-401F-BBC1-7C93D6498C2E}");
ExtendedPropertyDefinition customPropDefinition =
    new ExtendedPropertyDefinition(MyAppGuid, "ItemIndex", MapiPropertyType.Integer); 
SearchFilter.IsGreaterThan customPropFilter =
    new SearchFilter.IsGreaterThan(customPropDefinition, 3);
```

Você também pode combinar vários filtros de pesquisa para criar pesquisas mais complexas. Por exemplo, você pode combinar os dois filtros anteriores com um AND lógico, usando a classe [SearchFilter.SearchFilterCollection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) . 
  
```cs
SearchFilter.SearchFilterCollection compoundFilter =
    new SearchFilter.SearchFilterCollection(LogicalOperator.And, subjectFilter, customPropFilter);
```

### <a name="using-a-query-string"></a>Usando uma cadeia de caracteres de consulta

Cadeias de caracteres de consulta fornecem uma abordagem diferente para pesquisar. Você tem menos controle sobre os campos que são pesquisados e como a pesquisa é executada quando você usa uma pesquisa de cadeia de caracteres de consulta. Não que é uma coisa ruim! Em alguns casos, talvez você queira convertida de uma rede mais ampla, por assim dizer.
  
Por exemplo, você pode pesquisar "notas de reunião" usando o método de API gerenciada de EWS [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/jj223808%28v=exchg.80%29.aspx) . 
  
```cs
FindItemsResults<Item> results = service.FindItems(folder, "meeting notes", view);
```

Se você comparar os resultados da pesquisa para os resultados do exemplo pesquisa **SearchFilter.ContainsSubstring** anteriormente, esta pesquisa irá conter mais resultados. A pesquisa de filtro de pesquisa retornará apenas os itens que possuem as "observações de reunião" no assunto, enquanto esta pesquisa irá retornar itens que tenham "anotações de reunião" no assunto, corpo e outros campos. 
  
Vamos analisar como você pode refinar a cadeia de caracteres de consulta para obter os resultados que você vê do filtro de pesquisa mais próximo. Usando AQS, você pode limitar a pesquisa para o assunto.
  
```cs
FindItemsResults<Item> results = service.FindItems(folder, "subject:meeting notes", view);
```

Isso é mais próximo, mas os resultados são ainda não exatamente iguais. Quando você usa uma cadeia de caracteres de consulta com várias palavras, você receberá correspondências mesmo se as palavras não estão na ordem especificada, ou mesmo se elas não estiverem adjacentes entre si. Com a sequência de consulta "Observações do assunto: reunião", você irá obter correspondências para "notas de reunião", "Observações da reunião" e assim por diante. Para refinar ainda mais, você poderá dispor os termos de pesquisa em aspas duplas para indicar que você deseja apenas essa frase.
  
```cs
FindItemsResults<Item> results = service.FindItems(folder, "subject:\"meeting notes\"", view);
```

## <a name="requesting-specific-properties-in-search-results"></a>Solicitando propriedades específicas nos resultados da pesquisa
<a name="bk_RequestSpecific"> </a>

Por padrão, os resultados da pesquisa irá conter todas as propriedades nos itens que correspondem a pesquisa. Em alguns casos, isso pode ser o que você deseja, mas na maioria dos casos seu aplicativo requer apenas um conjunto distinto de propriedades. Nesse caso, você deve limitar o conjunto de propriedades que são retornados para somente as propriedades de seu aplicativo precisa. No exemplo a seguir, a classe [ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) é usada para limitar as propriedades retornadas para o assunto, data/hora recebido e identificação dos itens. 
  
```cs
ItemView view = new ItemView(10);
// Creating a new PropertySet with this constructor includes 
// ItemSchema.Id.
view.PropertySet = new PropertySet(ItemSchema.Subject, ItemSchema.DateTimeReceived);
```

## <a name="controlling-search-depth"></a>Controlando a profundidade de pesquisa
<a name="bk_SearchDepth"> </a>

A definição de passagem no modo de exibição controla a profundidade e o escopo da pesquisa. 
  
**Tabela 2. Valores de passagem de pesquisa**

|**Valor de passagem**|**Aplica-se a**|**Descrição**|
|:-----|:-----|:-----|
|Raso  <br/> |Itens e pastas  <br/> |Pesquisas superficiais são limitadas para direcionar os filhos da pasta que estão sendo pesquisados.  <br/> |
|Profundo  <br/> |Pastas e itens (somente com pastas de pesquisa)  <br/> |Pesquisas de profundidade recursivamente pesquisar a pasta que estão sendo pesquisados e as subpastas.  <br/> |
|Associados  <br/> |Items  <br/> |Pesquisas associadas incluem apenas os itens associados da pasta que estão sendo pesquisados. Itens associados são itens ocultos dentro da pasta.  <br/> |
|SoftDeleted  <br/> |Itens e pastas  <br/> |Esse tipo de passagem foi preterido. Pesquisas de SoftDeleted incluem apenas os itens que estão no dumpster. O dumpster foi substituída pela [pasta itens recuperáveis](http://technet.microsoft.com/en-us/library/ee364755%28v=exchg.150%29.aspx(Office.15).aspx) no Exchange Online, o Exchange Online como parte do Office 365 e versões do Exchange, começando com o Exchange 2010.  <br/> |
   
## <a name="managing-search-results"></a>Gerenciando os resultados da pesquisa
<a name="bk_ManageSearchResults"> </a>

A API gerenciada de EWS e EWS também permitem que você altere como os resultados da pesquisa são retornados. Você pode usar os modos de exibição para especificar quais propriedades são incluídas nos resultados da, classificar os resultados e os resultados para obter apenas novamente um número de resultados por resposta de página. Você também pode agrupar resultados por valores de campo específicos e a profundidade de uma pesquisa de controle, especificando um tipo de passagem. Finalmente, você pode usar as pastas de pesquisa para criar pesquisas persistentes que são atualizadas dinamicamente à medida que novos itens chegam.
  
### <a name="sorting"></a>Classificação

Você pode obter o servidor para retornar resultados classificados, o que facilitam exibir ou processar itens na ordem. Neste exemplo, os resultados serão classificados pela data/hora recebida, com os itens mais recentes sendo primeiro.
  
```cs
view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
```

### <a name="paging"></a>Paginação

Quando você envia uma solicitação de pesquisa usando o EWS Managed API ou o EWS, você pode especificar um tamanho de modo de exibição, que controla o número máximo de itens retornados. No entanto, o número de itens no servidor que correspondem sua pesquisa pode ser maior que o tamanho do modo de exibição. Nesse caso, o servidor indica que mais itens estão disponíveis. Você pode [usar a paginação para repetir a pesquisa](how-to-perform-paged-searches-by-using-ews-in-exchange.md) e obtenha o próximo conjunto de resultados. 
  
Por exemplo, você pode enviar uma solicitação de pesquisa com um tamanho de modo de exibição de 10. Pode haver 15 itens no servidor que corresponde à sua pesquisa, mas você só receberá novamente os primeiros 10, juntamente com um indicador (o [FindItemsResults\<TItem\>. MoreAvailable](http://msdn.microsoft.com/en-us/library/dd635477%28v=exchg.80%29.aspx) propriedade se você estiver usando a API gerenciada de EWS) que não existem mais resultados no servidor. Em seguida, você pode enviar a mesma pesquisa com um deslocamento de 10 pedir os próximos 10 itens que correspondam à sua pesquisa. O servidor retornará os itens restantes de cinco. 
  
**Figura 1. Exemplo de pesquisa paginados**

![Uma ilustração que mostra uma pesquisa paginada. Uma solicitação inicial é enviada para 10 itens. Uma segunda solicitação é enviada para os próximos 10 itens.](media/Ex15_Search_PagedSearch.png)
  
### <a name="grouping"></a>Agrupamento

 Exchange permite aos resultados de pesquisa de grupo por um campo específico. Isso pode ajudar a dividir os resultados da pesquisa em conjuntos mais gerenciáveis. Por exemplo, você pode procurar "notas de reunião" e agrupar os resultados por remetente. Conforme mostrado na figura a seguir, os itens retornados serão separados em grupos, com todos os itens que correspondem aos critérios do mesmo remetente em um grupo, todos os itens correspondentes do remetente outra em outro grupo e assim por diante. 
  
**Figura 2. Resultados de pesquisa, agrupados por remetente**

![Uma ilustração que mostra os resultados da pesquisa agrupados por remetente.](media/Ex15_Search_GroupedResults.png)
  
## <a name="search-folders"></a>Pastas de pesquisa
<a name="bk_SearchFolders"> </a>

Com uma pesquisa regular, a pesquisa é executada, os resultados são retornados ao seu aplicativo para processamento e a pesquisa deixa de existir. Pastas de pesquisa fornecem uma maneira de fazer uma pesquisa persistentes. Isso é uma opção excelente para pesquisas que você sabe que você desejará executar várias vezes. Em vez de executá-lo a mesma pesquisa repetidamente, fazendo com que o servidor avaliar a pesquisa a partir do zero cada vez, uma pasta de pesquisa faz com que uma pesquisa sempre ativado, permitindo que o servidor atualizar o resultado existente definido como itens são adicionados à ou removidos do escopo da pesquisa. Act de pastas de pesquisa, como pastas regulares, em que eles aparecem como pastas que possuem itens neles. A diferença é que somente os itens contidos na pasta são aquelas que correspondem aos critérios de pesquisa que estão associados a pasta. Depois que uma pasta de pesquisa é criada, o seu aplicativo pode obter atualizados resultados da pesquisa apenas verificando o conteúdo da pasta.
  
Criar uma pasta de pesquisa é simple quando tiver dominado Criando filtros de pesquisa. No exemplo a seguir, uma pasta de pesquisa é criada para mostrar todos os emails com o assunto que contém as "observações de reunião".
  
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

- [Use os filtros de pesquisa com o EWS no Exchange](how-to-use-search-filters-with-ews-in-exchange.md)
    
- [Executar uma pesquisa AQS, usando o EWS no Exchange](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md)
    
- [Realizar pesquisas paginadas utilizando o EWS no Exchange](how-to-perform-paged-searches-by-using-ews-in-exchange.md)
    
- [Realizar pesquisas de agrupadas usando o EWS no Exchange](how-to-perform-grouped-searches-by-using-ews-in-exchange.md)
    
- [Trabalhar com pastas de pesquisa usando o EWS no Exchange](how-to-work-with-search-folders-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>Confira também


- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    
- [Pasta itens recuperáveis](http://technet.microsoft.com/en-us/library/ee364755%28v=exchg.150%29.aspx(Office.15).aspx)
    
- [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [Parâmetros de política de limitação que afetam o EWS operações de pesquisa](ews-throttling-in-exchange.md#bk_ThrottlingSearch)
    

