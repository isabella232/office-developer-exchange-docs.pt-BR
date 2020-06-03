---
title: Executar uma pesquisa do AQS usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: c136901a-313e-4adf-a223-1d090d16917a
description: Descubra como Pesquisar cadeias de caracteres de consulta e AQS em sua API gerenciada do EWS ou aplicativo do EWS.
localization_priority: Priority
ms.openlocfilehash: 9f611a8d90c6baf0f307897735c6366c82bb63c8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455713"
---
# <a name="perform-an-aqs-search-by-using-ews-in-exchange"></a>Executar uma pesquisa do AQS usando o EWS no Exchange

Descubra como Pesquisar cadeias de caracteres de consulta e AQS em sua API gerenciada do EWS ou aplicativo do EWS.
  
As cadeias de caracteres de consulta oferecem uma alternativa aos [filtros de pesquisa](how-to-use-search-filters-with-ews-in-exchange.md) para expressar critérios de pesquisa. A maior vantagem de usar cadeias de caracteres de consulta é que você não precisa especificar uma única propriedade a Pesquisar. Você pode simplesmente fornecer um valor e a pesquisa será aplicada a todos os campos usados com frequência nos itens. Você também pode refinar sua pesquisa usando a sintaxe de consulta avançada (AQS) em vez de um valor simples. No entanto, as cadeias de caracteres de consulta têm as seguintes limitações que você deve estar ciente antes de adicioná-las à caixa de ferramentas: 
  
- **Capacidade limitada de Pesquisar propriedades específicas.** Quando você pesquisa com um valor simples em uma cadeia de caracteres de consulta, a pesquisa é executada em todas as propriedades indexadas. Você pode refinar sua pesquisa a propriedades específicas, mas as propriedades disponíveis para uso em uma cadeia de caracteres AQS são limitadas. Se a propriedade que você deseja Pesquisar não é uma das propriedades que estão disponíveis para o AQS, considere usar um filtro de pesquisa. 
    
- **Propriedades personalizadas não são pesquisadas.** Pesquisas de cadeia de caracteres de consulta são realizadas em um índice e as propriedades personalizadas não são incluídas nesse índice. Se você precisar pesquisar Propriedades personalizadas, use um filtro de pesquisa. 
    
- **Controle limitado para pesquisas de cadeia de caracteres.** Pesquisas de cadeia de caracteres de consulta sempre ignoram maiúsculas e são sempre subcadeias de pesquisa. Se você deseja fazer pesquisas de diferenciação de maiúsculas e minúsculas, prefixo ou correspondência exata, use um filtro de pesquisa. 
    
- **Não disponível para pastas ou pastas de pesquisa.** As operações do EWS para pesquisa de pastas não são compatíveis com o uso de uma cadeia de caracteres de consulta. Além disso, as pastas de pesquisa não dão suporte a sequências de consulta. Em ambos os casos, um filtro de pesquisa é sua única opção. 
    
## <a name="creating-a-query-string"></a>Criar uma cadeia de caracteres de consulta
<a name="bk_CreateQueryString"> </a>

As cadeias de caracteres de consulta na API gerenciada do EWS e no EWS são interpretadas como um subconjunto da sintaxe AQS. As cadeias de caracteres AQS são compostas de valores ou pares de palavra-chave/valor, separados por dois-pontos (:).
  
`keyword:value`

Quando um valor é especificado sem uma palavra-chave, todas as propriedades indexadas são pesquisadas quanto ao valor. Se uma palavra-chave estiver emparelhada com um valor, a palavra-chave especificará uma propriedade para pesquisar o valor correspondente.
  
**Tabela 1. Palavras-chave AQS suportadas**

|**Chaves**|**Value type**|**Exemplo**|
|:-----|:-----|:-----|
|subject  <br/> |String  <br/> |Assunto: projeto  <br/> |
|corpo  <br/> |String  <br/> |corpo: números de vendas  <br/> |
|anexo  <br/> |String  <br/> |Anexo: relatório  <br/> |
|para  <br/> |String  <br/> |para: "Sadie Daniels"  <br/> |
|from  <br/> |String  <br/> |de: Espero  <br/> |
|cc  <br/> |String  <br/> |CC: "Ronnie Sturgis"  <br/> |
|bcc  <br/> |String  <br/> |CCO: Mack  <br/> |
|participants  <br/> |String  <br/> |participantes: Sadie  <br/> |
|category  <br/> |String  <br/> |Categoria: projeto  <br/> |
|importance  <br/> |String  <br/> |prioridade: alta  <br/> |
|Tipo  <br/> |Tipo de item  <br/> |tipo: reuniões  <br/> |
|enviado  <br/> |Data  <br/> |enviado: 12/10/2013  <br/> |
|recebido  <br/> |Data  <br/> |recebido: ontem  <br/> |
|HasAttachment  <br/> |Booliano  <br/> |Tem anexo: true  <br/> |
|issinalizado  <br/> |Booliano  <br/> |issinalizado: true  <br/> |
|IsRead  <br/> |Booliano  <br/> |IsRead: false  <br/> |
|size  <br/> |Número  <br/> |Tamanho: \> 5000  <br/> |
   
