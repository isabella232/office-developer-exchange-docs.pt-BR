---
title: Resolver nomes ambíguos usando o EWS no Exchange 2013
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1ba21c54-ecd2-4a1e-80d4-0f4171dea84f
description: Saiba como usar a API gerenciada do EWS ou o EWS para resolver nomes ambíguos obtendo possíveis correspondências dos serviços de domínio do Active Directory (AD DS) ou de uma pasta de contatos na caixa de correio do usuário.
ms.openlocfilehash: 5e30e268f54e6ca257e188592e49d168e64332ff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527744"
---
# <a name="resolve-ambiguous-names-by-using-ews-in-exchange-2013"></a><span data-ttu-id="8c5c1-103">Resolver nomes ambíguos usando o EWS no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="8c5c1-103">Resolve ambiguous names by using EWS in Exchange 2013</span></span>

<span data-ttu-id="8c5c1-104">Saiba como usar a API gerenciada do EWS ou o EWS para resolver nomes ambíguos obtendo possíveis correspondências dos serviços de domínio do Active Directory (AD DS) ou de uma pasta de contatos na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-104">Learn how to use the EWS Managed API or EWS to resolve ambiguous names by getting possible matches from Active Directory Domain Services (AD DS) or a contacts folder in your user's mailbox.</span></span>
  
