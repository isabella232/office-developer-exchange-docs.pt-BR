---
title: Executar uma pesquisa AQS, usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: c136901a-313e-4adf-a223-1d090d16917a
description: Descubra como pesquisar com cadeias de caracteres de consulta e AQS na sua API gerenciada de EWS ou aplicativos do EWS.
ms.openlocfilehash: dc859e24fa80cd5627477182979c9cc9527818d6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750823"
---
# <a name="perform-an-aqs-search-by-using-ews-in-exchange"></a>Executar uma pesquisa AQS, usando o EWS no Exchange

Descubra como pesquisar com cadeias de caracteres de consulta e AQS na sua API gerenciada de EWS ou aplicativos do EWS.
  
Cadeias de caracteres de consulta fornecem uma alternativa para [filtros de pesquisa](how-to-use-search-filters-with-ews-in-exchange.md) para expressar critérios de pesquisa. A maior vantagem ao uso de cadeias de caracteres de consulta é que não são necessários para especificar uma única propriedade a ser pesquisado. Você pode simplesmente fornecer um valor e a pesquisa se aplicará a todos os campos comumente usados nos itens. Você também pode refinar sua pesquisa usando a sintaxe de consulta avançada (AQS) em vez de um valor simple. No entanto, as cadeias de caracteres de consulta têm as seguintes limitações que você deve estar ciente antes de adicioná-los à sua caixa de ferramentas: 
  
- **Capacidade limitada de propriedades específicas de pesquisa.** Quando você pesquisa com um valor simple em uma cadeia de caracteres de consulta, a pesquisa é executada em relação a todas as propriedades indexadas. Você pode refinar a pesquisa às propriedades específicas, mas as propriedades disponíveis para serem usados em uma cadeia de caracteres AQS são limitadas. Se a propriedade que você deseja pesquisar não for uma das propriedades disponíveis para AQS, considere o uso de um filtro de pesquisa. 
    
- **Propriedades personalizadas não são pesquisadas.** As pesquisas de cadeia de caracteres de consulta são executadas em relação a um índice e propriedades personalizadas não são incluídas no índice. Se você precisar propriedades personalizadas de pesquisa, use um filtro de pesquisa. 
    
- **Controle limitado cadeia de caracteres de pesquisa.** As pesquisas de cadeia de caracteres de consulta sempre Ignorar maiusculas e minúsculas e são sempre pesquisas de subsequência. Se você deseja fazer diferencia maiusculas de minúsculas, o prefixo ou pesquisas de correspondência exata, usam um filtro de pesquisa. 
    
- **Não disponível para pastas ou pastas de pesquisa.** As operações de EWS para a procura de pastas não suportam o uso uma cadeia de caracteres de consulta. Além disso, as pastas de pesquisa não oferecem suporte a cadeias de caracteres de consulta. Em ambos os casos, um filtro de pesquisa é a única opção. 
    
## <a name="creating-a-query-string"></a>Criando uma cadeia de caracteres de consulta
<a name="bk_CreateQueryString"> </a>

Cadeias de caracteres de consulta na API gerenciada de EWS e EWS são interpretadas como um subconjunto da sintaxe AQS. Cadeias de caracteres AQS são compostas de valores ou pares de palavra-chave/valor, separados por dois pontos (:).
  
`keyword:value`

Quando um valor for especificado, sem uma palavra-chave, todas as propriedades indexadas são pesquisadas para o valor. Se uma palavra-chave é emparelhada com um valor, a palavra-chave especifica uma propriedade para procurar o valor correspondente.
  
**Tabela 1. Palavras-chave AQS com suporte**

