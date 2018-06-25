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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750815"
---
# <a name="resolve-ambiguous-names-by-using-ews-in-exchange-2013"></a><span data-ttu-id="40b80-103">Resolver nomes de ambíguos, usando o EWS no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="40b80-103">Resolve ambiguous names by using EWS in Exchange 2013</span></span>

<span data-ttu-id="40b80-104">Saiba como usar a API gerenciada de EWS ou o EWS para resolver nomes de ambíguos obtendo correspondências possíveis do serviços de domínio Active Directory (AD DS) ou uma pasta de contatos na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="40b80-104">Learn how to use the EWS Managed API or EWS to resolve ambiguous names by getting possible matches from Active Directory Domain Services (AD DS) or a contacts folder in your user's mailbox.</span></span>
  
<span data-ttu-id="40b80-105">Um usuário em sua organização recebe uma lista de nomes e endereços de escritas à mão para funcionários que participou de uma sessão de treinamento.</span><span class="sxs-lookup"><span data-stu-id="40b80-105">A user in your organization is given a hand-written list of names and addresses for employees that attended a training session.</span></span> <span data-ttu-id="40b80-106">Eles desejam enviar um email com algumas informações adicionais para pessoas na lista, mas não consegue ler o endereço de email de todos os participantes.</span><span class="sxs-lookup"><span data-stu-id="40b80-106">They want to send an email with some additional information to people on the list, but they can't read everyone's email address.</span></span> <span data-ttu-id="40b80-107">Se você deseja resolver esse problema para os usuários em seu aplicativo, EWS pode ajudar.</span><span class="sxs-lookup"><span data-stu-id="40b80-107">If you want to solve this problem for your users in your application, EWS can help.</span></span> <span data-ttu-id="40b80-108">Você pode usar o método de API gerenciada de EWS [ExchangeService.ResolveName](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) ou a operação de EWS [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) para retornar uma lista de correspondências possíveis para uma seleção de texto, como parte de um sobrenome.</span><span class="sxs-lookup"><span data-stu-id="40b80-108">You can use the [ExchangeService.ResolveName](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) EWS Managed API method or the [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) EWS operation to return a list of potential matches for a selection of text, such as part of a last name.</span></span> <span data-ttu-id="40b80-109">Os itens retornados podem ser caixas de correio de usuário público, grupos de distribuição e contatos.</span><span class="sxs-lookup"><span data-stu-id="40b80-109">The returned items can be public user mailboxes, distribution groups, and contacts.</span></span> 
  
<span data-ttu-id="40b80-110">Observe que o Exchange salva os endereços de email com tipos de roteamento de prefixados, como smtp ou sip, em uma matriz de valores múltiplos.</span><span class="sxs-lookup"><span data-stu-id="40b80-110">Note that Exchange saves email addresses with prefixed routing types, such as smtp or sip, in a multivalue array.</span></span> <span data-ttu-id="40b80-111">O método **ResolveName** e a operação de **ResolveNames** realizar uma correspondência parcial com cada valor dessa matriz quando você adiciona o tipo de roteamento no início do nome não resolvido, como "sip: User1".</span><span class="sxs-lookup"><span data-stu-id="40b80-111">The **ResolveName** method and the **ResolveNames** operation perform a partial match against each value of that array when you add the routing type at the beginning of the unresolved name, such as "sip:User1".</span></span> <span data-ttu-id="40b80-112">Se você não especificar um tipo de roteamento, o método ou a operação será como smtp padrão, associá-lo a uma propriedade de endereço smtp principal e não a matriz de vários valores de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="40b80-112">If you don't specify a routing type, the method or operation will default to smtp, match it to a primary smtp address property, and not search the multivalue array.</span></span> <span data-ttu-id="40b80-113">Por exemplo, se você procurar User1 e não incluir o prefixo sip, você não receberá sip:User1@Contoso.com como resultado, mesmo se for uma caixa de correio válida.</span><span class="sxs-lookup"><span data-stu-id="40b80-113">For example, if you search for User1 and do not include the sip prefix, you will not receive sip:User1@Contoso.com as a result, even if that is a valid mailbox.</span></span> 
  
