---
title: Encontrar os pontos de extremidade de descoberta automática usando pesquisa do SCP no Exchange
manager: kelbow
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: b24228a8-5127-4bac-aef0-9c9e8843c9ff
description: Descubra como localizar os objetos de descoberta automática SCP nos serviços de domínio Active Directory (AD DS) e usá-los para encontrar as URLs de ponto de extremidade de descoberta automática para usar com o serviço de descoberta automática do Exchange.
ms.openlocfilehash: 59fd316d0aa0feea81b60c279040da018c51b47d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750711"
---
# <a name="find-autodiscover-endpoints-by-using-scp-lookup-in-exchange"></a><span data-ttu-id="33f55-103">Encontrar os pontos de extremidade de descoberta automática usando pesquisa do SCP no Exchange</span><span class="sxs-lookup"><span data-stu-id="33f55-103">Find Autodiscover endpoints by using SCP lookup in Exchange</span></span>

<span data-ttu-id="33f55-104">Descubra como localizar os objetos de descoberta automática SCP nos serviços de domínio Active Directory (AD DS) e usá-los para encontrar as URLs de ponto de extremidade de descoberta automática para usar com o serviço de descoberta automática do Exchange.</span><span class="sxs-lookup"><span data-stu-id="33f55-104">Find out how to locate Autodiscover SCP objects in Active Directory Domain Services (AD DS) and use them to find Autodiscover endpoint URLs to use with the Exchange Autodiscover service.</span></span>
  
<span data-ttu-id="33f55-105">Descoberta automática facilita recuperar as informações necessárias para conectar-se às caixas de correio em servidores do Exchange.</span><span class="sxs-lookup"><span data-stu-id="33f55-105">Autodiscover makes it easy to retrieve information that you need to connect to mailboxes on Exchange servers.</span></span> <span data-ttu-id="33f55-106">No entanto, para usar a descoberta automática, você precisa descobrir servidores de descoberta automática que são apropriados para o usuário para que estiver recuperando configurações.</span><span class="sxs-lookup"><span data-stu-id="33f55-106">However, in order to use Autodiscover, you need a way to find Autodiscover servers that are appropriate for the user you're retrieving settings for.</span></span> <span data-ttu-id="33f55-107">Objetos de (SCP) do ponto de conexão de serviço no AD DS fornecem uma maneira fácil para clientes de domínio pesquisar outros servidores de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="33f55-107">Service connection point (SCP) objects in AD DS provide an easy way for domain-joined clients to look up Autodiscover servers.</span></span> 
  
## <a name="get-set-up-to-find-autodiscover-endpoints"></a><span data-ttu-id="33f55-108">Configurar o para encontrar os pontos de extremidade de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="33f55-108">Get set up to find Autodiscover endpoints</span></span>
<span data-ttu-id="33f55-109"><a name="bk_PreReqs"> </a></span><span class="sxs-lookup"><span data-stu-id="33f55-109"></span></span>

<span data-ttu-id="33f55-110">Para localizar os objetos SCP de descoberta automática no AD DS, você precisa ter acesso ao seguinte:</span><span class="sxs-lookup"><span data-stu-id="33f55-110">To locate Autodiscover SCP objects in AD DS, you need to have access to the following:</span></span>
  
- <span data-ttu-id="33f55-111">Um servidor que está executando uma versão do Exchange local começando com o Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="33f55-111">A server that is running a version of Exchange on-premises starting with Exchange 2007 SP1.</span></span>
    
- <span data-ttu-id="33f55-112">Um computador cliente que tenha ingressado no domínio em que o servidor do Exchange é instalado no.</span><span class="sxs-lookup"><span data-stu-id="33f55-112">A client computer that is joined to the domain that the Exchange server is installed in.</span></span>
    
- <span data-ttu-id="33f55-113">Uma conta de usuário que tenha uma caixa de correio no Exchange server.</span><span class="sxs-lookup"><span data-stu-id="33f55-113">A user account that has a mailbox on the Exchange server.</span></span> 
    
<span data-ttu-id="33f55-114">Além disso, antes de começar, você vai querer estar familiarizado alguns conceitos básicos.</span><span class="sxs-lookup"><span data-stu-id="33f55-114">Also, before you begin, you'll want to be familiar some basic concepts.</span></span> <span data-ttu-id="33f55-115">Estes são alguns recursos que você encontrará úteis.</span><span class="sxs-lookup"><span data-stu-id="33f55-115">The following are some resources that you'll find helpful.</span></span>
  