Vamos dar uma olhada em como os diferentes tipos de valor funcionam.
  
### <a name="using-a-string-value-type"></a>Usando um tipo de valor de cadeia de caracteres

Os tipos de valores de cadeia de caracteres são, por padrão, pesquisados como prefixo as pesquisas que não diferenciam maiúsculas de minúsculas. Isso significa que a pesquisa por assunto: Project corresponderia a qualquer um dos seguintes assuntos: 
  
- Notas da reunião do projeto
    
- Você tem os planos do projeto?
    
- Projeções de vendas de dezembro
    
Você pode alterar a pesquisa para exigir a palavra inteira em vez de coincidir prefixos, colocando a cadeia de caracteres entre aspas. Pesquisando o assunto: "projeto" eliminaria o valor "projeções de vendas de dezembro" da lista de correspondências. Observe que o valor ainda não diferencia maiúsculas de minúsculas. 
  
Se você usar várias palavras em uma cadeia de caracteres de consulta, uma correspondência exigirá que ambas as palavras apareçam nos campos pesquisados. Por exemplo, a pesquisa por assunto: o plano de projeto corresponderia a qualquer um dos seguintes assuntos: 
  
- Plano de projeto
    
- Você tem os planos do projeto?
    
- Envie-me o plano para o nosso projeto
    
- Planejar Marcos de projeto
    
Se você incluir várias palavras entre aspas, elas serão tratadas como uma única frase. Pesquisando o assunto: "plano de projeto" só corresponderia ao assunto "plano do projeto" da lista anterior. 
  
### <a name="using-an-item-type-value-type"></a>Usando um tipo de valor de tipo de item

Você pode usar os seguintes valores de tipo de item com a palavra-chave **Kind** para limitar os resultados da pesquisa a apenas um tipo específico de item, como email ou solicitações de reunião: 
  
- contacts    
- docs    
- email    
- fax    
- im (corresponde a mensagens instantâneas)    
- diários    
- reuniões (corresponde a compromissos e solicitações de reunião)    
- notes    
- postagens    
- rssfeeds    
- tarefas    
- postal
    
### <a name="using-a-date-value-type"></a>Usando um tipo de valor de data

Você pode Pesquisar tipos de valor de data de várias maneiras diferentes. O mais simples é Pesquisar uma data específica. Pesquisa com recebido: 12/11/2013 retornará todos os itens recebidos em 11 de dezembro de 2013. No entanto, você também pode ser menos específico. Pesquisa com recebido: 12/11 retornará todos os itens recebidos em 11 de dezembro do ano atual. 
  
Outra opção é usar os nomes dos meses. Você pode pesquisar com recebido: 11 de dezembro de 2013 ou dezembro 11 para obter os mesmos resultados recebidos: 12/11/2013 e recebidos: 12/11, respectivamente. Você também pode pesquisar com recebido: dezembro para obter todos os itens recebidos no mês de dezembro, no ano atual. 
  
O uso dos nomes dos dias da semana também é uma opção. Pesquisa com recebido: terça-feira retornará todos os itens recebidos na terça-feira da semana atual. 
  
Os tipos de valores de data também oferecem suporte a um conjunto de palavras-chave para pesquisas em relação à hora atual. Há suporte para as seguintes palavras-chave:
  
- hoje  
- tomorrow
- ontem
- esta semana    
- A semana passada    
- próximo mês    
- mês passado    
- próximo ano
    
Os tipos de valor de data também podem ser comparados com operadores relacionais, como maior ou menor que, ou especificados como um intervalo com o operador de intervalo **..**. Por exemplo, recebido: \> 11/30/2013, enviado: \> = ontem e recebido: 12/1/2013.. hoje são todas as cadeias de caracteres de consulta válidas. 
  
### <a name="using-a-boolean-value-type"></a>Usando um tipo de valor Boolean

Os tipos de valor Boolean podem ser "true" ou "false". Os valores não diferenciam maiúsculas de minúsculas, portanto, IsRead: false produzirá os mesmos resultados que IsRead: FALSE.
  
### <a name="using-a-number-value-type"></a>Usando um tipo de valor de número

Os tipos de valor numérico podem ser pesquisados como correspondências exatas, mas também podem ser pesquisados usando operadores relacionais, como maior ou menor que. Por exemplo, tamanho: 10000 retornará apenas os itens que têm um tamanho de exatamente 10000 bytes, mas tamanho: \> = 10000 retornará itens com um tamanho maior ou igual a 10000 bytes. Você também pode especificar um intervalo usando o operador de intervalo ( **..**). Por exemplo, tamanho: 7000.. 8000 retornará itens que têm um tamanho entre 7000 e 8000. 
  