<span data-ttu-id="40b80-114">Você só pode especificar um nome ambíguo em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="40b80-114">You can only specify one ambiguous name in a single request.</span></span> <span data-ttu-id="40b80-115">Se você tiver uma lista de nomes ambíguos para resolver, você precisará percorrer a lista e chame o método ou a operação para cada entrada.</span><span class="sxs-lookup"><span data-stu-id="40b80-115">If you have a list of ambiguous names to resolve, you will need to loop through the list and call the method or operation for each entry.</span></span> <span data-ttu-id="40b80-116">Os candidatos da pasta de contatos do usuário terão um valor de ID de item de não-nulo, que pode ser usado em uma chamada de método [Contact.Bind](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) ou uma solicitação de operação [GetItem](http://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) para recuperar informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="40b80-116">Candidates from a user's Contacts folder will have a non-null item ID value, which can then be used in a [Contact.Bind](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) method call or [GetItem](http://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) operation request to retrieve additional information.</span></span> <span data-ttu-id="40b80-117">Se o candidato é um grupo de distribuição, você pode usar o método de API gerenciada de EWS [ExpandGroup(ItemId)](http://msdn.microsoft.com/en-us/library/office/ee356407%28v=exchg.80%29.aspx) ou a operação de EWS [ExpandDL](http://msdn.microsoft.com/library/affe84a5-ad98-4aba-83f4-8732938b763d%28Office.15%29.aspx) para obter a lista de membros.</span><span class="sxs-lookup"><span data-stu-id="40b80-117">If the candidate is a distribution group, you can use the [ExpandGroup(ItemId)](http://msdn.microsoft.com/en-us/library/office/ee356407%28v=exchg.80%29.aspx) EWS Managed API method or the [ExpandDL](http://msdn.microsoft.com/library/affe84a5-ad98-4aba-83f4-8732938b763d%28Office.15%29.aspx) EWS operation to get the list of members.</span></span> <span data-ttu-id="40b80-118">Se o parâmetro _returnContactDetails_ ou o atributo **ReturnFullContactData** EWS estiver definido como true, entradas do Active Directory retornado por meio de um método **ResolveName** ou **ResolveNames** operação incluirá propriedades adicionais que descrevem o contato.</span><span class="sxs-lookup"><span data-stu-id="40b80-118">If the  _returnContactDetails_ parameter or the **ReturnFullContactData** EWS attribute is set to true, Active Directory entries returned via a **ResolveName** method or **ResolveNames** operation will include additional properties that describe the contact.</span></span> <span data-ttu-id="40b80-119">O parâmetro _returnContactDetails_ ou o atributo **ReturnFullContactData** não afeta os dados que são retornados para contatos e grupos de contatos.</span><span class="sxs-lookup"><span data-stu-id="40b80-119">The  _returnContactDetails_ parameter or the **ReturnFullContactData** attribute does not affect the data that is returned for contacts and contact groups.</span></span> 
  
## <a name="resolve-ambiguous-names-by-using-ews-managed-api"></a><span data-ttu-id="40b80-120">Resolver nomes de ambíguos usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="40b80-120">Resolve ambiguous names by using EWS Managed API</span></span>
<span data-ttu-id="40b80-121"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="40b80-121"></span></span>

<span data-ttu-id="40b80-122">Você pode usar o método [ResolveName](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) para encontrar os candidatos que correspondam ao nome ambíguo que você passar.</span><span class="sxs-lookup"><span data-stu-id="40b80-122">You can use the [ResolveName](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) method to find candidates that match the ambiguous name you pass.</span></span> <span data-ttu-id="40b80-123">Você pode usar sobrecarregados do método **ResolveName** para procurar candidatos de cinco maneiras diferentes.</span><span class="sxs-lookup"><span data-stu-id="40b80-123">You can use overloads of the **ResolveName** method to search for candidates in five different ways.</span></span> 
  
<span data-ttu-id="40b80-124">**Tabela 1. Métodos de ResolveName sobrecarregados**</span><span class="sxs-lookup"><span data-stu-id="40b80-124">**Table 1. Overloaded ResolveName methods**</span></span>

|<span data-ttu-id="40b80-125">**Method**</span><span class="sxs-lookup"><span data-stu-id="40b80-125">**Method**</span></span>|<span data-ttu-id="40b80-126">**Como funciona**</span><span class="sxs-lookup"><span data-stu-id="40b80-126">**How it works**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="40b80-127">ResolveName(String)</span><span class="sxs-lookup"><span data-stu-id="40b80-127">ResolveName(String)</span></span>](http://msdn.microsoft.com/en-us/library/dd635548%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="40b80-128">Localiza contatos na pasta de contatos do usuário e a lista de endereços Global (GAL) — nesta ordem.</span><span class="sxs-lookup"><span data-stu-id="40b80-128">Finds contacts in the user's Contacts folder and the Global Address List (GAL) — in that order.</span></span> <span data-ttu-id="40b80-129">A variável de cadeia de caracteres é o nome ambíguo que você está tentando resolver.</span><span class="sxs-lookup"><span data-stu-id="40b80-129">The string variable is the ambiguous name you are trying to resolve.</span></span>  <br/> |
|[<span data-ttu-id="40b80-130">ResolveName (cadeia de caracteres, ResolveNameSearchLocation, booleano)</span><span class="sxs-lookup"><span data-stu-id="40b80-130">ResolveName(String, ResolveNameSearchLocation, Boolean)</span></span>](http://msdn.microsoft.com/en-us/library/dd634595%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="40b80-131">Localiza contatos na pasta padrão Contatos e/ou a lista de endereços Global (GAL).</span><span class="sxs-lookup"><span data-stu-id="40b80-131">Finds contacts in the default Contacts folder and/or the Global Address List (GAL).</span></span> <span data-ttu-id="40b80-132">O valor de cadeia de caracteres é o nome ambíguo, o local da pesquisa especifica a pasta Contatos e/ou a GAL e o valor booleano indica se é necessário retornar as informações completas de contato.</span><span class="sxs-lookup"><span data-stu-id="40b80-132">The string value is the ambiguous name, the search location specifies the Contacts folder and/or the GAL, and the Boolean value indicates whether to return the full contact information.</span></span>  <br/> |
|[<span data-ttu-id="40b80-133">ResolveName (cadeia de caracteres, ResolveNameSearchLocation, booleano, PropertySet)</span><span class="sxs-lookup"><span data-stu-id="40b80-133">ResolveName(String, ResolveNameSearchLocation, Boolean, PropertySet)</span></span>](http://msdn.microsoft.com/en-us/library/hh532803%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="40b80-134">Localiza contatos na pasta padrão Contatos e/ou a lista de endereços Global (GAL).</span><span class="sxs-lookup"><span data-stu-id="40b80-134">Finds contacts in the default Contacts folder and/or Global Address List (GAL).</span></span> <span data-ttu-id="40b80-135">Esse método permite que você defina as propriedades que são retornadas.</span><span class="sxs-lookup"><span data-stu-id="40b80-135">This method enables you to set the properties that are returned.</span></span>  <br/> |
|[<span data-ttu-id="40b80-136">ResolveName (String, IEnumerable\<FolderId\>, ResolveNameSearchLocation, booleano)</span><span class="sxs-lookup"><span data-stu-id="40b80-136">ResolveName(String, IEnumerable\<FolderId\>, ResolveNameSearchLocation, Boolean)</span></span>](http://msdn.microsoft.com/en-us/library/dd636014%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="40b80-137">Localiza contatos em pastas de contatos especificadas e/ou a lista de endereços Global (GAL).</span><span class="sxs-lookup"><span data-stu-id="40b80-137">Finds contacts in specified contact folders and/or the Global Address List (GAL).</span></span> <span data-ttu-id="40b80-138">Você pode usar esse método para passar a uma coleção de pastas a serem pesquisadas.</span><span class="sxs-lookup"><span data-stu-id="40b80-138">You can use this method to pass a collection of folders to search.</span></span> <span data-ttu-id="40b80-139">Isso permite que você procure em pastas de contatos que não seja a pasta padrão Contatos.</span><span class="sxs-lookup"><span data-stu-id="40b80-139">This enables you to look in contact folders other than the default Contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="40b80-140">ResolveName (String, IEnumerable\<FolderId\>, ResolveNameSearchLocation, Boolean, PropertySet)</span><span class="sxs-lookup"><span data-stu-id="40b80-140">ResolveName(String, IEnumerable\<FolderId\>, ResolveNameSearchLocation, Boolean, PropertySet)</span></span>](http://msdn.microsoft.com/en-us/library/hh532581%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="40b80-141">Localiza contatos na lista de endereços Global (GAL) e/ou em pastas específicas de contato.</span><span class="sxs-lookup"><span data-stu-id="40b80-141">Finds contacts in the Global Address List (GAL) and/or in specific contact folders.</span></span> <span data-ttu-id="40b80-142">Esse método permite que você defina as propriedades que são retornadas.</span><span class="sxs-lookup"><span data-stu-id="40b80-142">This method enables you to set the properties that are returned.</span></span>  <br/> |
   
<span data-ttu-id="40b80-143">Vamos começar com um exemplo simples.</span><span class="sxs-lookup"><span data-stu-id="40b80-143">Let's start with a simple example.</span></span> <span data-ttu-id="40b80-144">O exemplo a seguir mostra como resolver a cadeia de caracteres de texto "dan" e o nome e endereço de email de cada candidato encontrado de saída.</span><span class="sxs-lookup"><span data-stu-id="40b80-144">The following example shows how to resolve the text string "dan" and output the name and email address of each candidate found.</span></span> <span data-ttu-id="40b80-145">Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="40b80-145">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
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

<span data-ttu-id="40b80-146">A resposta retorna um máximo de 100 candidatos, embora possa haver mais de 100 candidatos em potencial.</span><span class="sxs-lookup"><span data-stu-id="40b80-146">The response returns a maximum of 100 candidates, although there might be more than 100 potential candidates.</span></span> <span data-ttu-id="40b80-147">Para determinar se apenas os primeiros 100 candidatos de um número maior de candidatos foram retornados, verifique o valor de [IncludesAllResolutions](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.includesallresolutions%28v=exchg.80%29.aspx) no objeto [NameResolutionCollection](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="40b80-147">To determine whether only the first 100 candidates of a larger number of candidates were returned, check the value of [IncludesAllResolutions](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.includesallresolutions%28v=exchg.80%29.aspx) in the [NameResolutionCollection](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) object.</span></span> <span data-ttu-id="40b80-148">Se o valor for true, não há candidatos não é mais possíveis; Se o valor for false, o método retornado somente os primeiros 100 de um número maior de candidatos possíveis.</span><span class="sxs-lookup"><span data-stu-id="40b80-148">If the value is true, there are no more possible candidates; if the value is false, the method only returned the first 100 of a larger number of potential candidates.</span></span> 
  
<span data-ttu-id="40b80-149">Se você trabalha em uma grande organização, é provável que um nome como "dan" retornará o número máximo de 100 candidatos.</span><span class="sxs-lookup"><span data-stu-id="40b80-149">If you work in a large organization, it's likely that a name like "dan" will return the maximum number of 100 candidates.</span></span> <span data-ttu-id="40b80-150">Para reduzir o número de candidatos retornado, limite onde você pesquisar.</span><span class="sxs-lookup"><span data-stu-id="40b80-150">To reduce the number of candidates returned, limit where you search.</span></span> <span data-ttu-id="40b80-151">O exemplo a seguir usa a enumeração [ResolveNameSearchLocation](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.resolvenamesearchlocation%28v=exchg.80%29.aspx) para especificar onde pesquisar para resolver o nome ambíguo.</span><span class="sxs-lookup"><span data-stu-id="40b80-151">The next example uses the [ResolveNameSearchLocation](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.resolvenamesearchlocation%28v=exchg.80%29.aspx) enumeration to specify where to search to resolve the ambiguous name.</span></span> 
  
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

<span data-ttu-id="40b80-152">Se você armazenar seus contatos em uma pasta diferente da pasta de contatos conhecida, use um dos métodos sobrecarregados para especificar onde procurar candidatos.</span><span class="sxs-lookup"><span data-stu-id="40b80-152">If you store your contacts in a folder other than the well-known Contacts folder, use one of the overloaded methods to specify where to look for candidates.</span></span> <span data-ttu-id="40b80-153">O exemplo a seguir cria uma lista de pastas para o método **ResolveName** com base na identificação de pasta.</span><span class="sxs-lookup"><span data-stu-id="40b80-153">The following example creates a folder list for the **ResolveName** method based on the folder ID.</span></span> <span data-ttu-id="40b80-154">O **FolderId** foi reduzida para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="40b80-154">The **FolderId** has been shortened for readability.</span></span> 
  
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

<span data-ttu-id="40b80-155">Se você aplicar filtros e nenhum candidatos são retornados, o [NameResolutionCollection](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) irá conter zero entradas.</span><span class="sxs-lookup"><span data-stu-id="40b80-155">If you apply filters and no candidates are returned, the [NameResolutionCollection](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) will contain zero entries.</span></span> <span data-ttu-id="40b80-156">Você pode verificar isso examinando a propriedade [Count](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.count%28v=exchg.80%29.aspx) da coleção.</span><span class="sxs-lookup"><span data-stu-id="40b80-156">You can verify this by looking at the [Count](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.count%28v=exchg.80%29.aspx) property of the collection.</span></span> 
  
## <a name="resolve-ambiguous-names-by-using-ews"></a><span data-ttu-id="40b80-157">Resolver nomes de ambíguos usando o EWS</span><span class="sxs-lookup"><span data-stu-id="40b80-157">Resolve ambiguous names by using EWS</span></span>
<span data-ttu-id="40b80-158"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="40b80-158"></span></span>

<span data-ttu-id="40b80-159">Você pode usar a operação de EWS [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) para identificar possíveis candidatos para um nome ambíguo.</span><span class="sxs-lookup"><span data-stu-id="40b80-159">You can use the [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) EWS operation to identify possible candidates for an ambiguous name.</span></span> <span data-ttu-id="40b80-160">O elemento [UnresolvedEntry](http://msdn.microsoft.com/library/5ac6116a-3b24-40f8-a877-dbe9a6935919%28Office.15%29.aspx) contém o nome ambíguo que você deseja resolver.</span><span class="sxs-lookup"><span data-stu-id="40b80-160">The [UnresolvedEntry](http://msdn.microsoft.com/library/5ac6116a-3b24-40f8-a877-dbe9a6935919%28Office.15%29.aspx) element contains the ambiguous name you want to resolve.</span></span> <span data-ttu-id="40b80-161">O exemplo a seguir mostra como resolver o nome Sadie.</span><span class="sxs-lookup"><span data-stu-id="40b80-161">The following example shows how to resolve the name Sadie.</span></span> <span data-ttu-id="40b80-162">Isso também é a solicitação XML que o EWS Managed API usa quando você [usar o método ResolveName](#bk_EWSMA), exceto que ele usa um nome diferente para obter exemplos de saída válido.</span><span class="sxs-lookup"><span data-stu-id="40b80-162">This is also the XML request that the EWS Managed API uses when you [use the ResolveName method](#bk_EWSMA), except that it uses a different name for valid output examples.</span></span>
  
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

<span data-ttu-id="40b80-163">A resposta retorna um máximo de 100 candidatos, embora possa haver mais de 100 possíveis candidatos para determinar se apenas os primeiros 100 candidatos de um número maior de candidatos foram retornados, verifique o valor do [IncludesLastItemInRange](http://msdn.microsoft.com/library/e7d6c7d3-548e-48b0-a313-bfef81e4832a%28Office.15%29.aspx) atributo do elemento [ResolutionSet](http://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="40b80-163">The response returns a maximum of 100 candidates, although there might be more than 100 potential candidates To determine whether only the first 100 candidates of a larger number of candidates were returned, check the value of the [IncludesLastItemInRange](http://msdn.microsoft.com/library/e7d6c7d3-548e-48b0-a313-bfef81e4832a%28Office.15%29.aspx) attribute of the [ResolutionSet](http://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="40b80-164">Se o valor for true, não há candidatos não é mais possíveis; Se o valor for false, a operação retornado somente os primeiros 100 de um número maior de candidatos possíveis.</span><span class="sxs-lookup"><span data-stu-id="40b80-164">If the value is true, there are no more possible candidates; if the value is false, the operation only returned the first 100 of a larger number of potential candidates.</span></span> 
  
<span data-ttu-id="40b80-165">O exemplo a seguir mostra a resposta XML quando um candidato é encontrado.</span><span class="sxs-lookup"><span data-stu-id="40b80-165">The following example shows the XML response when one candidate is found.</span></span> <span data-ttu-id="40b80-166">Lembre-se de que o [ResolutionSet](http://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) pode conter até 100 candidatos, cada um representado por um elemento de [resolução](http://msdn.microsoft.com/library/573bed4b-d7b1-4baf-b16f-0795cdebf1a7%28Office.15%29.aspx) e seus elementos filhos.</span><span class="sxs-lookup"><span data-stu-id="40b80-166">Remember, the [ResolutionSet](http://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) can contain up to 100 candidates, each one represented by the [Resolution](http://msdn.microsoft.com/library/573bed4b-d7b1-4baf-b16f-0795cdebf1a7%28Office.15%29.aspx) element and its child elements.</span></span> 
  
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

<span data-ttu-id="40b80-167">Você vai nem sempre acompanham candidatos para seu nome ambíguo.</span><span class="sxs-lookup"><span data-stu-id="40b80-167">You're not always going to come up with candidates for your ambiguous name.</span></span> <span data-ttu-id="40b80-168">O exemplo a seguir mostra a resposta XML, como um erro, quando não há candidatos são encontrados.</span><span class="sxs-lookup"><span data-stu-id="40b80-168">The following example shows the XML response, as an error, when no candidates are found.</span></span>
  
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

## <a name="see-also"></a><span data-ttu-id="40b80-169">Confira também</span><span class="sxs-lookup"><span data-stu-id="40b80-169">See also</span></span>


- [<span data-ttu-id="40b80-170">Pessoas e contatos no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="40b80-170">People and contacts in EWS in Exchange</span></span>](people-and-contacts-in-ews-in-exchange.md)
    
- [<span data-ttu-id="40b80-171">Expandir grupos de distribuição, usando o EWS no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="40b80-171">Expand distribution groups by using EWS in Exchange 2013</span></span>](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    