|**Palavra-chave**|**Value type**|**Exemplo**|
|:-----|:-----|:-----|
|subject  <br/> |String  <br/> |Assunto: project  <br/> |
|body  <br/> |String  <br/> |ilustrações de sales de corpo:  <br/> |
|anexo  <br/> |String  <br/> |anexo: relatório  <br/> |
|para  <br/> |String  <br/> |para: "Sadie Daniels"  <br/> |
|from  <br/> |String  <br/> |de:, esperamos  <br/> |
|cc  <br/> |String  <br/> |cc: "Ronnie Sturgis"  <br/> |
|bcc  <br/> |String  <br/> |BCC:mack  <br/> |
|participantes  <br/> |String  <br/> |participantes: sadie  <br/> |
|Ferramentas para desenvolvedores  <br/> |Cadeia de caracteres  <br/> |projeto de categoria:  <br/> |
|importance  <br/> |String  <br/> |importância: alta  <br/> |
|tipo  <br/> |Tipo de item  <br/> |reuniões do tipo:  <br/> |
|enviado  <br/> |Data  <br/> |enviados: 12/10/2013  <br/> |
|recebido  <br/> |Data  <br/> |recebidos: ontem  <br/> |
|hasattachment  <br/> |Booliano  <br/> |Tem anexo: true  <br/> |
|está sinalizado  <br/> |Booliano  <br/> |isflagged:True  <br/> |
|foi lido  <br/> |Booliano  <br/> |isread:False  <br/> |
|size  <br/> |Número  <br/> |Tamanho:\>5000  <br/> |
   
Vamos dar uma olhada em como os tipos de valores diferentes funcionam.
  
### <a name="using-a-string-value-type"></a>Usando um tipo de valor de cadeia de caracteres

Tipos de valores de cadeia de caracteres são por padrão pesquisada como pesquisas de subcadeia de caracteres de prefixo que não diferenciam maiusculas de minúsculas. Isso significa que procurando por assunto: project encontraria como correspondente qualquer um dos seguintes assuntos: 
  
- Notas de reunião de projeto
    
- Você tem os planos de projeto?
    
- Projeções de vendas de dezembro
    
Você pode alterar a pesquisa para exigir a palavra inteira em vez de prefixos correspondentes colocando-se a cadeia de caracteres entre aspas. Procurando por assunto: "projeto" seria eliminar o valor de "Projeções de vendas de dezembro" da lista de correspondências. Observe que o valor é ainda não diferencia maiusculas de minúsculas. 
  
Se você usar várias palavras em uma cadeia de caracteres de consulta, uma correspondência requer que ambas as palavras aparecem nos campos pesquisados. Por exemplo, procurando o plano de projeto de assunto: encontraria como correspondente qualquer um dos seguintes assuntos: 
  
- Plano de projeto
    
- Você tem os planos de projeto?
    
- Oriente-me o plano para nosso projeto
    
- Planejando as etapas do projeto
    
Se você colocar várias palavras entre aspas, eles são tratados como uma única frase. Procurando por assunto: "plano de projeto" encontraria como correspondente apenas o assunto "Plano de projeto" da lista anterior. 
  
### <a name="using-an-item-type-value-type"></a>Usando um tipo de valor de tipo de item

Você pode usar os seguintes valores de tipo de item com a palavra-chave de **tipo** para limitar os resultados de pesquisa a apenas um tipo específico de item, como email ou solicitações de reunião: 
  
- contatos    
- documentos    
- email    
- aparelhos de fax    
- IM (corresponde a mensagens instantâneas)    
- diários    
- reuniões (corresponde à compromissos e solicitações de reunião)    
- Observações    
- postagens    
- rssfeeds    
- tarefas    
- caixa postal
    
### <a name="using-a-date-value-type"></a>Usando um tipo de valor de data

Você pode pesquisar os tipos de valores de data em um número de formas diferentes. É o mais simples para procurar uma data específica. Pesquisando com recebidos: 12/11/2013 retornará todos os itens recebidos em 11 de dezembro de 2013. No entanto, você também pode ser menos específico. Pesquisando com recebidos: 12/11 retornará todos os itens recebidos em 11 de dezembro do ano atual. 
  
Outra opção é usar os nomes dos meses. Você pode pesquisar com recebidos: 11 de dezembro de 2013 ou em 11 de dezembro para obter os mesmos resultados como recebido: 12/11/2013 e recebidos: 12/11, respectivamente. Você também pode pesquisar com recebidos: dezembro para obter todos os itens recebidos no mês de dezembro, no ano atual. 
  
Também é uma opção usando os nomes dos dias da semana. Pesquisando com recebidos: terça-feira retornará todos os itens recebidos na terça-feira da semana atual. 
  
Tipos de valores de data também suportam um conjunto de palavras-chave para pesquisas em relação a hora atual. Há suporte para as seguintes palavras-chave:
  
- hoje  
- tomorrow
- ontem
- esta semana    
- A semana passada    
- próximo mês    
- mês passado    
- próximo ano
    
