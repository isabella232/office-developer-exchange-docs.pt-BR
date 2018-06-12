---
title: Realizar pesquisas paginadas utilizando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 64ed70e4-32eb-4c25-bfc4-43d1477296e5
description: Descubra como realizar pesquisas paginadas em sua API gerenciada de EWS ou aplicativos do EWS que tem como destino o Exchange.
ms.openlocfilehash: 3f82f46d0582b0b7ff8be63de8a7054b5f3cacab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750806"
---
# <a name="perform-paged-searches-by-using-ews-in-exchange"></a>Realizar pesquisas paginadas utilizando o EWS no Exchange

Descubra como realizar pesquisas paginadas em sua API gerenciada de EWS ou aplicativos do EWS que tem como destino o Exchange.
  
Paginação é um recurso do EWS que permite controlar o tamanho dos resultados de uma pesquisa. Em vez de recuperar o conjunto em uma resposta EWS de resultados inteiro, é possível recuperar conjuntos menores em várias respostas do EWS. Por exemplo, considere um usuário com 10.000 mensagens de email na sua caixa de entrada. Hipoteticamente, você pode recuperar todos os emails de 10.000 em uma resposta muito grande, mas talvez você queira que divida em partes mais gerenciáveis por motivos de desempenho ou a largura de banda. Paginação oferece as ferramentas necessárias para fazer isso.
  
> [!NOTE]
> Hipoteticamente, é possível recuperar 10.000 itens em uma solicitação, na verdade, isso é improvável devido à limitação EWS. Para obter mais informações, consulte a [limitação do EWS no Exchange](ews-throttling-in-exchange.md). 
  
**Tabela 1. Parâmetros de paginação na API gerenciada de EWS e EWS**

