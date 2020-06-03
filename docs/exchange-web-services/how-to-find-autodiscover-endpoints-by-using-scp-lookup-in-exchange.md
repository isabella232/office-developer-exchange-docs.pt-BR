---
title: Localizar os pontos de extremidade de Descoberta Automática usando pesquisa do SCP no Exchange
manager: kelbow
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: b24228a8-5127-4bac-aef0-9c9e8843c9ff
description: Descubra como localizar os objetos SCP de descoberta automática nos serviços de domínio do Active Directory (AD DS) e usá-los para localizar URLs de ponto de extremidade de descoberta automática para usar com o serviço de descoberta automática do Exchange.
localization_priority: Priority
ms.openlocfilehash: c0c0364a7d69364e12db902f1f22d65c4b5a0cc5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455874"
---
# <a name="find-autodiscover-endpoints-by-using-scp-lookup-in-exchange"></a><span data-ttu-id="f62f6-103">Localizar os pontos de extremidade de Descoberta Automática usando pesquisa do SCP no Exchange</span><span class="sxs-lookup"><span data-stu-id="f62f6-103">Find Autodiscover endpoints by using SCP lookup in Exchange</span></span>

<span data-ttu-id="f62f6-104">Descubra como localizar os objetos SCP de descoberta automática nos serviços de domínio do Active Directory (AD DS) e usá-los para localizar URLs de ponto de extremidade de descoberta automática para usar com o serviço de descoberta automática do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f62f6-104">Find out how to locate Autodiscover SCP objects in Active Directory Domain Services (AD DS) and use them to find Autodiscover endpoint URLs to use with the Exchange Autodiscover service.</span></span>
  
<span data-ttu-id="f62f6-105">A descoberta automática facilita a recuperação de informações que você precisa para se conectar às caixas de correio nos servidores do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f62f6-105">Autodiscover makes it easy to retrieve information that you need to connect to mailboxes on Exchange servers.</span></span> <span data-ttu-id="f62f6-106">No entanto, para usar a descoberta automática, você precisa encontrar servidores de descoberta automática apropriados para o usuário para o qual você está recuperando as configurações.</span><span class="sxs-lookup"><span data-stu-id="f62f6-106">However, in order to use Autodiscover, you need a way to find Autodiscover servers that are appropriate for the user you're retrieving settings for.</span></span> <span data-ttu-id="f62f6-107">Os objetos SCP (ponto de conexão de serviço) no AD DS fornecem uma maneira fácil para os clientes associados ao domínio procurarem servidores de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="f62f6-107">Service connection point (SCP) objects in AD DS provide an easy way for domain-joined clients to look up Autodiscover servers.</span></span> 
  
## <a name="get-set-up-to-find-autodiscover-endpoints"></a><span data-ttu-id="f62f6-108">Obter configuração para localizar pontos de extremidade de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="f62f6-108">Get set up to find Autodiscover endpoints</span></span>
<span data-ttu-id="f62f6-109"><a name="bk_PreReqs"> </a></span><span class="sxs-lookup"><span data-stu-id="f62f6-109"><a name="bk_PreReqs"> </a></span></span>

<span data-ttu-id="f62f6-110">Para localizar objetos do SCP de descoberta automática no AD DS, você precisa ter acesso ao seguinte:</span><span class="sxs-lookup"><span data-stu-id="f62f6-110">To locate Autodiscover SCP objects in AD DS, you need to have access to the following:</span></span>
  
- <span data-ttu-id="f62f6-111">Um servidor que está executando uma versão do Exchange no local, começando com o Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="f62f6-111">A server that is running a version of Exchange on-premises starting with Exchange 2007 SP1.</span></span>
    
- <span data-ttu-id="f62f6-112">Um computador cliente que ingressou no domínio em que o servidor Exchange está instalado.</span><span class="sxs-lookup"><span data-stu-id="f62f6-112">A client computer that is joined to the domain that the Exchange server is installed in.</span></span>
    
