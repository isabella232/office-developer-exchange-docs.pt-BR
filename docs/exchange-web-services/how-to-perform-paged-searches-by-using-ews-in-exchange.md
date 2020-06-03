---
title: Executar pesquisas paginadas usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 64ed70e4-32eb-4c25-bfc4-43d1477296e5
description: Descubra como realizar pesquisas paginadas em sua API gerenciada do EWS ou aplicativo EWS que tem como alvo o Exchange.
localization_priority: Priority
ms.openlocfilehash: 2b608584918c936f62883b8b444d59c05c5952ff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456821"
---
# <a name="perform-paged-searches-by-using-ews-in-exchange"></a>Executar pesquisas paginadas usando o EWS no Exchange

Descubra como realizar pesquisas paginadas em sua API gerenciada do EWS ou aplicativo EWS que tem como alvo o Exchange.
  
Paginação é um recurso do EWS que permite controlar o tamanho dos resultados de uma pesquisa. Em vez de recuperar todo o conjunto de resultados em uma resposta do EWS, você pode recuperar conjuntos menores em várias respostas do EWS. Por exemplo, considere um usuário com 10.000 mensagens de email na caixa de entrada. De forma hipotética, você pode recuperar todos os emails 10.000 em uma resposta muito grande, mas você pode querer desmembrar isso em partes mais gerenciáveis para fins de largura de banda ou desempenho. A paginação fornece as ferramentas para fazer exatamente isso.
  
> [!NOTE]
> Embora você possa recuperar de fato 10.000 itens em uma única solicitação, na realidade, isso é improvável devido à limitação do EWS. Para saber mais, confira [limitação do EWS no Exchange](ews-throttling-in-exchange.md). 
  
**Tabela 1. Parâmetros de paginação na API gerenciada do EWS e EWS**