|**Para definir ou recuperar o …**|**Na API gerenciada do EWS, use …**|**No EWS, use …**|
|:-----|:-----|:-----|
|Número máximo de itens ou pastas em uma resposta  <br/> |O parâmetro **pageSize** para o [Construtor de ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview.itemview%28v=exchg.80%29.aspx) ou o [Construtor de FolderView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderview.folderview%28v=exchg.80%29.aspx) <br/> Or  <br/> A propriedade [PagedView.PageSize](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pagedview.pagesize%28v=exchg.80%29.aspx)  <br/> |O atributo **MaxEntriesReturned** no elemento [IndexedPageItemView](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) ou o elemento [IndexedPageFolderView](http://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx)  <br/> |
|Ponto de partida na lista de itens ou pastas  <br/> |O parâmetro **offsetBasePoint** para o construtor de **ItemView** ou o construtor de **FolderView**  <br/> Or  <br/> A propriedade [PagedView.OffsetBasePoint](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pagedview.offsetbasepoint%28v=exchg.80%29.aspx)  <br/> |O atributo de **ponto de base** no elemento **IndexedPageItemView** ou o elemento **IndexedPageFolderView**  <br/> |
|Deslocamento a partir do ponto de partida  <br/> |O parâmetro de **deslocamento** para o construtor de **ItemView** ou o construtor de **FolderView**  <br/> Or  <br/> A propriedade [PagedView.Offset](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pagedview.offset%28v=exchg.80%29.aspx)  <br/> |O atributo **deslocamento** no elemento **IndexedPageItemView** ou o elemento **IndexedPageFolderView**  <br/> |
|Número total de resultados no servidor  <br/> |A propriedade [FindItemsResults.TotalCount](http://msdn.microsoft.com/en-us/library/dd635348%28v=exchg.80%29.aspx) ou a propriedade [FindFoldersResults.TotalCount](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.findfoldersresults.totalcount%28v=exchg.80%29.aspx)  <br/> |O atributo **TotalItemsInView** no elemento [RootFolder (FindItemResponseMessage)](http://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) ou o elemento [RootFolder (FindFolderResponseMessage)](http://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx)  <br/> |
|Deslocamento do primeiro item ou pasta não incluído na resposta atual  <br/> |A propriedade [FindItemsResults.NextPageOffset](http://msdn.microsoft.com/en-us/library/ee693014%28v=exchg.80%29.aspx) ou a propriedade [FindFoldersResults.NextPageOffset](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.findfoldersresults.nextpageoffset%28v=exchg.80%29.aspx)  <br/> |O atributo **IndexedPagingOffset** no elemento **RootFolder**  <br/> |
|Indicador que a resposta inclui o último item ou a pasta na lista  <br/> |A propriedade [FindItemsResults.MoreAvailable](http://msdn.microsoft.com/en-us/library/dd635477%28v=exchg.80%29.aspx) ou a propriedade [FindFoldersResults.MoreAvailable](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.findfoldersresults.moreavailable%28v=exchg.80%29.aspx)  <br/> |O atributo **IncludesLastItemInRange** no elemento **RootFolder**  <br/> |
   
## <a name="how-paging-works"></a>Como funciona a paginação
<a name="bk_HowPagingWorks"> </a>

Para entender como funciona a paginação, é útil visualizar as mensagens em uma pasta como cartazes alinhados lado a lado em um campo fora de sua casa. Você pode ver alguns desses cartazes é através de uma janela de mágica. Você tem a capacidade de alterar o tamanho da janela (para ver cartazes é mais ou menos de uma vez) e para mover a janela (para controlar quais cartazes, você pode ver). Este manipulação da janela é paginação. 
  
Quando você enviar sua solicitação para o Exchange server, você pode especificar o tamanho da sua janela em termos de quantos itens para retornar. Você pode definir a posição da janela, especificando um ponto de partida um (o início da linha) ou o final da linha e um deslocamento a partir desse ponto inicial, expressado em um número de itens. O início da janela é o número de itens especificada pelo deslocamento, desde o ponto de partida.
  
Onde paginação obtém um pouco mais interessante está na resposta do servidor, e como o seu aplicativo pode usar essa resposta para sua próxima solicitação de forma. O servidor fornece três partes de informações que você pode usar para determinar como configurar seu "janela" para sua próxima solicitação: 
  
- Se os resultados na resposta incluir o último item geral conjunto de resultados no servidor.
    
- O número total de itens no resultado definido no servidor.
    
- O que o valor de deslocamento próximo deve ser, se você deseja avançar sua janela para o próximo item no conjunto de resultados que não esteja incluído na resposta atual.
    
Vamos ver um exemplo simples. Imagine uma caixa de entrada com 15 mensagens dela. Seu aplicativo envia uma solicitação inicial para recuperar um máximo de 10 itens, desde o início da lista de mensagens (para que o deslocamento for zero). O servidor responde com as mensagens de 10 primeiros e indica que a resposta não incluir o último item, que não há um total de 15 itens e que o próximo deslocamento deve ser 10.
  
**Figura 1. Solicitando 10 itens em deslocamento 0 desde o início de uma lista de 15 itens**

![A diagram showing the results of requesting 10 items at offset 0 from the beginning of a list of 15 items.](media/Ex15_PagedSearch_FirstPage.png)
  
Seu aplicativo, em seguida, reenvia a mesma solicitação ao servidor, com a única alteração de que o deslocamento agora é 10. O servidor retorna os últimos cinco itens e indica que a resposta incluir o último item, que não há um total de 15 itens e que o próximo deslocamento deve ser 15 (embora obviamente, você chegou final, portanto, não haverá um deslocamento próximo.)
  
**Figura 2. Solicitando 10 itens em deslocamento 10 desde o início de uma lista de 15 itens**

![A diagram showing the results of requesting 10 items at offset 10 from the beginning of a list of 15 items.](media/Ex15_PagedSearch_SecondPage.png)
  
## <a name="design-considerations-for-paging"></a>Considerações de design para paginação
<a name="bk_DesignConsiderations"> </a>

Tornar o máximo da paginação em seu aplicativo requerem alguns consideração. Por exemplo, como grandes ter sua janela""? O que fazer se os resultados no servidor alterar enquanto você estiver movendo sua janela""?
  
### <a name="determine-the-size-of-your-window"></a>Determinar o tamanho da sua janela

Não há nenhum "única" número máximo de entradas que todos os aplicativos devem usar. Determinando o número correto para seu aplicativo depende de vários fatores diferentes. No entanto, é útil ter as seguintes diretrizes em mente:
  
- Por padrão, o Exchange limita o número máximo de itens que podem ser retornadas em uma única solicitação a 1000.
    
- Definindo o número máximo de entradas para um maior resulta de número em precisar enviar solicitações menos para obter todos os itens ao custo da necessidade de aguardar mais respostas.
    
- Definindo o número máximo de entradas para um menor número os resultados nos tempos de resposta mais rápidos, ao custo de enviar mais solicitações para obter todos os itens.
    
### <a name="handling-changes-to-the-result-set"></a>Tratamento de alterações ao conjunto de resultados

No exemplo simple neste artigo, o número de itens na caixa de entrada do usuário permaneceu constante. No entanto, na realidade, o número de itens em uma caixa de entrada pode alterar com frequência. Novas mensagens podem chegar e itens podem ser excluídos ou movidos a qualquer momento. Mas como funciona a paginação este impacto? Vamos modificar o cenário de exemplo anterior para descobrir.
  
Começaremos novamente com os 15 itens na caixa de entrada do usuário e enviar a solicitação inicial mesma. Como antes, o servidor responde com as mensagens de 10 primeiros e indica que a resposta não incluir o último item, que não há um total de 15 itens e que o próximo deslocamento deve ser 10, conforme mostrado na Figura 1.
  
Agora, enquanto o seu aplicativo está processando esses 10 itens, uma nova mensagem chega na caixa de entrada e é adicionada ao resultado definido no servidor. Seu aplicativo reenvia a mesma solicitação ao servidor (somente com o deslocamento definido como 10). Neste momento o servidor obtém volta seis itens e indica que há um total de 16 itens no conjunto de resultados.
  
Nesse momento você deve estar se perguntando se isso ainda é um problema. Afinal, você obteve 16 itens novamente sobre as duas respostas, então, por que tudo isso? A resposta depende de onde colocado o novo item na lista. Se a lista é classificada para que os itens mais antigos (por data/hora recebido) sejam primeiro, não há nenhum motivo de preocupação neste cenário. O novo item será colocado no final da lista e será incluído na segunda resposta.
  
**Figura 3. Solicitando 10 itens em deslocamento 10 desde o início de uma lista de itens de 16, com o item 16 na lista sendo novo**

![A diagram showing the results of requesting 10 items at offset 10 from the beginning of a list of 16 items when the 16th item was added to the end of the list.](media/Ex15_PagedSearch_SecondPage_NewItemEnd.png)
  
Se a lista é classificada para que os itens mais novos são primeiro, é uma história diferente. Nesse caso, o primeiro item na segunda solicitação seria o último item da solicitação anterior plus os cinco itens restantes de 15 a original. Para colocar em termos de nossa janela mágica imaginária, você deslocados posição da sua janela em 10, mas os cartazes sozinhos também deslocadas por 1.
  
**Figura 4. Solicitando 10 itens em deslocamento 10 desde o início de uma lista de itens de 16, com o primeiro item na lista que está sendo novo**

![A diagram showing the results of asking for 10 items at offset 10 from the beginning of a list of 16 items when the 16th item was added to the beginning of the list.](media/Ex15_PagedSearch_SecondPage_NewItemBeginning.png)
  
Uma maneira para detectar uma alteração para os resultados no servidor é usar o conceito de um item de âncora. Um item de âncora é um item adicional em sua resposta que não é processado com o restante dos resultados, mas é usada para comparação com os próximos resultados para ver se alteraram próprios itens. Criando novamente no nosso exemplo simple, se o seu aplicativo está usando um tamanho de "janela" 10, realmente definir o número máximo de itens para retornar à 11. Seu aplicativo processa os 10 primeiros itens na resposta como de costume. Para o último item, você salvar o identificador do item como âncora e emita a próxima solicitação com um deslocamento de 10. Se os dados não tem sido alterado, o primeiro item na segunda resposta deve ter um identificador de item que corresponda à âncora. Se os identificadores de item não coincidirem, você saberá que os dados foi removidos ou inseridos na lista partes da lista de você ter já "paginados" sobre.
  
Mesmo quando você souber que os dados foram alterados, você ainda precisará decidir como reagir. Há não uma única resposta para essa pergunta. Suas ações dependerá da natureza do seu aplicativo e como é essencial capturar todos os itens. Você pode ignorá-la completamente, reinicie o processo desde o início, ou fazer track e tente detectar onde a alteração aconteceu.
  
## <a name="example-perform-a-paged-search-by-using-the-ews-managed-api"></a>Exemplo: Executar uma pesquisa paginada usando a API gerenciada de EWS
<a name="bk_PagedSearchEWSMA"> </a>

Paginação é suportada pelos seguintes métodos API gerenciada de EWS:
  
- [ExchangeService.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
Se você estiver usando a API gerenciada de EWS, seu aplicativo configura paginação com a classe [ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) ou [FolderView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) e recebe informações do servidor referente a paginação do [FindItemsResults](http://msdn.microsoft.com/en-us/library/dd635381%28v=exchg.80%29.aspx) ou [FindFoldersResults](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.findfoldersresults%28v=exchg.80%29.aspx) classe. 
  
O exemplo a seguir recupera todos os itens em uma pasta usando uma pesquisa paginada que retorne cinco itens em cada resposta. Ele também recupera um item adicional para servir como uma âncora para detectar alterações aos resultados no servidor. 
  
Este exemplo pressupõe que o objeto **ExchangeService** foi inicializado com valores válidos nas propriedades [credenciais](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) e [Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) . 
  
```cs
using Microsoft.Exchange.WebServices.Data;
static void PageSearchItems(ExchangeService service, WellKnownFolderName folder)
{
    int pageSize = 5;
    int offset = 0;
    // Request one more item than your actual pageSize.
    // This will be used to detect a change to the result
    // set while paging.
    ItemView view = new ItemView(pageSize + 1, offset);
    view.PropertySet = new PropertySet(ItemSchema.Subject);
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    view.Traversal = ItemTraversal.Shallow;
    bool moreItems = true;
    ItemId anchorId = null;
    while (moreItems)
    {
        try
        {
            FindItemsResults<Item> results = service.FindItems(folder, view);
            moreItems = results.MoreAvailable;
            if (moreItems &amp;&amp; anchorId != null)
            {
                // Check the first result to make sure it matches
                // the last result (anchor) from the previous page.
                // If it doesn't, that means that something was added
                // or deleted since you started the search.
                if (results.Items.First<Item>().Id != anchorId)
                {
                    Console.WriteLine("The collection has changed while paging. Some results may be missed.");
                }
            }
            if (moreItems)
                view.Offset += pageSize;
            anchorId = results.Items.Last<Item>().Id;
            // Because you're including an additional item on the end of your results
            // as an anchor, you don't want to display it.
            // Set the number to loop as the smaller value between
            // the number of items in the collection and the page size.
            int displayCount = results.Items.Count > pageSize ? pageSize : results.Items.Count;
            for (int i = 0; i < displayCount; i++)
            {
                Item item = results.Items[i];
                Console.WriteLine("Subject: {0}", item.Subject);
                Console.WriteLine("Id: {0}\n", item.Id.ToString());
            }
        }
        catch (Exception ex)
        {
            Console.WriteLine("Exception while paging results: {0}", ex.Message);
        }
    }
}
```

## <a name="example-perform-a-paged-search-by-using-ews"></a>Exemplo: Executar uma pesquisa paginada usando o EWS
<a name="bk_PagedSearchEWS"> </a>

Paginação é suportada pelos seguintes operações EWS:
  
- [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
Se você estiver usando o EWS, seu aplicativo configura paginação com o elemento [IndexedPageItemView](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) ou o elemento [IndexedPageFolderView](http://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) e recebe informações do servidor referente a paginação do [(RootFolder FindItemResponseMessage)](http://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) elemento ou o elemento [RootFolder (FindFolderResponseMessage)](http://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx) . 
  
Neste exemplo de solicitação, uma solicitação de **FindItem** é enviada para um máximo de seis itens, começando em um deslocamento de zero desde o início da lista de itens na caixa de entrada do usuário. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="6" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

O servidor retorna a seguinte resposta, que contém seis itens. A resposta também indica que não há um total de oito itens nos resultados no servidor e que o último item na lista de resultados não está presente nesta resposta.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="35" Version="V2_4" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="6" TotalItemsInView="8" IncludesLastItemInRange="false">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Query</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Update</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Planning resources</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Timeline</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>For your perusal</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>meeting notes</t:Subject>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

Neste exemplo, a mesma solicitação é enviada, mas desta vez, o atributo de **deslocamento** é alterado para cinco, que indica que o servidor deve retornar no máximo seis itens, começando com offset cinco desde o início. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="6" Offset="5" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

O servidor envia a seguinte resposta, que contém três itens. A resposta também indica que o número total de itens nos resultados no servidor ainda oito e que o último item nos resultados da lista está incluída nesta resposta.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="35" Version="V2_4" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="8" TotalItemsInView="8" IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>meeting notes</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Meeting notes</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>This cat is hilarious!</t:Subject>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a>Confira também


- [Pesquisa e EWS no Exchange](search-and-ews-in-exchange.md)
    
- [Método ExchangeService.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [Método ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [Método Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [Método Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
- [Operação FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [Operação FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
- [EWS limitação no Exchange](ews-throttling-in-exchange.md)
    