- <span data-ttu-id="f62f6-113">Uma conta de usuário que tenha uma caixa de correio no servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="f62f6-113">A user account that has a mailbox on the Exchange server.</span></span> 
    
<span data-ttu-id="f62f6-114">Além disso, antes de começar, você deve estar familiarizado com alguns conceitos básicos.</span><span class="sxs-lookup"><span data-stu-id="f62f6-114">Also, before you begin, you'll want to be familiar some basic concepts.</span></span> <span data-ttu-id="f62f6-115">Veja a seguir alguns recursos que você encontrará úteis.</span><span class="sxs-lookup"><span data-stu-id="f62f6-115">The following are some resources that you'll find helpful.</span></span>
  
<span data-ttu-id="f62f6-116">**Tabela 1. Artigos relacionados para localizar pontos de extremidade de descoberta automática a partir de objetos SCP**</span><span class="sxs-lookup"><span data-stu-id="f62f6-116">**Table 1. Related articles for finding Autodiscover endpoints from SCP objects**</span></span>

|<span data-ttu-id="f62f6-117">**Leia este artigo**</span><span class="sxs-lookup"><span data-stu-id="f62f6-117">**Read this article**</span></span>|<span data-ttu-id="f62f6-118">**Saiba mais sobre...**</span><span class="sxs-lookup"><span data-stu-id="f62f6-118">**To learn about…**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f62f6-119">Descoberta Automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="f62f6-119">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md) <br/> |<span data-ttu-id="f62f6-120">Como funciona o serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="f62f6-120">How the Autodiscover service works.</span></span>  <br/> |
|[<span data-ttu-id="f62f6-121">Publicação com pontos de conexão de serviço</span><span class="sxs-lookup"><span data-stu-id="f62f6-121">Publishing with Service Connection Points</span></span>](https://msdn.microsoft.com/library/3544aa64-ecb0-48a1-ae49-05247a983842%28Office.15%29.aspx) <br/> |<span data-ttu-id="f62f6-122">Como os objetos SCP são usados para publicar dados específicos do serviço.</span><span class="sxs-lookup"><span data-stu-id="f62f6-122">How SCP objects are used to publish service-specific data.</span></span>  <br/> |
   
## <a name="locate-autodiscover-scp-objects-in-ad-ds"></a><span data-ttu-id="f62f6-123">Localizar objetos SCP de descoberta automática no AD DS</span><span class="sxs-lookup"><span data-stu-id="f62f6-123">Locate Autodiscover SCP objects in AD DS</span></span>
<span data-ttu-id="f62f6-124"><a name="bk_LocateScpObjects"> </a></span><span class="sxs-lookup"><span data-stu-id="f62f6-124"><a name="bk_LocateScpObjects"> </a></span></span>

<span data-ttu-id="f62f6-125">A primeira etapa para localizar os pontos de extremidade de descoberta automática publicados no AD DS é localizar os objetos SCP de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="f62f6-125">The first step toward finding Autodiscover endpoints published in AD DS is to locate the Autodiscover SCP objects.</span></span> <span data-ttu-id="f62f6-126">O Exchange publica dois tipos de objetos SCP para descoberta automática:</span><span class="sxs-lookup"><span data-stu-id="f62f6-126">Exchange publishes two types of SCP objects for Autodiscover:</span></span>
  
- <span data-ttu-id="f62f6-127">**Ponteiros SCP** — contêm informações que apontam para servidores LDAP específicos que devem ser usados para localizar os objetos SCP de descoberta automática para o domínio do usuário.</span><span class="sxs-lookup"><span data-stu-id="f62f6-127">**SCP pointers** — These contain information that points to specific LDAP servers that should be used to locate Autodiscover SCP objects for the user's domain.</span></span> <span data-ttu-id="f62f6-128">Os ponteiros SCP são marcados com o GUID seguinte: 67661d7F-8FC4-4fa7-BFAC-E1D7794C1F68.</span><span class="sxs-lookup"><span data-stu-id="f62f6-128">SCP pointers are stamped with the following GUID: 67661d7F-8FC4-4fa7-BFAC-E1D7794C1F68.</span></span> 
    
- <span data-ttu-id="f62f6-129">**URLs de SCP** — contêm URLs para pontos de extremidade de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="f62f6-129">**SCP URLs** — These contain URLs for Autodiscover endpoints.</span></span> <span data-ttu-id="f62f6-130">As URLs de SCP são carimbadas com o seguinte GUID: 77378F46-2C66-4aa9-A6A6-3E7A48B19596.</span><span class="sxs-lookup"><span data-stu-id="f62f6-130">SCP URLs are stamped with the following GUID: 77378F46-2C66-4aa9-A6A6-3E7A48B19596.</span></span> 
    
### <a name="to-locate-autodiscover-scp-objects"></a><span data-ttu-id="f62f6-131">Para localizar os objetos SCP de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="f62f6-131">To locate Autodiscover SCP objects</span></span>

1. <span data-ttu-id="f62f6-132">Leia a propriedade **configurationNamingContext** da entrada de DSE raiz no AD DS para obter o caminho para o contexto de nomenclatura de configuração para o domínio.</span><span class="sxs-lookup"><span data-stu-id="f62f6-132">Read the **configurationNamingContext** property of the root DSE entry in AD DS to get the path to the configuration naming context for the domain.</span></span> <span data-ttu-id="f62f6-133">Você pode fazer isso usando a classe [DirectoryEntry](https://msdn2.microsoft.com/library/z9cddzaa) ou qualquer outra API que possa acessar o AD DS.</span><span class="sxs-lookup"><span data-stu-id="f62f6-133">You can do this by using the [DirectoryEntry](https://msdn2.microsoft.com/library/z9cddzaa) class, or any other API that can acces AD DS.</span></span> 
    
2. <span data-ttu-id="f62f6-134">Procure objetos SCP no contexto de nomenclatura de configuração que tenham o GUID do ponteiro SCP ou a URL do SCP na propriedade **Keywords** .</span><span class="sxs-lookup"><span data-stu-id="f62f6-134">Search for SCP objects in the configuration naming context that have either the SCP pointer GUID or the SCP URL GUID in the **keywords** property.</span></span> 
    
3. <span data-ttu-id="f62f6-135">Verifique os objetos SCP que você encontrou para um ponteiro SCP que tem escopo para o domínio do usuário, verificando a propriedade **Keywords** de uma entrada igual a `"Domain=<domain>"` .</span><span class="sxs-lookup"><span data-stu-id="f62f6-135">Check the SCP objects you found for an SCP pointer that is scoped to the user's domain by checking the **keywords** property for an entry equal to `"Domain=<domain>"`.</span></span> <span data-ttu-id="f62f6-136">Por exemplo, se o endereço de email do usuário for elvin@contoso.com, você procuraria um ponteiro SCP com uma entrada na propriedade **Keywords** que é igual a `"Domain=contoso.com"` .</span><span class="sxs-lookup"><span data-stu-id="f62f6-136">For example, if the user's email address is elvin@contoso.com, you would look for an SCP pointer with an entry in the **keywords** property that is equal to `"Domain=contoso.com"`.</span></span> <span data-ttu-id="f62f6-137">Se um ponteiro SCP correspondente for encontrado, descartar o conjunto de objetos SCP e começar novamente na etapa 1 usando o valor da propriedade **ServiceBindingInformation** como o servidor para se conectar para a entrada do DSE raiz.</span><span class="sxs-lookup"><span data-stu-id="f62f6-137">If a matching SCP pointer is found, discard the set of SCP objects and start over at step 1 using the value of the **serviceBindingInformation** property as the server to connect to for the Root DSE entry.</span></span> 
    
4. <span data-ttu-id="f62f6-138">Se você não encontrar nenhum apontador SCP com escopo para o domínio do usuário, verifique se há ponteiros SCP que não são do escopo para qualquer domínio e salve o valor da propriedade **ServiceBindingInformation** como um servidor de "fallback", caso o servidor atual não dê nenhum resultado.</span><span class="sxs-lookup"><span data-stu-id="f62f6-138">If you don't find any SCP pointers scoped to the user's domain, check for any SCP pointers that aren't scoped to any domain, and save the value of the **serviceBindingInformation** property as a "fallback" server, in case the current server doesn't give you any results.</span></span> 
    
5. <span data-ttu-id="f62f6-139">Se você não encontrou nenhum apontador SCP com escopo para o domínio, você está pronto para passar para a próxima etapa: gerar uma lista priorizada de pontos de extremidade de descoberta automática dos resultados.</span><span class="sxs-lookup"><span data-stu-id="f62f6-139">If you didn't find any SCP pointers scoped to the domain, you're ready to move on to the next step: generating a prioritized list of Autodiscover endpoints from your results.</span></span>
    
## <a name="generate-a-prioritized-list-of-autodiscover-endpoints"></a><span data-ttu-id="f62f6-140">Gerar uma lista priorizada de pontos de extremidade de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="f62f6-140">Generate a prioritized list of Autodiscover endpoints</span></span>
<span data-ttu-id="f62f6-141"><a name="bk_GenerateList"> </a></span><span class="sxs-lookup"><span data-stu-id="f62f6-141"><a name="bk_GenerateList"> </a></span></span>

<span data-ttu-id="f62f6-142">Você pode gerar uma lista priorizada das URLs de ponto de extremidade de descoberta automática, usando o conjunto de objetos SCP que você localizou, fazendo o seguinte:</span><span class="sxs-lookup"><span data-stu-id="f62f6-142">You can generate a prioritized list of Autodiscover endpoint URLs, using the set of SCP objects that you located, by doing the following:</span></span>
  
1. <span data-ttu-id="f62f6-143">Obtenha o nome do site do Active Directory do computador cliente.</span><span class="sxs-lookup"><span data-stu-id="f62f6-143">Get the Active Directory site name of the client computer.</span></span>
    
2. <span data-ttu-id="f62f6-144">Verifique a propriedade **Keywords** em cada URL de SCP no conjunto de objetos SCP que você encontrou e atribua uma prioridade à URL com base nas seguintes regras:</span><span class="sxs-lookup"><span data-stu-id="f62f6-144">Check the **keywords** property on each SCP URL in the set of SCP objects you found, and assign a priority to the URL based on the following rules:</span></span> 
    
  - <span data-ttu-id="f62f6-145">Se a propriedade **Keywords** contiver um valor de `"Site=<site name>"` , onde `<site name>` igual ao nome do site do Active Directory que você recuperou na etapa anterior, atribua a URL a prioridade 1.</span><span class="sxs-lookup"><span data-stu-id="f62f6-145">If the **keywords** property contains a value of `"Site=<site name>"`, where `<site name>` equals the name of the Active Directory site you retrieved in the previous step, assign the URL a priority of 1.</span></span> 
    
  - <span data-ttu-id="f62f6-146">Se a propriedade **Keywords** não contiver uma entrada com um valor que comece com `"Site="` , atribua a URL uma prioridade de 2.</span><span class="sxs-lookup"><span data-stu-id="f62f6-146">If the **keywords** property does not contain an entry with a value that starts with `"Site="`, assign the URL a priority of 2.</span></span> 
    
  - <span data-ttu-id="f62f6-147">Se a propriedade **Keywords** contiver um valor de `"Site=<site name>` , onde não `<site name>` é igual ao nome do site do Active Directory que você recuperou na etapa anterior, atribua a URL a prioridade 3.</span><span class="sxs-lookup"><span data-stu-id="f62f6-147">If the **keywords** property contains a value of `"Site=<site name>`, where `<site name>` does not equal the name of the Active Directory site you retrieved in the previous step, assign the URL a priority of 3.</span></span> 
    
## <a name="code-example-performing-an-scp-lookup"></a><span data-ttu-id="f62f6-148">Exemplo de código: realizando uma pesquisa de SCP</span><span class="sxs-lookup"><span data-stu-id="f62f6-148">Code example: Performing an SCP lookup</span></span>
<span data-ttu-id="f62f6-149"><a name="bk_CodeExample"> </a></span><span class="sxs-lookup"><span data-stu-id="f62f6-149"><a name="bk_CodeExample"> </a></span></span>

<span data-ttu-id="f62f6-150">No exemplo de código a seguir, você verá como localizar objetos do SCP de descoberta automática e gerar uma lista de prioridades de pontos de extremidade de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="f62f6-150">In the following code example, you'll see how to locate Autodiscover SCP objects and generate a prioritized list of Autodiscover endpoints.</span></span>
  
```cs
using System;
using System.Collections.Generic;
using System.DirectoryServices;
using System.DirectoryServices.ActiveDirectory;
namespace ScpLookup
{
    // This sample is for demonstration purposes only. Before you run this sample, make sure 
    // that the code meets the coding requirements of your organization. 
    class Program
    {
        static void Main(string[] args)
        {
            string domain = args[0];
            Console.WriteLine("Performing SCP lookup for {0}.", domain);
            List<string> scpUrls = GetScpUrls(null, domain);
            Console.WriteLine("\nOrdered List of Autodiscover endpoints:");
            foreach (string url in scpUrls)
            {
                Console.WriteLine("  {0}", url);
            }
            Console.WriteLine("SCP lookup done.");
        }
        // GUID for SCP URL keyword.
        private const string ScpUrlGuidString = @"77378F46-2C66-4aa9-A6A6-3E7A48B19596";
        // GUID for SCP pointer keyword.
        private const string ScpPtrGuidString = @"67661d7F-8FC4-4fa7-BFAC-E1D7794C1F68";
        static List<string> GetScpUrls(string ldapServer, string domain)
        {
            // Create a new list to return.
            List<string> scpUrlList = new List<string>();
            string rootDSEPath = null;
            // If ldapServer is null/empty, use LDAP://RootDSE to
            // connect to Active Directory Domain Services (AD DS). Otherwise, use
            // LDAP://SERVERNAME/RootDSE to connect to a specific server.
            if (string.IsNullOrEmpty(ldapServer))
            {
                rootDSEPath = "LDAP://RootDSE";
            }
            else
            {
                rootDSEPath = ldapServer + "/RootDSE";
            }
            SearchResultCollection scpEntries = null;
            try
            {
                // Get the root directory entry.
                DirectoryEntry rootDSE = new DirectoryEntry(rootDSEPath);
                // Get the configuration path.
                string configPath = rootDSE.Properties["configurationNamingContext"].Value as string;
                // Get the configuration entry.
                DirectoryEntry configEntry = new DirectoryEntry("LDAP://" + configPath);
                // Create a search object for the configuration entry.
                DirectorySearcher configSearch = new DirectorySearcher(configEntry);
                // Set the search filter to find SCP URLs and SCP pointers.
                configSearch.Filter = "(&amp;(objectClass=serviceConnectionPoint)" +
                    "(|(keywords=" + ScpPtrGuidString + ")(keywords=" + ScpUrlGuidString + ")))";
                // Specify which properties you want to retrieve.
                configSearch.PropertiesToLoad.Add("keywords");
                configSearch.PropertiesToLoad.Add("serviceBindingInformation");
                scpEntries = configSearch.FindAll();
            }
            catch (Exception ex)
            {
                Console.WriteLine("SCP lookup failed with: ");
                Console.WriteLine(ex.ToString());
            }
            // If no SCP entries were found, then exit.
            if (scpEntries == null || scpEntries.Count <= 0)
            {
                Console.WriteLine("No SCP records found.");
                return null;
            }
            string fallBackLdapPath = null;
            // Check for SCP pointers.
            foreach (SearchResult scpEntry in scpEntries)
            {
                ResultPropertyValueCollection entryKeywords = scpEntry.Properties["keywords"];
                if (CollectionContainsExactValue(entryKeywords, ScpPtrGuidString))
                {
                    string ptrLdapPath = scpEntry.Properties["serviceBindingInformation"][0] as string;
                    // Determine whether this pointer is scoped to the user's domain.
                    if (CollectionContainsExactValue(entryKeywords, "Domain=" + domain))
                    {
                        Console.WriteLine("Found SCP pointer for " + domain + " in " + scpEntry.Path);
                        // Restart SCP lookup with the server assigned for the domain.
                        Console.WriteLine("Restarting SCP lookup in " + ptrLdapPath);
                        return GetScpUrls(ptrLdapPath, domain);
                    }
                    else
                    {
                        // Save the first SCP pointer that is not scoped to a domain as a fallback
                        // in case you do not get any results from this server.
                        if (entryKeywords.Count == 1 &amp;&amp; string.IsNullOrEmpty(fallBackLdapPath))
                        {
                            fallBackLdapPath = ptrLdapPath;
                            Console.WriteLine("Saved fallback SCP pointer: " + fallBackLdapPath);
                        }
                    }
                }
            }
            string computerSiteName = null;
            try
            {
                // Get the name of the ActiveDirectorySite the computer
                // belongs to (if it belongs to one).
                ActiveDirectorySite site = ActiveDirectorySite.GetComputerSite();
                computerSiteName = site.Name;
                Console.WriteLine("Local computer in site: " + computerSiteName);
            }
            catch (Exception ex)
            {
                Console.WriteLine("Unable to get computer site name.");
                Console.WriteLine(ex.ToString());
            }
            if (!string.IsNullOrEmpty(computerSiteName))
            {
                // Scan the search results for SCP URLs.
                // SCP URLs fit into three tiers:
                //   Priority 1: The URL is scoped to the computer's Active Directory site.
                //   Priority 2: The URL is not scoped to any Active Directory site.
                //   Priority 3: The URL is scoped to a different Active Directory site.
                // Temporary lists to hold priority 2 and 3 URLs.
                List<string> priorityTwoUrls = new List<string>();
                List<string> priorityThreeUrls = new List<string>();
                foreach (SearchResult scpEntry in scpEntries)
                {
                    ResultPropertyValueCollection entryKeywords = scpEntry.Properties["keywords"];
                    // Check for SCP URLs.
                    if (CollectionContainsExactValue(entryKeywords, ScpUrlGuidString))
                    {
                        string scpUrlPath = scpEntry.Properties["adsPath"][0] as string;
                        Console.WriteLine("SCP URL found at {0}", scpUrlPath);
                        string scpUrl = scpEntry.Properties["serviceBindingInformation"][0] as string;
                        scpUrl = scpUrl.ToLower();
                        // Determine whether this entry is scoped to the computer's site.
                        if (CollectionContainsExactValue(entryKeywords, "Site=" + computerSiteName))
                        {
                            // Priority 1.
                            if (!scpUrlList.Contains(scpUrl.ToLower()))
                            {
                                Console.WriteLine("Adding priority 1 SCP URL: {0}", scpUrl.ToLower());
                                scpUrlList.Add(scpUrl);
                            }
                            else
                            {
                                Console.WriteLine("Priority 1 SCP URL already found: {0}", scpUrl);
                            }
                        }
                        else
                        {
                            // Determine whether this is a priority 2 or 3 URL.
                            if (CollectionContainsPrefixValue(entryKeywords, "Site="))
                            {
                                // Priority 3.
                                if (!priorityThreeUrls.Contains(scpUrl))
                                {
                                    Console.WriteLine("Adding priority 3 SCP URL: {0}", scpUrl);
                                    priorityThreeUrls.Add(scpUrl);
                                }
                                else
                                {
                                    Console.WriteLine("Priority 3 SCP URL already found: {0}", scpUrl);
                                }
                            }
                            else
                            {
                                // Priority 2.
                                if (!priorityTwoUrls.Contains(scpUrl))
                                {
                                    Console.WriteLine("Adding priority 2 SCP URL: {0}", scpUrl);
                                    priorityTwoUrls.Add(scpUrl);
                                }
                                else
                                {
                                    Console.WriteLine("Priority 2 SCP URL already found: {0}", scpUrl);
                                }
                            }
                        }
                    }
                }
                // Now add the priority 2 URLs into the main list.
                foreach (string priorityTwoUrl in priorityTwoUrls)
                {
                    // If the URL is already in the list as a priority 1, 
                    // don't add it again.
                    if (!scpUrlList.Contains(priorityTwoUrl))
                    {
                        scpUrlList.Add(priorityTwoUrl);
                    }
                }
                // Now add the priority 3 URLs into the main list.
                foreach (string priorityThreeUrl in priorityThreeUrls)
                {
                    // If the URL is already in the list as a priority 1
                    // or priority 2, don't add it again.
                    if (!scpUrlList.Contains(priorityThreeUrl))
                    {
                        scpUrlList.Add(priorityThreeUrl);
                    }
                }
                // If after all this, you still have no URLs in your list,
                // try the fallback SCP pointer, if you have one.
                if (scpUrlList.Count == 0 &amp;&amp; fallBackLdapPath != null)
                {
                    return GetScpUrls(fallBackLdapPath, domain);
                }
            }
            return scpUrlList;
        }
        private static bool CollectionContainsExactValue(ResultPropertyValueCollection collection, string value)
        {
            foreach (object obj in collection)
            {
                string entry = obj as string;
                if (entry != null)
                {
                    if (string.Compare(value, entry, true) == 0)
                        return true;
                }
            }
            return false;
        }
        private static bool CollectionContainsPrefixValue(ResultPropertyValueCollection collection, string value)
        {
            foreach (object obj in collection)
            {
                string entry = obj as string;
                if (entry != null)
                {
                    if (entry.StartsWith(value))
                        return true;
                }
            }
            return false;
        }
    }
}
```

## <a name="next-steps"></a><span data-ttu-id="f62f6-151">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="f62f6-151">Next steps</span></span>
<span data-ttu-id="f62f6-152"><a name="bk_NextSteps"> </a></span><span class="sxs-lookup"><span data-stu-id="f62f6-152"><a name="bk_NextSteps"> </a></span></span>

<span data-ttu-id="f62f6-153">A próxima etapa do processo de descoberta automática é enviar solicitações de descoberta automática para as URLs que você encontrou, começando com as URLs de prioridade 1, e depois prioridade 2 URLs e, por fim, as URLs de prioridade 3.</span><span class="sxs-lookup"><span data-stu-id="f62f6-153">The next step in the Autodiscover process is to send Autodiscover requests to the URLs that you found, starting with priority 1 URLs, then priority 2 URLs, and finally priority 3 URLs.</span></span> <span data-ttu-id="f62f6-154">Para saber mais sobre como enviar solicitações de descoberta automática e lidar com respostas, leia os seguintes artigos:</span><span class="sxs-lookup"><span data-stu-id="f62f6-154">To learn more about how to send Autodiscover requests and handle responses, read the following articles:</span></span>
  
- [<span data-ttu-id="f62f6-155">Obter as configurações de usuário do Exchange usando a Descoberta Automática</span><span class="sxs-lookup"><span data-stu-id="f62f6-155">Get user settings from Exchange by using Autodiscover</span></span>](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
- [<span data-ttu-id="f62f6-156">Manipulação de mensagens de erro de Descoberta Automática</span><span class="sxs-lookup"><span data-stu-id="f62f6-156">Handling Autodiscover error messages</span></span>](handling-autodiscover-error-messages.md)
    
## <a name="see-also"></a><span data-ttu-id="f62f6-157">Confira também</span><span class="sxs-lookup"><span data-stu-id="f62f6-157">See also</span></span>

- [<span data-ttu-id="f62f6-158">Descoberta Automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="f62f6-158">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md)   
- [<span data-ttu-id="f62f6-159">Configurando o aplicativo EWS</span><span class="sxs-lookup"><span data-stu-id="f62f6-159">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)
    

