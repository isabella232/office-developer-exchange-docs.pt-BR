---
title: Resolver nomes de ambíguos, usando o EWS no Exchange 2013
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1ba21c54-ecd2-4a1e-80d4-0f4171dea84f
description: Saiba como usar a API gerenciada de EWS ou o EWS para resolver nomes de ambíguos obtendo correspondências possíveis do serviços de domínio Active Directory (AD DS) ou uma pasta de contatos na caixa de correio do usuário.
ms.openlocfilehash: 05a88043083a27d2e6d445cd71e5f3919c5a775d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750815"
---
# <a name="resolve-ambiguous-names-by-using-ews-in-exchange-2013"></a>Resolver nomes de ambíguos, usando o EWS no Exchange 2013

Saiba como usar a API gerenciada de EWS ou o EWS para resolver nomes de ambíguos obtendo correspondências possíveis do serviços de domínio Active Directory (AD DS) ou uma pasta de contatos na caixa de correio do usuário.
  
Um usuário em sua organização recebe uma lista de nomes e endereços de escritas à mão para funcionários que participou de uma sessão de treinamento. Eles desejam enviar um email com algumas informações adicionais para pessoas na lista, mas não consegue ler o endereço de email de todos os participantes. Se você deseja resolver esse problema para os usuários em seu aplicativo, EWS pode ajudar. Você pode usar o método de API gerenciada de EWS [ExchangeService.ResolveName](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) ou a operação de EWS [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) para retornar uma lista de correspondências possíveis para uma seleção de texto, como parte de um sobrenome. Os itens retornados podem ser caixas de correio de usuário público, grupos de distribuição e contatos. 
  
Observe que o Exchange salva os endereços de email com tipos de roteamento de prefixados, como smtp ou sip, em uma matriz de valores múltiplos. O método **ResolveName** e a operação de **ResolveNames** realizar uma correspondência parcial com cada valor dessa matriz quando você adiciona o tipo de roteamento no início do nome não resolvido, como "sip: User1". Se você não especificar um tipo de roteamento, o método ou a operação será como smtp padrão, associá-lo a uma propriedade de endereço smtp principal e não a matriz de vários valores de pesquisa. Por exemplo, se você procurar User1 e não incluir o prefixo sip, você não receberá sip:User1@Contoso.com como resultado, mesmo se for uma caixa de correio válida. 
  