Tipos de valores de data também podem ser comparados com os operadores relacionais como maior ou menor que, ou especificado como um intervalo com o operador de intervalo **.**. Por exemplo, recebido:\>30/11/2013, enviados:\>= ontem, e received:12/1/2013..today são todas as cadeias de caracteres de consulta válido. 
  
### <a name="using-a-boolean-value-type"></a>Usando um tipo de valor booleano

Tipos de valor booleano podem ser "verdadeiro" ou "falso". Os valores não diferenciam maiusculas de minúsculas, portanto isread:false produzirá os mesmos resultados que isread:FALSE.
  
### <a name="using-a-number-value-type"></a>Usando um tipo de valor de número

Tipos de valor de número podem ser pesquisados como correspondências exatas, mas eles também podem ser pesquisados usando operadores relacionais como maior ou menor que. Por exemplo, tamanho: 10000 retornará apenas os itens que tenham um tamanho de exatamente 10000 bytes, mas tamanho:\>= 10000 retornará os itens que tenham um tamanho maior ou igual a 10000 bytes. Você também pode especificar um intervalo usando o operador de intervalo ( **.**). Por exemplo, tamanho: 7000..8000 retornará os itens que tenham um tamanho entre 7000 e 8000. 
  
### <a name="using-logical-operators"></a>Usando operadores lógicos

Cadeias de caracteres de consulta suportam os seguintes operadores lógicos.
  
**Tabela 2. Suporte para os operadores lógicos**

|**Operador**|**Exemplos**|
|:-----|:-----|
|E  <br/> |projeto e de: "Sadie Daniels"  <br/> Assunto:(project AND plan)  <br/> |
|OU  <br/> |Assunto: reunião ou de: "Espero bruta"  <br/> de: ("Sadie Daniels" ou "Valor bruto, esperamos")  <br/> |
|NÃO  <br/> |NÃO de: "Ronnie Sturgis"  <br/> recebidos: não hoje  <br/> |
   
Observe que você pode usar esses operadores para unir vários critérios ou unir vários valores dentro de um par de palavra-chave/valor único. No entanto, ao unir vários valores em um par de palavra-chave/valor único, você deve usar parênteses para delimitar vários valores. Para entender o porquê, considere a pesquisa com a partir de: "Sadie Daniels" ou "Espero bruto". Na verdade, essa pesquisa será interpretada como os seguintes critérios:
  
- O item é de Sadie Daniels, OR
    
- O item tem a frase "Espero bruta" em qualquer uma das suas propriedades indexadas.
    
Por outro lado, a partir: ("Sadie Daniels" ou "Espero bruta") será interpretada como: 
  
- O item é de Sadie Daniels, OR
    
- O item é de espero bruta
    
O operador padrão quando vários critérios são especificados, mas nenhum operador lógico é incluído é and. Por exemplo, tem anexo: true assunto: project é equivalente à tem: anexo: true e assunto: project.
  
## <a name="example-find-items-by-using-a-query-string-and-the-ews-managed-api"></a>Exemplo: Localizar itens usando uma cadeia de caracteres de consulta e a API gerenciada de EWS
<a name="bk_ExampleEWSMA"> </a>

Neste exemplo, um método chamado **SearchWithQueryString** é definido. Que leva a um objeto [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , um objeto [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) e um objeto de **cadeia de caracteres** que representa a cadeia de caracteres de consulta como parâmetros. Este exemplo pressupõe que o objeto **ExchangeService** foi inicializado com valores válidos nas propriedades [credenciais](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) e [Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) . 
  
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

Você pode usar esse método para procurar todos os itens com a frase "plano de projeto" no assunto, conforme mostrado neste exemplo.
  
```cs
string queryString = "subject:\"project plan\"";
SearchWithQueryString(service, WellKnownFolderName.Inbox, queryString);
```

## <a name="example-find-items-by-using-a-query-string-and-ews"></a>Exemplo: Localizar itens usando uma cadeia de caracteres de consulta e o EWS
<a name="bk_ExampleEWS"> </a>

Neste exemplo, uma solicitação SOAP [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) localiza todos os itens na caixa de entrada com a frase "plano de projeto" no assunto. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

- [Pesquisa e EWS no Exchange](search-and-ews-in-exchange.md)    
- [Use os filtros de pesquisa com o EWS no Exchange](how-to-use-search-filters-with-ews-in-exchange.md)    
- [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [Operação FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