|**Para configurar ou recuperar o...**|**Na API gerenciada do EWS, use...**|**Em EWS, use...**|
|:-----|:-----|:-----|
|Número máximo de itens ou pastas em uma resposta  <br/> |O parâmetro **PageSize** para o [Construtor de AllViews](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.itemview%28v=exchg.80%29.aspx) ou o [Construtor folderview](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview.folderview%28v=exchg.80%29.aspx) <br/> Ou  <br/> A propriedade [PagedView. PageSize](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.pagesize%28v=exchg.80%29.aspx)  <br/> |O atributo **MaxEntriesReturned** no elemento [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) ou no elemento [IndexedPageFolderView](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx)  <br/> |
|Ponto de partida na lista de itens ou pastas  <br/> |O parâmetro **offsetBasePoint** para o construtor **AllViews** ou o construtor **folderview**  <br/> Ou  <br/> A propriedade [PagedView. OffsetBasePoint](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offsetbasepoint%28v=exchg.80%29.aspx)  <br/> |O atributo **BasePoint** no elemento **IndexedPageItemView** ou no elemento **IndexedPageFolderView**  <br/> |
|Deslocamento a partir do ponto de partida  <br/> |O parâmetro **offset** para o construtor de **AllViews** ou o construtor **folderview**  <br/> Ou  <br/> A propriedade [PagedView. Offset](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offset%28v=exchg.80%29.aspx)  <br/> |O atributo **offset** no elemento **IndexedPageItemView** ou o elemento **IndexedPageFolderView**  <br/> |
|Número total de resultados no servidor  <br/> |A propriedade [FindItemsResults. TotalCount](https://msdn.microsoft.com/library/dd635348%28v=exchg.80%29.aspx) ou a propriedade [FindFoldersResults. TotalCount](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.totalcount%28v=exchg.80%29.aspx)  <br/> |O atributo **TotalItemsInView** no elemento [RootFolder (FindItemResponseMessage)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) ou no elemento [RootFolder (FindFolderResponseMessage)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx)  <br/> |
|Deslocamento do primeiro item ou pasta não incluído na resposta atual  <br/> |A propriedade [FindItemsResults. NextPageOffset](https://msdn.microsoft.com/library/ee693014%28v=exchg.80%29.aspx) ou a propriedade [FindFoldersResults. NextPageOffset](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.nextpageoffset%28v=exchg.80%29.aspx)  <br/> |O atributo **IndexedPagingOffset** no elemento **RootFolder**  <br/> |
|Indicador de que a resposta inclui o último item ou pasta na lista  <br/> |A propriedade [FindItemsResults. MoreAvailable](https://msdn.microsoft.com/library/dd635477%28v=exchg.80%29.aspx) ou a propriedade [FindFoldersResults. MoreAvailable](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.moreavailable%28v=exchg.80%29.aspx)  <br/> |O atributo **IncludesLastItemInRange** no elemento **RootFolder**  <br/> |
   
## <a name="how-paging-works"></a>Como a paginação funciona
<a name="bk_HowPagingWorks"> </a>

Para entender como a paginação funciona, é útil visualizar as mensagens em uma pasta como os murals alinhados lado a lado em um campo fora da sua casa. Você pode ver algumas dessas mensagems por meio de uma janela do Magical. Você pode alterar o tamanho da janela (para ver mais ou menos mensagens de uma vez) e mover a janela (para controlar quais mensagens você pode ver). Essa manipulação da janela é paginação. 
  
Ao enviar sua solicitação para o servidor do Exchange, você especifica o tamanho da janela em termos de quantos itens serão retornados. Você define a posição da janela especificando um ponto de partida (o início da linha ou o final da linha) e um deslocamento a partir desse ponto inicial, expresso em um número de itens. O início da janela é o número de itens especificados pelo deslocamento a partir do ponto inicial.
  
Onde a paginação fica um pouco mais interessante é na resposta do servidor e como seu aplicativo pode usar essa resposta para forma sua próxima solicitação. O servidor fornece três informações que você pode usar para determinar como configurar sua "janela" para sua próxima solicitação: 
  
- Se os resultados na resposta incluem o último item no conjunto de resultados geral no servidor.
    
- O número total de itens no conjunto de resultados no servidor.
    
- Qual será o próximo valor de deslocamento, se você quiser avançar a janela para o próximo item no conjunto de resultados que não está incluído na resposta atual.
    
Vamos dar uma olhada em um exemplo simples. Imagine uma caixa de entrada com 15 mensagens. O aplicativo envia uma solicitação inicial para recuperar um máximo de 10 itens, começando no início da lista de mensagens (de modo que o deslocamento seja zero). O servidor responde com as 10 primeiras mensagens e indica que a resposta não inclui o último item, que há um total de 15 itens e que o próximo deslocamento deve ser 10.
  
**Figura 1. Solicitar 10 itens no deslocamento 0 do início de uma lista de 15 itens**

![A diagram showing the results of requesting 10 items at offset 0 from the beginning of a list of 15 items.](media/Ex15_PagedSearch_FirstPage.png)
  
Em seguida, o aplicativo reenvia a mesma solicitação para o servidor, com a única alteração que o deslocamento agora é 10. O servidor retorna os últimos cinco itens e indica que a resposta inclui o último item, que há um total de 15 itens e que o próximo deslocamento deve ser 15 (porém, você chegou ao fim, portanto, não haverá um deslocamento próximo).
  
**Figura 2. Solicitar 10 itens no deslocamento 10 do início de uma lista de 15 itens**

![A diagram showing the results of requesting 10 items at offset 10 from the beginning of a list of 15 items.](media/Ex15_PagedSearch_SecondPage.png)
  
## <a name="design-considerations-for-paging"></a>Considerações de design para paginação
<a name="bk_DesignConsiderations"> </a>

Tornar o máximo da paginação em seu aplicativo exige alguma consideração. Por exemplo, qual é o tamanho da "janela"? O que fazer se os resultados no servidor mudarem enquanto você estiver movendo sua "janela"?
  
### <a name="determine-the-size-of-your-window"></a>Determinar o tamanho da janela

Não há um número máximo de entradas de "um tamanho para tudo" que todos os aplicativos devem usar. Determinar o número certo para seu aplicativo depende de vários fatores diferentes. No entanto, é útil manter as seguintes diretrizes em mente:
  
- Por padrão, o Exchange limita o número máximo de itens que podem ser retornados em uma única solicitação para 1000.
    
- Definir o número máximo de entradas para um número maior resulta em ter que enviar menos solicitações para obter todos os itens, ao custo de esperar mais por respostas.
    
- Definir o número máximo de entradas para um número menor resulta em tempos de resposta mais rápidos, ao custo de ter que enviar mais solicitações para obter todos os itens.
    
### <a name="handling-changes-to-the-result-set"></a>Gerenciar alterações no conjunto de resultados

No exemplo simples, anteriormente neste artigo, o número de itens na caixa de entrada do usuário permaneceu constante. No entanto, na realidade, o número de itens em uma caixa de entrada pode ser alterado com frequência. Novas mensagens podem chegar e os itens podem ser excluídos ou movidos a qualquer momento. Mas como isso afeta a paginação? Vamos modificar o cenário de exemplo anterior para descobrir.
  
Vamos começar novamente com os 15 itens na caixa de entrada do usuário e enviar a mesma solicitação inicial. Como antes, o servidor responde com as 10 primeiras mensagens e indica que a resposta não inclui o último item, que há um total de 15 itens e que o próximo deslocamento deve ser 10, conforme mostrado na Figura 1.
  
Agora, enquanto o aplicativo está processando esses 10 itens, uma nova mensagem chega na caixa de entrada e é adicionada ao conjunto de resultados no servidor. O aplicativo reenvia a mesma solicitação para o servidor (somente com o deslocamento definido como 10). Desta vez, o servidor recebe o retorno de seis itens e indica que há um total de 16 itens no conjunto de resultados.
  
Neste ponto, você pode estar se perguntando se isso é um problema. Afinal, você tem 16 itens de volta nas duas respostas, então por que todas as complicações? A resposta depende de onde o novo item é colocado na lista. Se a lista for classificada de forma que os itens mais antigos (por data/hora de recebimento) sejam os primeiros, não há nenhuma causa de preocupação neste cenário. O novo item será colocado no final da lista e será incluído na segunda resposta.
  
**Figura 3. Solicitar 10 itens no deslocamento 10 do início de uma lista de 16 itens, com o 16º item na lista sendo novo**

![A diagram showing the results of requesting 10 items at offset 10 from the beginning of a list of 16 items when the 16th item was added to the end of the list.](media/Ex15_PagedSearch_SecondPage_NewItemEnd.png)
  
Se a lista for classificada de forma que os itens mais recentes sejam primeiro, ele será um texto diferente. Nesse caso, o primeiro item da segunda solicitação seria o último item da solicitação anterior mais os cinco itens restantes do original 15. Para colocá-lo em termos de nossa janela imaginária Magical, você moveu a posição da sua janela por 10, mas os próprios murals também foram deslocados por 1.
  
**Figura 4. Solicitar 10 itens no deslocamento 10 do início de uma lista de 16 itens, com o primeiro item da lista sendo novo**

![A diagram showing the results of asking for 10 items at offset 10 from the beginning of a list of 16 items when the 16th item was added to the beginning of the list.](media/Ex15_PagedSearch_SecondPage_NewItemBeginning.png)
  
Uma maneira de detectar uma alteração nos resultados no servidor é usar o conceito de um item de âncora. Um item de âncora é um item adicional em sua resposta que não é processado junto com o restante dos resultados, mas é usado para comparar com os próximos resultados para ver se os itens em si foram deslocados. Criando novamente em nosso exemplo simples, se o aplicativo estiver usando um tamanho de "janela" de 10, você realmente definirá o número máximo de itens para retornar a 11. Seu aplicativo processa os primeiros 10 itens na resposta como de costume. Para o último item, você salva o identificador do item como uma âncora e, em seguida, emite a próxima solicitação com um deslocamento de 10. Se os dados não tiverem sido alterados, o primeiro item da segunda resposta deverá ter um identificador de item que corresponda à âncora. Se os identificadores de item não forem correspondentes, você saberá que os dados foram removidos ou inseridos nas partes da lista que você já "pausou".
  
Mesmo quando você sabe que os dados foram alterados, ainda precisa decidir como reagir. Não há uma resposta de tamanho único para essa pergunta. Suas ações dependerão da natureza do seu aplicativo e de como é essencial capturar todos os itens. Você pode ignorá-lo, reiniciar o processo do início ou do controle de volta e tentar detectar onde a alteração ocorreu.
  
## <a name="example-perform-a-paged-search-by-using-the-ews-managed-api"></a>Exemplo: executar uma pesquisa paginada usando a API gerenciada do EWS
<a name="bk_PagedSearchEWSMA"> </a>

A paginação é suportada pelos seguintes métodos da API gerenciada do EWS:
  
- [ExchangeService. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [Folder. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [Folder. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
Se você estiver usando a API gerenciada do EWS, seu aplicativo configurará a paginação com o [DefaultView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) ou a classe [folderview](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) e receberá informações do servidor referente à paginação na classe [FindItemsResults](https://msdn.microsoft.com/library/dd635381%28v=exchg.80%29.aspx) ou [FindFoldersResults](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults%28v=exchg.80%29.aspx) . 
  
O exemplo a seguir recupera todos os itens em uma pasta usando uma pesquisa paginada que retorna cinco itens em cada resposta. Ele também recupera um item adicional para servir como uma âncora para detectar alterações nos resultados no servidor. 
  
Este exemplo pressupõe que o objeto **ExchangeService** tenha sido inicializado com valores válidos nas propriedades de [credenciais](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) e [URL](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) . 
  
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

## <a name="example-perform-a-paged-search-by-using-ews"></a>Exemplo: executar uma pesquisa paginada usando o EWS
<a name="bk_PagedSearchEWS"> </a>

A paginação é suportada pelas seguintes operações do EWS:
  
- [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
Se você estiver usando o EWS, o aplicativo configurará a paginação com o elemento [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) ou o elemento [IndexedPageFolderView](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) e receberá informações do servidor em relação à paginação a partir do elemento [RootFolder (FindItemResponseMessage)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) ou do elemento [RootFolder (FindFolderResponseMessage)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx) . 
  
Neste exemplo de solicitação, uma solicitação **FindItem** é enviada para um máximo de seis itens, começando em um deslocamento de zero do início da lista de itens na caixa de entrada do usuário. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

O servidor retorna a seguinte resposta, que contém seis itens. A resposta também indica que há um total de oito itens nos resultados no servidor e que o último item na lista de resultados não está presente nesta resposta.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="35" Version="V2_4" 
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

Neste exemplo, a mesma solicitação é enviada, mas desta vez, o atributo **offset** é alterado para cinco, o que indica que o servidor deve retornar no máximo seis itens começando no deslocamento cinco do início. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

O servidor envia a seguinte resposta, que contém três itens. A resposta também indica que o número total de itens nos resultados no servidor ainda é oito e que o último item na lista de resultados está incluído nesta resposta.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="35" Version="V2_4" 
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


- [Pesquisar e EWS no Exchange](search-and-ews-in-exchange.md)
    
- [Método ExchangeService. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [Método ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [Método Folder. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [Método Folder. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
- [Operação FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [Operação FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
- [Limitação do EWS no Exchange](ews-throttling-in-exchange.md)
    