Você só pode especificar um nome ambíguo em uma única solicitação. Se você tiver uma lista de nomes ambíguos para resolver, você precisará percorrer a lista e chame o método ou a operação para cada entrada. Os candidatos da pasta de contatos do usuário terão um valor de ID de item de não-nulo, que pode ser usado em uma chamada de método [Contact.Bind](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) ou uma solicitação de operação [GetItem](http://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) para recuperar informações adicionais. Se o candidato é um grupo de distribuição, você pode usar o método de API gerenciada de EWS [ExpandGroup(ItemId)](http://msdn.microsoft.com/en-us/library/office/ee356407%28v=exchg.80%29.aspx) ou a operação de EWS [ExpandDL](http://msdn.microsoft.com/library/affe84a5-ad98-4aba-83f4-8732938b763d%28Office.15%29.aspx) para obter a lista de membros. Se o parâmetro _returnContactDetails_ ou o atributo **ReturnFullContactData** EWS estiver definido como true, entradas do Active Directory retornado por meio de um método **ResolveName** ou **ResolveNames** operação incluirá propriedades adicionais que descrevem o contato. O parâmetro _returnContactDetails_ ou o atributo **ReturnFullContactData** não afeta os dados que são retornados para contatos e grupos de contatos. 
  
## <a name="resolve-ambiguous-names-by-using-ews-managed-api"></a>Resolver nomes de ambíguos usando a API gerenciada de EWS
<a name="bk_EWSMA"> </a>

Você pode usar o método [ResolveName](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) para encontrar os candidatos que correspondam ao nome ambíguo que você passar. Você pode usar sobrecarregados do método **ResolveName** para procurar candidatos de cinco maneiras diferentes. 
  
**Tabela 1. Métodos de ResolveName sobrecarregados**

|**Method**|**Como funciona**|
|:-----|:-----|
|[ResolveName(String)](http://msdn.microsoft.com/en-us/library/dd635548%28v=exchg.80%29.aspx) <br/> |Localiza contatos na pasta de contatos do usuário e a lista de endereços Global (GAL) — nesta ordem. A variável de cadeia de caracteres é o nome ambíguo que você está tentando resolver.  <br/> |
|[ResolveName (cadeia de caracteres, ResolveNameSearchLocation, booleano)](http://msdn.microsoft.com/en-us/library/dd634595%28v=exchg.80%29.aspx) <br/> |Localiza contatos na pasta padrão Contatos e/ou a lista de endereços Global (GAL). O valor de cadeia de caracteres é o nome ambíguo, o local da pesquisa especifica a pasta Contatos e/ou a GAL e o valor booleano indica se é necessário retornar as informações completas de contato.  <br/> |
|[ResolveName (cadeia de caracteres, ResolveNameSearchLocation, booleano, PropertySet)](http://msdn.microsoft.com/en-us/library/hh532803%28v=exchg.80%29.aspx) <br/> |Localiza contatos na pasta padrão Contatos e/ou a lista de endereços Global (GAL). Esse método permite que você defina as propriedades que são retornadas.  <br/> |
|[ResolveName (String, IEnumerable\<FolderId\>, ResolveNameSearchLocation, booleano)](http://msdn.microsoft.com/en-us/library/dd636014%28v=exchg.80%29.aspx) <br/> |Localiza contatos em pastas de contatos especificadas e/ou a lista de endereços Global (GAL). Você pode usar esse método para passar a uma coleção de pastas a serem pesquisadas. Isso permite que você procure em pastas de contatos que não seja a pasta padrão Contatos.  <br/> |
|[ResolveName (String, IEnumerable\<FolderId\>, ResolveNameSearchLocation, Boolean, PropertySet)](http://msdn.microsoft.com/en-us/library/hh532581%28v=exchg.80%29.aspx) <br/> |Localiza contatos na lista de endereços Global (GAL) e/ou em pastas específicas de contato. Esse método permite que você defina as propriedades que são retornadas.  <br/> |
   
Vamos começar com um exemplo simples. O exemplo a seguir mostra como resolver a cadeia de caracteres de texto "dan" e o nome e endereço de email de cada candidato encontrado de saída. Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange. 
  
```cs
// Resolve the ambiguous name "dan".
   NameResolutionCollection resolvedNames = service.ResolveName("dan");
   // Output the list of candidates.
   foreach (NameResolution nameRes in resolvedNames)
   {
      Console.WriteLine("Contact name: " + nameRes.Mailbox.Name);
      Console.WriteLine("Contact e-mail address: " + nameRes.Mailbox.Address);
      Console.WriteLine("Mailbox type: " + nameRes.Mailbox.MailboxType);
   }

```

A resposta retorna um máximo de 100 candidatos, embora possa haver mais de 100 candidatos em potencial. Para determinar se apenas os primeiros 100 candidatos de um número maior de candidatos foram retornados, verifique o valor de [IncludesAllResolutions](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.includesallresolutions%28v=exchg.80%29.aspx) no objeto [NameResolutionCollection](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) . Se o valor for true, não há candidatos não é mais possíveis; Se o valor for false, o método retornado somente os primeiros 100 de um número maior de candidatos possíveis. 
  
Se você trabalha em uma grande organização, é provável que um nome como "dan" retornará o número máximo de 100 candidatos. Para reduzir o número de candidatos retornado, limite onde você pesquisar. O exemplo a seguir usa a enumeração [ResolveNameSearchLocation](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.resolvenamesearchlocation%28v=exchg.80%29.aspx) para especificar onde pesquisar para resolver o nome ambíguo. 
  
```cs
// Resolve the ambiguous name "dan".
// Only use the Contacts folder.
   NameResolutionCollection resolvedNames = service.ResolveName("dan", ResolveNameSearchLocation.ContactsOnly, false);
   // Output the list of candidates.   
   foreach (NameResolution nameRes in resolvedNames)
   {
      Console.WriteLine("Contact name: " + nameRes.Mailbox.Name);
      Console.WriteLine("Contact e-mail address: " + nameRes.Mailbox.Address);
      Console.WriteLine("Mailbox type: " + nameRes.Mailbox.MailboxType);
   }

```

Se você armazenar seus contatos em uma pasta diferente da pasta de contatos conhecida, use um dos métodos sobrecarregados para especificar onde procurar candidatos. O exemplo a seguir cria uma lista de pastas para o método **ResolveName** com base na identificação de pasta. O **FolderId** foi reduzida para melhorar a legibilidade. 
  
```cs
// Create a list to store folders to search.
List<FolderId> folders = new List<FolderId>();
// Add a folder to the list based on the FolderId.
folders.Add(new FolderId("AABR8mboAAA="));
// Resolve the ambiguous name "dan".
// Only use the folders specified.
NameResolutionCollection resolvedNames = service.ResolveName("dan", folders, ResolveNameSearchLocation.ContactsOnly, false);
   foreach (NameResolution nameRes in resolvedNames)
   {
      Console.WriteLine("Contact name: " + nameRes.Mailbox.Name);
      Console.WriteLine("Contact e-mail address: " + nameRes.Mailbox.Address);
      Console.WriteLine("Mailbox type: " + nameRes.Mailbox.MailboxType);
   }

```

Se você aplicar filtros e nenhum candidatos são retornados, o [NameResolutionCollection](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) irá conter zero entradas. Você pode verificar isso examinando a propriedade [Count](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.count%28v=exchg.80%29.aspx) da coleção. 
  
## <a name="resolve-ambiguous-names-by-using-ews"></a>Resolver nomes de ambíguos usando o EWS
<a name="bk_EWSMA"> </a>

Você pode usar a operação de EWS [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) para identificar possíveis candidatos para um nome ambíguo. O elemento [UnresolvedEntry](http://msdn.microsoft.com/library/5ac6116a-3b24-40f8-a877-dbe9a6935919%28Office.15%29.aspx) contém o nome ambíguo que você deseja resolver. O exemplo a seguir mostra como resolver o nome Sadie. Isso também é a solicitação XML que o EWS Managed API usa quando você [usar o método ResolveName](#bk_EWSMA), exceto que ele usa um nome diferente para obter exemplos de saída válido.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ResolveNames xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                  ReturnFullContactData="true">
      <UnresolvedEntry>Sadie</UnresolvedEntry>
    </ResolveNames>
  </soap:Body>
</soap:Envelope>
```

A resposta retorna um máximo de 100 candidatos, embora possa haver mais de 100 possíveis candidatos para determinar se apenas os primeiros 100 candidatos de um número maior de candidatos foram retornados, verifique o valor do [IncludesLastItemInRange](http://msdn.microsoft.com/library/e7d6c7d3-548e-48b0-a313-bfef81e4832a%28Office.15%29.aspx) atributo do elemento [ResolutionSet](http://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) . Se o valor for true, não há candidatos não é mais possíveis; Se o valor for false, a operação retornado somente os primeiros 100 de um número maior de candidatos possíveis. 
  
O exemplo a seguir mostra a resposta XML quando um candidato é encontrado. Lembre-se de que o [ResolutionSet](http://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) pode conter até 100 candidatos, cada um representado por um elemento de [resolução](http://msdn.microsoft.com/library/573bed4b-d7b1-4baf-b16f-0795cdebf1a7%28Office.15%29.aspx) e seus elementos filhos. 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ResolutionSet TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Resolution>
              <t:Mailbox>
                <t:Name>Sadie Daniels</t:Name>
                <t:EmailAddress>Sadie@Contoso.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Mailbox</t:MailboxType>
              </t:Mailbox>
              <t:Contact>
                <t:DisplayName>Sadie Daniels</t:DisplayName>
                <t:EmailAddresses>
                  <t:Entry Key="EmailAddress1">SMTP:Sadie@Contoso.com</t:Entry>
                </t:EmailAddresses>
                <t:ContactSource>ActiveDirectory</t:ContactSource>
              </t:Contact>
            </t:Resolution>
          </m:ResolutionSet>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </ResolveNamesResponse>
  </soap:Body>
</soap:Envelope>
```

Você vai nem sempre acompanham candidatos para seu nome ambíguo. O exemplo a seguir mostra a resposta XML, como um erro, quando não há candidatos são encontrados.
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Error">
          <m:MessageText>No results were found.</m:MessageText>
          <m:ResponseCode>ErrorNameResolutionNoResults</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </ResolveNamesResponse>
  </soap:Body>
</soap:Envelope>

```

## <a name="see-also"></a>Confira também


- [Pessoas e contatos no EWS no Exchange](people-and-contacts-in-ews-in-exchange.md)
    
- [Expandir grupos de distribuição, usando o EWS no Exchange 2013](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    