<span data-ttu-id="8c5c1-105">Um usuário na sua organização recebe uma lista de nomes e endereços de escrita à mão para os funcionários que participaram de uma sessão de treinamento.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-105">A user in your organization is given a hand-written list of names and addresses for employees that attended a training session.</span></span> <span data-ttu-id="8c5c1-106">Eles desejam enviar um email com algumas informações adicionais para pessoas na lista, mas não podem ler o endereço de email de todos.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-106">They want to send an email with some additional information to people on the list, but they can't read everyone's email address.</span></span> <span data-ttu-id="8c5c1-107">Se você deseja resolver esse problema para seus usuários em seu aplicativo, o EWS pode ajudar.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-107">If you want to solve this problem for your users in your application, EWS can help.</span></span> <span data-ttu-id="8c5c1-108">Você pode usar o método [ExchangeService. ResolveName](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) EWS Managed API ou a operação [ResolveNames](https://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) EWS para retornar uma lista de possíveis correspondências para uma seleção de texto, como parte de um sobrenome.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-108">You can use the [ExchangeService.ResolveName](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) EWS Managed API method or the [ResolveNames](https://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) EWS operation to return a list of potential matches for a selection of text, such as part of a last name.</span></span> <span data-ttu-id="8c5c1-109">Os itens retornados podem ser caixas de correio de usuários públicos, grupos de distribuição e contatos.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-109">The returned items can be public user mailboxes, distribution groups, and contacts.</span></span> 
  
<span data-ttu-id="8c5c1-110">Observe que o Exchange salva endereços de email com tipos de roteamento prefixos, como SMTP ou SIP, em uma matriz de vários valores.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-110">Note that Exchange saves email addresses with prefixed routing types, such as smtp or sip, in a multivalue array.</span></span> <span data-ttu-id="8c5c1-111">O método **ResolveName** e a operação **ResolveNames** executam uma correspondência parcial em relação a cada valor dessa matriz quando você adiciona o tipo de roteamento no início do nome não resolvido, como "SIP: Usuário1".</span><span class="sxs-lookup"><span data-stu-id="8c5c1-111">The **ResolveName** method and the **ResolveNames** operation perform a partial match against each value of that array when you add the routing type at the beginning of the unresolved name, such as "sip:User1".</span></span> <span data-ttu-id="8c5c1-112">Se você não especificar um tipo de roteamento, o método ou a operação padrão será SMTP, corresponderá a uma propriedade de endereço SMTP primária e não pesquisará a matriz de vários valores.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-112">If you don't specify a routing type, the method or operation will default to smtp, match it to a primary smtp address property, and not search the multivalue array.</span></span> <span data-ttu-id="8c5c1-113">Por exemplo, se você Pesquisar Usuário1 e não incluir o prefixo SIP, não receberá sip:User1@Contoso.com como resultado, mesmo que seja uma caixa de correio válida.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-113">For example, if you search for User1 and do not include the sip prefix, you will not receive sip:User1@Contoso.com as a result, even if that is a valid mailbox.</span></span> 
  
<span data-ttu-id="8c5c1-114">Você só pode especificar um nome ambíguo em uma única solicitação.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-114">You can only specify one ambiguous name in a single request.</span></span> <span data-ttu-id="8c5c1-115">Se você tiver uma lista de nomes ambíguos para resolver, será necessário fazer um loop pela lista e chamar o método ou a operação para cada entrada.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-115">If you have a list of ambiguous names to resolve, you will need to loop through the list and call the method or operation for each entry.</span></span> <span data-ttu-id="8c5c1-116">Os candidatos da pasta contatos de um usuário terão um valor de ID de item não nulo, que pode ser usado em uma chamada de método de [contato. bind](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) ou solicitação de operação [GetItem](https://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) para recuperar informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-116">Candidates from a user's Contacts folder will have a non-null item ID value, which can then be used in a [Contact.Bind](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) method call or [GetItem](https://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) operation request to retrieve additional information.</span></span> <span data-ttu-id="8c5c1-117">Se o candidato for um grupo de distribuição, você poderá usar o método de API gerenciada do EWS (SetGroup [)](https://msdn.microsoft.com/library/office/ee356407%28v=exchg.80%29.aspx) ou a operação do EWS [ExpandDL](https://msdn.microsoft.com/library/affe84a5-ad98-4aba-83f4-8732938b763d%28Office.15%29.aspx) para obter a lista de membros.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-117">If the candidate is a distribution group, you can use the [ExpandGroup(ItemId)](https://msdn.microsoft.com/library/office/ee356407%28v=exchg.80%29.aspx) EWS Managed API method or the [ExpandDL](https://msdn.microsoft.com/library/affe84a5-ad98-4aba-83f4-8732938b763d%28Office.15%29.aspx) EWS operation to get the list of members.</span></span> <span data-ttu-id="8c5c1-118">Se o parâmetro _returnContactDetails_ ou o atributo **ReturnFullContactData** EWS estiver definido como true, as entradas do Active Directory retornadas por meio de um método **ResolveName** ou **ResolveNames** incluirão propriedades adicionais que descrevem o contato.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-118">If the  _returnContactDetails_ parameter or the **ReturnFullContactData** EWS attribute is set to true, Active Directory entries returned via a **ResolveName** method or **ResolveNames** operation will include additional properties that describe the contact.</span></span> <span data-ttu-id="8c5c1-119">O parâmetro _returnContactDetails_ ou o atributo **ReturnFullContactData** não afeta os dados retornados para contatos e grupos de contatos.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-119">The  _returnContactDetails_ parameter or the **ReturnFullContactData** attribute does not affect the data that is returned for contacts and contact groups.</span></span> 
  
## <a name="resolve-ambiguous-names-by-using-ews-managed-api"></a><span data-ttu-id="8c5c1-120">Resolver nomes ambíguos usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="8c5c1-120">Resolve ambiguous names by using EWS Managed API</span></span>
<span data-ttu-id="8c5c1-121"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="8c5c1-121"><a name="bk_EWSMA"> </a></span></span>

<span data-ttu-id="8c5c1-122">Você pode usar o método [ResolveName](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) para localizar candidatos que correspondam ao nome ambíguo aprovado.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-122">You can use the [ResolveName](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) method to find candidates that match the ambiguous name you pass.</span></span> <span data-ttu-id="8c5c1-123">Você pode usar sobrecargas do método **ResolveName** para Pesquisar candidatos de cinco maneiras diferentes.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-123">You can use overloads of the **ResolveName** method to search for candidates in five different ways.</span></span> 
  
<span data-ttu-id="8c5c1-124">**Tabela 1. Métodos resolvêname sobrecarregados**</span><span class="sxs-lookup"><span data-stu-id="8c5c1-124">**Table 1. Overloaded ResolveName methods**</span></span>

|<span data-ttu-id="8c5c1-125">**Método**</span><span class="sxs-lookup"><span data-stu-id="8c5c1-125">**Method**</span></span>|<span data-ttu-id="8c5c1-126">**Como funciona**</span><span class="sxs-lookup"><span data-stu-id="8c5c1-126">**How it works**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8c5c1-127">ResolveName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="8c5c1-127">ResolveName(String)</span></span>](https://msdn.microsoft.com/library/dd635548%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="8c5c1-128">Localiza contatos na pasta contatos do usuário e na GAL (lista de endereços global), nessa ordem.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-128">Finds contacts in the user's Contacts folder and the Global Address List (GAL) — in that order.</span></span> <span data-ttu-id="8c5c1-129">A variável de cadeia de caracteres é o nome ambíguo que você está tentando resolver.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-129">The string variable is the ambiguous name you are trying to resolve.</span></span>  <br/> |
|[<span data-ttu-id="8c5c1-130">ResolveName (String, ResolveNameSearchLocation, Boolean)</span><span class="sxs-lookup"><span data-stu-id="8c5c1-130">ResolveName(String, ResolveNameSearchLocation, Boolean)</span></span>](https://msdn.microsoft.com/library/dd634595%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="8c5c1-131">Localiza contatos na pasta padrão contatos e/ou na lista de endereços global (GAL).</span><span class="sxs-lookup"><span data-stu-id="8c5c1-131">Finds contacts in the default Contacts folder and/or the Global Address List (GAL).</span></span> <span data-ttu-id="8c5c1-132">O valor da cadeia de caracteres é o nome ambíguo, o local da pesquisa especifica a pasta contatos e/ou a GAL e o valor booliano indica se deve retornar as informações completas de contato.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-132">The string value is the ambiguous name, the search location specifies the Contacts folder and/or the GAL, and the Boolean value indicates whether to return the full contact information.</span></span>  <br/> |
|[<span data-ttu-id="8c5c1-133">ResolveName (String, ResolveNameSearchLocation, Boolean, PropertySet)</span><span class="sxs-lookup"><span data-stu-id="8c5c1-133">ResolveName(String, ResolveNameSearchLocation, Boolean, PropertySet)</span></span>](https://msdn.microsoft.com/library/hh532803%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="8c5c1-134">Localiza contatos na pasta padrão contatos e/ou na GAL (lista de endereços global).</span><span class="sxs-lookup"><span data-stu-id="8c5c1-134">Finds contacts in the default Contacts folder and/or Global Address List (GAL).</span></span> <span data-ttu-id="8c5c1-135">Este método permite que você defina as propriedades que são retornadas.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-135">This method enables you to set the properties that are returned.</span></span>  <br/> |
|[<span data-ttu-id="8c5c1-136">ResolveName (cadeia de caracteres, IEnumerable \<FolderId\> , ResolveNameSearchLocation, Boolean)</span><span class="sxs-lookup"><span data-stu-id="8c5c1-136">ResolveName(String, IEnumerable\<FolderId\>, ResolveNameSearchLocation, Boolean)</span></span>](https://msdn.microsoft.com/library/dd636014%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="8c5c1-137">Localiza contatos em pastas de contatos especificadas e/ou na GAL (lista de endereços global).</span><span class="sxs-lookup"><span data-stu-id="8c5c1-137">Finds contacts in specified contact folders and/or the Global Address List (GAL).</span></span> <span data-ttu-id="8c5c1-138">Você pode usar esse método para passar uma coleção de pastas para pesquisa.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-138">You can use this method to pass a collection of folders to search.</span></span> <span data-ttu-id="8c5c1-139">Isso permite que você procure em pastas de contatos diferentes da pasta contatos padrão.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-139">This enables you to look in contact folders other than the default Contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="8c5c1-140">ResolveName (cadeia de caracteres, IEnumerable \<FolderId\> , ResolveNameSearchLocation, Boolean, PropertySet)</span><span class="sxs-lookup"><span data-stu-id="8c5c1-140">ResolveName(String, IEnumerable\<FolderId\>, ResolveNameSearchLocation, Boolean, PropertySet)</span></span>](https://msdn.microsoft.com/library/hh532581%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="8c5c1-141">Localiza contatos na lista de endereços global (GAL) e/ou em pastas de contato específicas.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-141">Finds contacts in the Global Address List (GAL) and/or in specific contact folders.</span></span> <span data-ttu-id="8c5c1-142">Este método permite que você defina as propriedades que são retornadas.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-142">This method enables you to set the properties that are returned.</span></span>  <br/> |
   
<span data-ttu-id="8c5c1-143">Vamos começar com um exemplo simples.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-143">Let's start with a simple example.</span></span> <span data-ttu-id="8c5c1-144">O exemplo a seguir mostra como resolver a cadeia de caracteres de texto "Dan" e saída o nome e o endereço de email de cada candidato encontrado.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-144">The following example shows how to resolve the text string "dan" and output the name and email address of each candidate found.</span></span> <span data-ttu-id="8c5c1-145">Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário foi autenticado em um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-145">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
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

<span data-ttu-id="8c5c1-146">A resposta retorna um máximo de 100 candidatos, embora possa haver mais de 100 possíveis candidatos.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-146">The response returns a maximum of 100 candidates, although there might be more than 100 potential candidates.</span></span> <span data-ttu-id="8c5c1-147">Para determinar se somente os primeiros 100 candidatos de um maior número de candidatos foram retornados, verifique o valor de [IncludesAllResolutions](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.includesallresolutions%28v=exchg.80%29.aspx) no objeto [NameResolutionCollection](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8c5c1-147">To determine whether only the first 100 candidates of a larger number of candidates were returned, check the value of [IncludesAllResolutions](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.includesallresolutions%28v=exchg.80%29.aspx) in the [NameResolutionCollection](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) object.</span></span> <span data-ttu-id="8c5c1-148">Se o valor for true, não haverá mais candidatos possíveis; Se o valor for false, o método retornará apenas o primeiro 100 de um número maior de possíveis candidatos.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-148">If the value is true, there are no more possible candidates; if the value is false, the method only returned the first 100 of a larger number of potential candidates.</span></span> 
  
<span data-ttu-id="8c5c1-149">Se você trabalhar em uma organização de grande porte, é provável que um nome como "Dan" retornará o número máximo de 100 candidatos.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-149">If you work in a large organization, it's likely that a name like "dan" will return the maximum number of 100 candidates.</span></span> <span data-ttu-id="8c5c1-150">Para reduzir o número de candidatos retornados, limite o local em que você pesquisa.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-150">To reduce the number of candidates returned, limit where you search.</span></span> <span data-ttu-id="8c5c1-151">O exemplo a seguir usa a enumeração [ResolveNameSearchLocation](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.resolvenamesearchlocation%28v=exchg.80%29.aspx) para especificar onde Pesquisar para resolver o nome ambíguo.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-151">The next example uses the [ResolveNameSearchLocation](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.resolvenamesearchlocation%28v=exchg.80%29.aspx) enumeration to specify where to search to resolve the ambiguous name.</span></span> 
  
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

<span data-ttu-id="8c5c1-152">Se você armazenar seus contatos em uma pasta diferente da pasta contatos conhecidos, use um dos métodos sobrecarregados para especificar onde procurar candidatos.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-152">If you store your contacts in a folder other than the well-known Contacts folder, use one of the overloaded methods to specify where to look for candidates.</span></span> <span data-ttu-id="8c5c1-153">O exemplo a seguir cria uma lista de pastas para o método **ResolveName** com base na ID da pasta.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-153">The following example creates a folder list for the **ResolveName** method based on the folder ID.</span></span> <span data-ttu-id="8c5c1-154">O **FolderId** foi reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-154">The **FolderId** has been shortened for readability.</span></span> 
  
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

<span data-ttu-id="8c5c1-155">Se você aplicar filtros e nenhum candidato for retornado, o [NameResolutionCollection](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) conterá zero entradas.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-155">If you apply filters and no candidates are returned, the [NameResolutionCollection](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) will contain zero entries.</span></span> <span data-ttu-id="8c5c1-156">Você pode verificar isso observando a propriedade [Count](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.count%28v=exchg.80%29.aspx) da coleção.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-156">You can verify this by looking at the [Count](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.count%28v=exchg.80%29.aspx) property of the collection.</span></span> 
  
## <a name="resolve-ambiguous-names-by-using-ews"></a><span data-ttu-id="8c5c1-157">Resolver nomes ambíguos usando o EWS</span><span class="sxs-lookup"><span data-stu-id="8c5c1-157">Resolve ambiguous names by using EWS</span></span>
<span data-ttu-id="8c5c1-158"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="8c5c1-158"><a name="bk_EWSMA"> </a></span></span>

<span data-ttu-id="8c5c1-159">Você pode usar a operação [ResolveNames](https://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) do EWS para identificar possíveis candidatos para um nome ambíguo.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-159">You can use the [ResolveNames](https://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) EWS operation to identify possible candidates for an ambiguous name.</span></span> <span data-ttu-id="8c5c1-160">O elemento [UnresolvedEntry](https://msdn.microsoft.com/library/5ac6116a-3b24-40f8-a877-dbe9a6935919%28Office.15%29.aspx) contém o nome ambíguo que você deseja resolver.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-160">The [UnresolvedEntry](https://msdn.microsoft.com/library/5ac6116a-3b24-40f8-a877-dbe9a6935919%28Office.15%29.aspx) element contains the ambiguous name you want to resolve.</span></span> <span data-ttu-id="8c5c1-161">O exemplo a seguir mostra como resolver o nome Sadie.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-161">The following example shows how to resolve the name Sadie.</span></span> <span data-ttu-id="8c5c1-162">Essa é também a solicitação XML que a API gerenciada do EWS usa quando você [usa o método ResolveName](#bk_EWSMA), exceto pelo fato de usar um nome diferente para exemplos de saída válidos.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-162">This is also the XML request that the EWS Managed API uses when you [use the ResolveName method](#bk_EWSMA), except that it uses a different name for valid output examples.</span></span>
  
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

<span data-ttu-id="8c5c1-163">A resposta retorna um máximo de 100 candidatos, embora possa haver mais de 100 possíveis candidatos para determinar se somente os primeiros candidatos 100 de um maior número de candidatos foram retornados, verifique o valor do atributo [IncludesLastItemInRange](https://msdn.microsoft.com/library/e7d6c7d3-548e-48b0-a313-bfef81e4832a%28Office.15%29.aspx) do elemento [ResolutionSet](https://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8c5c1-163">The response returns a maximum of 100 candidates, although there might be more than 100 potential candidates To determine whether only the first 100 candidates of a larger number of candidates were returned, check the value of the [IncludesLastItemInRange](https://msdn.microsoft.com/library/e7d6c7d3-548e-48b0-a313-bfef81e4832a%28Office.15%29.aspx) attribute of the [ResolutionSet](https://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="8c5c1-164">Se o valor for true, não haverá mais candidatos possíveis; Se o valor for false, a operação retornará apenas o primeiro 100 de um número maior de possíveis candidatos.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-164">If the value is true, there are no more possible candidates; if the value is false, the operation only returned the first 100 of a larger number of potential candidates.</span></span> 
  
<span data-ttu-id="8c5c1-165">O exemplo a seguir mostra a resposta XML quando um candidato é encontrado.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-165">The following example shows the XML response when one candidate is found.</span></span> <span data-ttu-id="8c5c1-166">Lembre-se de que o [ResolutionSet](https://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) pode conter até 100 candidatos, cada um representado pelo elemento de [resolução](https://msdn.microsoft.com/library/573bed4b-d7b1-4baf-b16f-0795cdebf1a7%28Office.15%29.aspx) e seus elementos filhos.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-166">Remember, the [ResolutionSet](https://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) can contain up to 100 candidates, each one represented by the [Resolution](https://msdn.microsoft.com/library/573bed4b-d7b1-4baf-b16f-0795cdebf1a7%28Office.15%29.aspx) element and its child elements.</span></span> 
  
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

<span data-ttu-id="8c5c1-167">Você nem sempre virá com candidatos para seu nome ambíguo.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-167">You're not always going to come up with candidates for your ambiguous name.</span></span> <span data-ttu-id="8c5c1-168">O exemplo a seguir mostra a resposta XML, como um erro, quando nenhum candidato é encontrado.</span><span class="sxs-lookup"><span data-stu-id="8c5c1-168">The following example shows the XML response, as an error, when no candidates are found.</span></span>
  
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

## <a name="see-also"></a><span data-ttu-id="8c5c1-169">Confira também</span><span class="sxs-lookup"><span data-stu-id="8c5c1-169">See also</span></span>


- [<span data-ttu-id="8c5c1-170">Pessoas e contatos no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8c5c1-170">People and contacts in EWS in Exchange</span></span>](people-and-contacts-in-ews-in-exchange.md)
    
- [<span data-ttu-id="8c5c1-171">Expandir grupos de distribuição usando EWS no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="8c5c1-171">Expand distribution groups by using EWS in Exchange 2013</span></span>](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    