<span data-ttu-id="33f55-116">**Tabela 1. Artigos relacionados para localizar os pontos de extremidade de descoberta automática de objetos SCP**</span><span class="sxs-lookup"><span data-stu-id="33f55-116">**Table 1. Related articles for finding Autodiscover endpoints from SCP objects**</span></span>

|<span data-ttu-id="33f55-117">**Leia este artigo**</span><span class="sxs-lookup"><span data-stu-id="33f55-117">**Read this article**</span></span>|<span data-ttu-id="33f55-118">**Para saber mais sobre...**</span><span class="sxs-lookup"><span data-stu-id="33f55-118">**To learn about…**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="33f55-119">Descoberta Automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="33f55-119">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md) <br/> |<span data-ttu-id="33f55-120">Como funciona o serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="33f55-120">How the Autodiscover service works.</span></span>  <br/> |
|[<span data-ttu-id="33f55-121">Publicação com pontos de Conexão de serviço</span><span class="sxs-lookup"><span data-stu-id="33f55-121">Publishing with Service Connection Points</span></span>](http://msdn.microsoft.com/library/3544aa64-ecb0-48a1-ae49-05247a983842%28Office.15%29.aspx) <br/> |<span data-ttu-id="33f55-122">Como os objetos de SCP são usados para publicar dados específicos do serviço.</span><span class="sxs-lookup"><span data-stu-id="33f55-122">How SCP objects are used to publish service-specific data.</span></span>  <br/> |
   
## <a name="locate-autodiscover-scp-objects-in-ad-ds"></a><span data-ttu-id="33f55-123">Localize objetos SCP de descoberta automática no AD DS</span><span class="sxs-lookup"><span data-stu-id="33f55-123">Locate Autodiscover SCP objects in AD DS</span></span>
<span data-ttu-id="33f55-124"><a name="bk_LocateScpObjects"> </a></span><span class="sxs-lookup"><span data-stu-id="33f55-124"></span></span>

<span data-ttu-id="33f55-125">A primeira etapa para encontrar os pontos de extremidade de descoberta automática publicados no AD DS é localizar os objetos SCP de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="33f55-125">The first step toward finding Autodiscover endpoints published in AD DS is to locate the Autodiscover SCP objects.</span></span> <span data-ttu-id="33f55-126">Exchange publica dois tipos de objetos SCP para descoberta automática:</span><span class="sxs-lookup"><span data-stu-id="33f55-126">Exchange publishes two types of SCP objects for Autodiscover:</span></span>
  
- <span data-ttu-id="33f55-127">**Ponteiros de SCP** — eles contêm informações que apontam para os servidores LDAP específicos que devem ser usados para localizar os objetos de descoberta automática SCP para o domínio do usuário.</span><span class="sxs-lookup"><span data-stu-id="33f55-127">**SCP pointers** — These contain information that points to specific LDAP servers that should be used to locate Autodiscover SCP objects for the user's domain.</span></span> <span data-ttu-id="33f55-128">Ponteiros de SCP estão marcados com a seguinte GUID: FC de 8 67661d7F-4-4fa7-BFAC-E1D7794C1F68.</span><span class="sxs-lookup"><span data-stu-id="33f55-128">SCP pointers are stamped with the following GUID: 67661d7F-8FC4-4fa7-BFAC-E1D7794C1F68.</span></span> 
    
- <span data-ttu-id="33f55-129">**URLs de SCP** — eles contêm URLs para pontos de extremidade de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="33f55-129">**SCP URLs** — These contain URLs for Autodiscover endpoints.</span></span> <span data-ttu-id="33f55-130">URLs de SCP estão marcados com a seguinte GUID: 77378F46-2 66 de C-4aa9-A6A6-3E7A48B19596.</span><span class="sxs-lookup"><span data-stu-id="33f55-130">SCP URLs are stamped with the following GUID: 77378F46-2C66-4aa9-A6A6-3E7A48B19596.</span></span> 
    
### <a name="to-locate-autodiscover-scp-objects"></a><span data-ttu-id="33f55-131">Para localizar os objetos SCP de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="33f55-131">To locate Autodiscover SCP objects</span></span>

1. <span data-ttu-id="33f55-132">Ler a propriedade **configurationNamingContext** da entrada DSE no AD DS para obter o caminho para o contexto de nomenclatura de configuração para o domínio raiz.</span><span class="sxs-lookup"><span data-stu-id="33f55-132">Read the **configurationNamingContext** property of the root DSE entry in AD DS to get the path to the configuration naming context for the domain.</span></span> <span data-ttu-id="33f55-133">Você pode fazer isso usando a classe [DirectoryEntry](http://msdn2.microsoft.com/EN-US/library/z9cddzaa) ou qualquer outra API que pode acessar o AD DS.</span><span class="sxs-lookup"><span data-stu-id="33f55-133">You can do this by using the [DirectoryEntry](http://msdn2.microsoft.com/EN-US/library/z9cddzaa) class, or any other API that can acces AD DS.</span></span> 
    
2. <span data-ttu-id="33f55-134">Procurar SCP objetos no contexto de nomenclatura de configuração que tenham tanto o SCP ponteiro GUID ou o GUID da URL de SCP na propriedade **palavras-chave** .</span><span class="sxs-lookup"><span data-stu-id="33f55-134">Search for SCP objects in the configuration naming context that have either the SCP pointer GUID or the SCP URL GUID in the **keywords** property.</span></span> 
    
3. <span data-ttu-id="33f55-135">Verifique o SCP objetos encontrada para um ponteiro de SCP com escopo para o domínio do usuário, verificando a propriedade de **palavras-chave** para uma entrada igual a `"Domain=<domain>"`.</span><span class="sxs-lookup"><span data-stu-id="33f55-135">Check the SCP objects you found for an SCP pointer that is scoped to the user's domain by checking the **keywords** property for an entry equal to `"Domain=<domain>"`.</span></span> <span data-ttu-id="33f55-136">Por exemplo, se o endereço de email do usuário for elvin@contoso.com, você faria procure um SCP ponteiro com uma entrada na propriedade **palavras-chave** for igual a `"Domain=contoso.com"`.</span><span class="sxs-lookup"><span data-stu-id="33f55-136">For example, if the user's email address is elvin@contoso.com, you would look for an SCP pointer with an entry in the **keywords** property that is equal to `"Domain=contoso.com"`.</span></span> <span data-ttu-id="33f55-137">Se for encontrado um ponteiro de SCP correspondente, descartar o conjunto de objetos SCP e recomece na etapa 1, usando o valor da propriedade **serviceBindingInformation** como o servidor para se conectar para a entrada de raiz DSE.</span><span class="sxs-lookup"><span data-stu-id="33f55-137">If a matching SCP pointer is found, discard the set of SCP objects and start over at step 1 using the value of the **serviceBindingInformation** property as the server to connect to for the Root DSE entry.</span></span> 
    
4. <span data-ttu-id="33f55-138">Se você não encontrar qualquer ponteiros de SCP com escopo para o domínio do usuário, procure qualquer ponteiros de SCP que não estão no escopo para qualquer domínio e salve o valor da propriedade **serviceBindingInformation** como um servidor de "fallback", caso o servidor atual não obtiver qualquer um resultados.</span><span class="sxs-lookup"><span data-stu-id="33f55-138">If you don't find any SCP pointers scoped to the user's domain, check for any SCP pointers that aren't scoped to any domain, and save the value of the **serviceBindingInformation** property as a "fallback" server, in case the current server doesn't give you any results.</span></span> 
    
5. <span data-ttu-id="33f55-139">Se você não encontrou qualquer ponteiros de SCP com escopo para o domínio, você estará pronto para passar para a próxima etapa: gerando uma lista de prioridades de pontos de extremidade de descoberta automática a partir de seus resultados.</span><span class="sxs-lookup"><span data-stu-id="33f55-139">If you didn't find any SCP pointers scoped to the domain, you're ready to move on to the next step: generating a prioritized list of Autodiscover endpoints from your results.</span></span>
    
## <a name="generate-a-prioritized-list-of-autodiscover-endpoints"></a><span data-ttu-id="33f55-140">Gerar uma lista de prioridades de pontos de extremidade de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="33f55-140">Generate a prioritized list of Autodiscover endpoints</span></span>
<span data-ttu-id="33f55-141"><a name="bk_GenerateList"> </a></span><span class="sxs-lookup"><span data-stu-id="33f55-141"></span></span>

<span data-ttu-id="33f55-142">Você pode gerar uma lista de prioridades de URLs de ponto de extremidade de descoberta automática, usando o conjunto de objetos SCP que você localizou, fazendo o seguinte:</span><span class="sxs-lookup"><span data-stu-id="33f55-142">You can generate a prioritized list of Autodiscover endpoint URLs, using the set of SCP objects that you located, by doing the following:</span></span>
  
1. <span data-ttu-id="33f55-143">Obtenha o nome do site do Active Directory do computador cliente.</span><span class="sxs-lookup"><span data-stu-id="33f55-143">Get the Active Directory site name of the client computer.</span></span>
    
2. <span data-ttu-id="33f55-144">Verifique a propriedade **palavras-chave** em cada URL SCP no conjunto de objetos SCP encontrada e atribuir uma prioridade para a URL com base nas seguintes regras:</span><span class="sxs-lookup"><span data-stu-id="33f55-144">Check the **keywords** property on each SCP URL in the set of SCP objects you found, and assign a priority to the URL based on the following rules:</span></span> 
    
  - <span data-ttu-id="33f55-145">Se a propriedade de **palavras-chave** contém um valor de `"Site=<site name>"`, onde `<site name>` é igual a, o nome do diretório ativo do site que você recuperada na etapa anterior, atribua o URL uma prioridade de 1.</span><span class="sxs-lookup"><span data-stu-id="33f55-145">If the **keywords** property contains a value of `"Site=<site name>"`, where `<site name>` equals the name of the Active Directory site you retrieved in the previous step, assign the URL a priority of 1.</span></span> 
    
  - <span data-ttu-id="33f55-146">Se a propriedade de **palavras-chave** não contiver uma entrada com um valor que começa com `"Site="`, atribuir uma prioridade de 2 de URL.</span><span class="sxs-lookup"><span data-stu-id="33f55-146">If the **keywords** property does not contain an entry with a value that starts with `"Site="`, assign the URL a priority of 2.</span></span> 
    
  - <span data-ttu-id="33f55-147">Se a propriedade de **palavras-chave** contém um valor de `"Site=<site name>`, onde `<site name>` não igual o nome do site do Active Directory recuperado na etapa anterior, atribuir uma prioridade de 3 de URL.</span><span class="sxs-lookup"><span data-stu-id="33f55-147">If the **keywords** property contains a value of `"Site=<site name>`, where `<site name>` does not equal the name of the Active Directory site you retrieved in the previous step, assign the URL a priority of 3.</span></span> 
    
## <a name="code-example-performing-an-scp-lookup"></a><span data-ttu-id="33f55-148">Exemplo de código: realizando uma pesquisa de SCP</span><span class="sxs-lookup"><span data-stu-id="33f55-148">Code example: Performing an SCP lookup</span></span>
<span data-ttu-id="33f55-149"><a name="bk_CodeExample"> </a></span><span class="sxs-lookup"><span data-stu-id="33f55-149"></span></span>

<span data-ttu-id="33f55-150">No exemplo de código a seguir, você verá como localizar objetos SCP de descoberta automática e gerar uma lista de prioridades de pontos de extremidade de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="33f55-150">In the following code example, you'll see how to locate Autodiscover SCP objects and generate a prioritized list of Autodiscover endpoints.</span></span>
  
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

## <a name="next-steps"></a><span data-ttu-id="33f55-151">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="33f55-151">Next steps</span></span>
<span data-ttu-id="33f55-152"><a name="bk_NextSteps"> </a></span><span class="sxs-lookup"><span data-stu-id="33f55-152"></span></span>

<span data-ttu-id="33f55-153">A próxima etapa do processo de descoberta automática é enviar solicitações de descoberta automática para as URLs que você encontrou, começando com prioridade 1 URLs, e em seguida, URLs de prioridade 2 e finalmente prioridade 3.</span><span class="sxs-lookup"><span data-stu-id="33f55-153">The next step in the Autodiscover process is to send Autodiscover requests to the URLs that you found, starting with priority 1 URLs, then priority 2 URLs, and finally priority 3 URLs.</span></span> <span data-ttu-id="33f55-154">Para saber mais sobre como enviar solicitações de descoberta automática e controlar as respostas, leia os seguintes artigos:</span><span class="sxs-lookup"><span data-stu-id="33f55-154">To learn more about how to send Autodiscover requests and handle responses, read the following articles:</span></span>
  
- [<span data-ttu-id="33f55-155">Obter configurações de usuário do Exchange usando a descoberta automática</span><span class="sxs-lookup"><span data-stu-id="33f55-155">Get user settings from Exchange by using Autodiscover</span></span>](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
- [<span data-ttu-id="33f55-156">Manipulação de mensagens de erro de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="33f55-156">Handling Autodiscover error messages</span></span>](handling-autodiscover-error-messages.md)
    
## <a name="see-also"></a><span data-ttu-id="33f55-157">Confira também</span><span class="sxs-lookup"><span data-stu-id="33f55-157">See also</span></span>

- [<span data-ttu-id="33f55-158">Descoberta Automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="33f55-158">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md)   
- [<span data-ttu-id="33f55-159">Configurando seu aplicativo de EWS</span><span class="sxs-lookup"><span data-stu-id="33f55-159">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)
    