### <a name="using-logical-operators"></a>Usando operadores lógicos

As cadeias de caracteres de consulta dão suporte aos seguintes operadores lógicos.
  
**Tabela 2. Operadores lógicos suportados**

|**Operator**|**Exemplos**|
|:-----|:-----|
|E  <br/> |Project e de: "Sadie Daniels"  <br/> Assunto: (projeto e plano)  <br/> |
|OU  <br/> |Assunto: reunião ou de: "Espero bruto"  <br/> de:("Sadie Daniels" ou "esperança bruto")  <br/> |
|NÃO  <br/> |Não de: "Ronnie Sturgis"  <br/> recebido: não hoje  <br/> |
   
Observe que você pode usar esses operadores para participar de vários critérios juntos ou para unir vários valores em um único par de palavra-chave/valor juntos. No entanto, ao unir vários valores em um único par de palavra-chave/valor, você deve usar parênteses para incluir os vários valores. Para entender por que, considere Pesquisar de: "Sadie Daniels" ou "esperança bruto". Na verdade, essa pesquisa é interpretada como o seguinte critério:
  
- O item é de Sadie Daniels ou
    
- O item tem a frase "Espero bruto" em qualquer uma das propriedades indexadas.
    
Por outro lado, de:("Sadie Daniels" ou "Espero bruto") é interpretado como: 
  
- O item é de Sadie Daniels ou
    
- O item é de esperança bruto
    
O operador padrão quando vários critérios são especificados, mas nenhum operador lógico está incluído é e. Por exemplo, tem anexo: verdadeiro assunto: o projeto é equivalente a: Attachment: true e subject: Project.
  
## <a name="example-find-items-by-using-a-query-string-and-the-ews-managed-api"></a>Exemplo: localizar itens usando uma cadeia de caracteres de consulta e a API gerenciada do EWS
<a name="bk_ExampleEWSMA"> </a>

Neste exemplo, um método chamado **SearchWithQueryString** é definido. Ele usa um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , um objeto [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) e um objeto **String** que representa a cadeia de caracteres de consulta como parâmetros. Este exemplo pressupõe que o objeto **ExchangeService** tenha sido inicializado com valores válidos nas propriedades de [credenciais](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) e [URL](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) . 
  
```cs
using Microsoft.Exchange.WebServices.Data;
static void SearchWithQueryString(ExchangeService service, WellKnownFolderName folder, string queryString)
{
    // Limit the result set to 10 items.
    ItemView view = new ItemView(10);
    view.PropertySet = new PropertySet(ItemSchema.Subject,
                                       ItemSchema.DateTimeReceived,
                                       ItemSchema.Size,
                                       ItemSchema.Importance,
                                       EmailMessageSchema.IsRead);
    // Item searches do not support Deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Sorting
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    try
    {
        // Execute the search based on the query string.
        // Example: "subject:project plan"
        FindItemsResults<Item> results = service.FindItems(folder, queryString, view);
        foreach (Item item in results.Items)
        {
            Console.WriteLine("Subject: {0}", item.Subject);
            Console.WriteLine("Received: {0}", item.DateTimeReceived.ToString());
            Console.WriteLine("Size: {0}", item.Size.ToString());
            Console.WriteLine("Importance: {0}", item.Importance.ToString());
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

Você pode usar esse método para pesquisar todos os itens com a frase "plano de projeto" no assunto, conforme mostrado neste exemplo.
  
```cs
string queryString = "subject:\"project plan\"";
SearchWithQueryString(service, WellKnownFolderName.Inbox, queryString);
```

## <a name="example-find-items-by-using-a-query-string-and-ews"></a>Exemplo: localizar itens usando uma cadeia de caracteres de consulta e EWS
<a name="bk_ExampleEWS"> </a>

Neste exemplo, uma solicitação SOAP [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) localiza todos os itens na caixa de entrada com a frase "plano do projeto" no assunto. 
  
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
          <t:FieldURI FieldURI="item:Size" />
          <t:FieldURI FieldURI="item:Importance" />
          <t:FieldURI FieldURI="message:IsRead" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="10" Offset="0" BasePoint="Beginning" />
      <m:SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:FieldOrder>
      </m:SortOrder>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
      <m:QueryString>subject:"project plan"</m:QueryString>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

O exemplo a seguir mostra a resposta do servidor com os resultados da pesquisa.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1" TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>project plan</t:Subject>
                <t:DateTimeReceived>2013-12-11T15:42:02Z</t:DateTimeReceived>
                <t:Size>7406</t:Size>
                <t:Importance>Normal</t:Importance>
                <t:IsRead>false</t:IsRead>
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
- [Usar filtros de pesquisa com o EWS no Exchange](how-to-use-search-filters-with-ews-in-exchange.md)    
- [ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [Operação FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

