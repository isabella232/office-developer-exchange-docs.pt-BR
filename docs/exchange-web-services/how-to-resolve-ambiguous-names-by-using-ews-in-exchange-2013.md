---
title: Resolver nomes ambíguos usando o EWS no Exchange 2013
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 1ba21c54-ecd2-4a1e-80d4-0f4171dea84f
description: Saiba como usar a API Gerenciada do EWS ou o EWS para resolver nomes ambíguos, conseguindo possíveis correspondências dos Serviços de Domínio do Active Directory (AD DS) ou de uma pasta de contatos na caixa de correio do usuário.
ms.openlocfilehash: 5946dad32639b454b3961eaa172b6069ce118b58
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521120"
---
# <a name="resolve-ambiguous-names-by-using-ews-in-exchange-2013"></a>Resolver nomes ambíguos usando o EWS no Exchange 2013

Saiba como usar a API Gerenciada do EWS ou o EWS para resolver nomes ambíguos, conseguindo possíveis correspondências dos Serviços de Domínio do Active Directory (AD DS) ou de uma pasta de contatos na caixa de correio do usuário.
  
Um usuário em sua organização recebe uma lista escrita à mão de nomes e endereços para funcionários que participaram de uma sessão de treinamento. Eles querem enviar um email com algumas informações adicionais para as pessoas na lista, mas não podem ler o endereço de email de todos. Se você quiser resolver esse problema para seus usuários em seu aplicativo, o EWS pode ajudar. Você pode usar o método api gerenciada do [ExchangeService.ResolveName](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) EWS ou a operação [ResolveNames](https://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) EWS para retornar uma lista de possíveis combinações para uma seleção de texto, como parte de um sobrenome. Os itens retornados podem ser caixas de correio de usuário público, grupos de distribuição e contatos. 
  
Observe que Exchange salva endereços de email com tipos de roteamento prefixados, como smtp ou sip, em uma matriz de vários valores. O **método ResolveName** e a operação **ResolveNames** executam uma combinação parcial com cada valor dessa matriz quando você adiciona o tipo de roteamento no início do nome não resolvido, como "sip:User1". Se você não especificar um tipo de roteamento, o método ou a operação será padrão para smtp, corresponderá a uma propriedade de endereço smtp principal e não pesquisará a matriz multivalente. Por exemplo, se você procurar User1 e não incluir o prefixo sip, não receberá sip:User1@Contoso.com como resultado, mesmo que seja uma caixa de correio válida. 
  
Você só pode especificar um nome ambíguo em uma única solicitação. Se você tiver uma lista de nomes ambíguos para resolver, precisará fazer um loop pela lista e chamar o método ou a operação para cada entrada. Os candidatos da pasta Contatos de um usuário terão um valor de ID de item não nulo, que pode ser usado em uma chamada de método [Contact.Bind](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) ou solicitação de operação [GetItem](https://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) para recuperar informações adicionais. Se o candidato for um grupo de distribuição, você poderá usar o método [ExpandGroup(ItemId)](https://msdn.microsoft.com/library/office/ee356407%28v=exchg.80%29.aspx) EWS Managed API ou a operação [ExpandDL](https://msdn.microsoft.com/library/affe84a5-ad98-4aba-83f4-8732938b763d%28Office.15%29.aspx) EWS para obter a lista de membros. Se o parâmetro  _returnContactDetails_ ou o atributo **ReturnFullContactData** EWS estiver definido como true, as entradas do Active Directory retornadas por meio de um método **ResolveName** ou a operação **ResolveNames** incluirão propriedades adicionais que descrevem o contato. O  _parâmetro returnContactDetails_ ou o **atributo ReturnFullContactData** não afeta os dados retornados para contatos e grupos de contatos. 
  
## <a name="resolve-ambiguous-names-by-using-ews-managed-api"></a>Resolver nomes ambíguos usando a API Gerenciada do EWS
<a name="bk_EWSMA"> </a>

Você pode usar o [método ResolveName](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) para encontrar candidatos que corresponderem ao nome ambíguo que você passar. Você pode usar sobrecargas do método **ResolveName** para pesquisar candidatos de cinco maneiras diferentes. 
  
**Tabela 1. Métodos ResolveName sobrecarregados**

|**Method**|**Como funciona**|
|:-----|:-----|
|[ResolveName(String)](https://msdn.microsoft.com/library/dd635548%28v=exchg.80%29.aspx) <br/> |Localiza contatos na pasta Contatos do usuário e na Gal (Lista de Endereços Global) — nessa ordem. A variável de cadeia de caracteres é o nome ambíguo que você está tentando resolver.  <br/> |
|[ResolveName(String, ResolveNameSearchLocation, Boolean)](https://msdn.microsoft.com/library/dd634595%28v=exchg.80%29.aspx) <br/> |Localiza contatos na pasta contatos padrão e/ou na GAL (Lista de Endereços Global). O valor da cadeia de caracteres é o nome ambíguo, o local de pesquisa especifica a pasta Contatos e/ou a GAL e o valor Boolean indica se as informações de contato completas são retornadas.  <br/> |
|[ResolveName(String, ResolveNameSearchLocation, Boolean, PropertySet)](https://msdn.microsoft.com/library/hh532803%28v=exchg.80%29.aspx) <br/> |Localiza contatos na pasta de Contatos padrão e/ou Gal (Lista de Endereços Globais). Esse método permite definir as propriedades retornadas.  <br/> |
|[ResolveName(String, IEnumerable, \<FolderId\> ResolveNameSearchLocation, Boolean)](https://msdn.microsoft.com/library/dd636014%28v=exchg.80%29.aspx) <br/> |Localiza contatos em pastas de contatos especificadas e/ou na GAL (Lista de Endereços Global). Você pode usar esse método para passar uma coleção de pastas para pesquisa. Isso permite que você procure em pastas de contato que não seja a pasta de Contatos padrão.  <br/> |
|[ResolveName(String, IEnumerable, \<FolderId\> ResolveNameSearchLocation, Boolean, PropertySet)](https://msdn.microsoft.com/library/hh532581%28v=exchg.80%29.aspx) <br/> |Localiza contatos na GAL (Lista de Endereços Globais) e/ou em pastas de contato específicas. Esse método permite definir as propriedades retornadas.  <br/> |
   
Vamos começar com um exemplo simples. O exemplo a seguir mostra como resolver a cadeia de caracteres de texto "dan" e a saída do nome e endereço de email de cada candidato encontrado. Este exemplo pressupõe que o **serviço** seja um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário tenha sido autenticado em um servidor Exchange servidor. 
  
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

A resposta retorna um máximo de 100 candidatos, embora possa haver mais de 100 candidatos em potencial. Para determinar se apenas os primeiros 100 candidatos de um número maior de candidatos foram retornados, verifique o valor [de IncludesAllResolutions](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.includesallresolutions%28v=exchg.80%29.aspx) no [objeto NameResolutionCollection.](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) Se o valor for verdadeiro, não haverá mais candidatos possíveis; se o valor for false, o método retornará apenas os primeiros 100 de um número maior de possíveis candidatos. 
  
Se você trabalhar em uma organização grande, é provável que um nome como "dan" retorne o número máximo de 100 candidatos. Para reduzir o número de candidatos retornados, limite onde você pesquisa. O próximo exemplo usa a enumeração [ResolveNameSearchLocation](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.resolvenamesearchlocation%28v=exchg.80%29.aspx) para especificar onde pesquisar para resolver o nome ambíguo. 
  
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

Se você armazenar seus contatos em uma pasta diferente da conhecida pasta Contatos, use um dos métodos sobrecarregados para especificar onde procurar candidatos. O exemplo a seguir cria uma lista de pastas para o **método ResolveName** com base na ID da pasta. O **FolderId** foi reduzido para a capacidade de leitura. 
  
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

Se você aplicar filtros e nenhum candidato for retornado, [NameResolutionCollection](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) conterá zero entradas. Você pode verificar isso analisando a [propriedade Count](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.count%28v=exchg.80%29.aspx) da coleção. 
  
## <a name="resolve-ambiguous-names-by-using-ews"></a>Resolver nomes ambíguos usando o EWS
<a name="bk_EWSMA"> </a>

Você pode usar a [operação ResolveNames](https://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) EWS para identificar possíveis candidatos para um nome ambíguo. O [elemento UnresolvedEntry](https://msdn.microsoft.com/library/5ac6116a-3b24-40f8-a877-dbe9a6935919%28Office.15%29.aspx) contém o nome ambíguo que você deseja resolver. O exemplo a seguir mostra como resolver o nome Sadie. Esta também é a solicitação XML que a API Gerenciada do EWS usa quando você usa o método [ResolveName](#bk_EWSMA), exceto que ele usa um nome diferente para exemplos de saída válidos.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ResolveNames xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                  ReturnFullContactData="true">
      <UnresolvedEntry>Sadie</UnresolvedEntry>
    </ResolveNames>
  </soap:Body>
</soap:Envelope>
```

A resposta retorna um máximo de 100 candidatos, embora possa haver mais de 100 candidatos em potencial Para determinar se apenas os primeiros 100 candidatos de um número maior de candidatos foram retornados, verifique o valor do atributo [IncludesLastItemInRange](https://msdn.microsoft.com/library/e7d6c7d3-548e-48b0-a313-bfef81e4832a%28Office.15%29.aspx) do elemento [ResolutionSet.](https://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) Se o valor for verdadeiro, não haverá mais candidatos possíveis; se o valor for false, a operação retornará apenas os primeiros 100 de um número maior de possíveis candidatos. 
  
O exemplo a seguir mostra a resposta XML quando um candidato é encontrado. Lembre-se de [que o ResolutionSet](https://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) pode conter até 100 candidatos, cada um representado pelo elemento [Resolution](https://msdn.microsoft.com/library/573bed4b-d7b1-4baf-b16f-0795cdebf1a7%28Office.15%29.aspx) e seus elementos filho. 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <ResolveNamesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

Nem sempre você terá candidatos para seu nome ambíguo. O exemplo a seguir mostra a resposta XML, como um erro, quando nenhum candidato é encontrado.
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <ResolveNamesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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
    
- [Expandir grupos de distribuição usando o EWS no Exchange 2013](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    

