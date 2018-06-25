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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750711"
---
# <a name="find-autodiscover-endpoints-by-using-scp-lookup-in-exchange"></a>Encontrar os pontos de extremidade de descoberta automática usando pesquisa do SCP no Exchange

Descubra como localizar os objetos de descoberta automática SCP nos serviços de domínio Active Directory (AD DS) e usá-los para encontrar as URLs de ponto de extremidade de descoberta automática para usar com o serviço de descoberta automática do Exchange.
  
Descoberta automática facilita recuperar as informações necessárias para conectar-se às caixas de correio em servidores do Exchange. No entanto, para usar a descoberta automática, você precisa descobrir servidores de descoberta automática que são apropriados para o usuário para que estiver recuperando configurações. Objetos de (SCP) do ponto de conexão de serviço no AD DS fornecem uma maneira fácil para clientes de domínio pesquisar outros servidores de descoberta automática. 
  
## <a name="get-set-up-to-find-autodiscover-endpoints"></a>Configurar o para encontrar os pontos de extremidade de descoberta automática
<a name="bk_PreReqs"> </a>

Para localizar os objetos SCP de descoberta automática no AD DS, você precisa ter acesso ao seguinte:
  
- Um servidor que está executando uma versão do Exchange local começando com o Exchange 2007 SP1.
    
- Um computador cliente que tenha ingressado no domínio em que o servidor do Exchange é instalado no.
    
- Uma conta de usuário que tenha uma caixa de correio no Exchange server. 
    
Além disso, antes de começar, você vai querer estar familiarizado alguns conceitos básicos. Estes são alguns recursos que você encontrará úteis.
  
**Tabela 1. Artigos relacionados para localizar os pontos de extremidade de descoberta automática de objetos SCP**

|**Leia este artigo**|**Para saber mais sobre...**|
|:-----|:-----|
|[Descoberta Automática do Exchange](autodiscover-for-exchange.md) <br/> |Como funciona o serviço de descoberta automática.  <br/> |
|[Publicação com pontos de Conexão de serviço](http://msdn.microsoft.com/library/3544aa64-ecb0-48a1-ae49-05247a983842%28Office.15%29.aspx) <br/> |Como os objetos de SCP são usados para publicar dados específicos do serviço.  <br/> |
   
## <a name="locate-autodiscover-scp-objects-in-ad-ds"></a>Localize objetos SCP de descoberta automática no AD DS
<a name="bk_LocateScpObjects"> </a>

A primeira etapa para encontrar os pontos de extremidade de descoberta automática publicados no AD DS é localizar os objetos SCP de descoberta automática. Exchange publica dois tipos de objetos SCP para descoberta automática:
  
- **Ponteiros de SCP** — eles contêm informações que apontam para os servidores LDAP específicos que devem ser usados para localizar os objetos de descoberta automática SCP para o domínio do usuário. Ponteiros de SCP estão marcados com a seguinte GUID: FC de 8 67661d7F-4-4fa7-BFAC-E1D7794C1F68. 
    
- **URLs de SCP** — eles contêm URLs para pontos de extremidade de descoberta automática. URLs de SCP estão marcados com a seguinte GUID: 77378F46-2 66 de C-4aa9-A6A6-3E7A48B19596. 
    
### <a name="to-locate-autodiscover-scp-objects"></a>Para localizar os objetos SCP de descoberta automática

1. Ler a propriedade **configurationNamingContext** da entrada DSE no AD DS para obter o caminho para o contexto de nomenclatura de configuração para o domínio raiz. Você pode fazer isso usando a classe [DirectoryEntry](http://msdn2.microsoft.com/EN-US/library/z9cddzaa) ou qualquer outra API que pode acessar o AD DS. 
    
2. Procurar SCP objetos no contexto de nomenclatura de configuração que tenham tanto o SCP ponteiro GUID ou o GUID da URL de SCP na propriedade **palavras-chave** . 
    
3. Verifique o SCP objetos encontrada para um ponteiro de SCP com escopo para o domínio do usuário, verificando a propriedade de **palavras-chave** para uma entrada igual a `"Domain=<domain>"`. Por exemplo, se o endereço de email do usuário for elvin@contoso.com, você faria procure um SCP ponteiro com uma entrada na propriedade **palavras-chave** for igual a `"Domain=contoso.com"`. Se for encontrado um ponteiro de SCP correspondente, descartar o conjunto de objetos SCP e recomece na etapa 1, usando o valor da propriedade **serviceBindingInformation** como o servidor para se conectar para a entrada de raiz DSE. 
    
4. Se você não encontrar qualquer ponteiros de SCP com escopo para o domínio do usuário, procure qualquer ponteiros de SCP que não estão no escopo para qualquer domínio e salve o valor da propriedade **serviceBindingInformation** como um servidor de "fallback", caso o servidor atual não obtiver qualquer um resultados. 
    
5. Se você não encontrou qualquer ponteiros de SCP com escopo para o domínio, você estará pronto para passar para a próxima etapa: gerando uma lista de prioridades de pontos de extremidade de descoberta automática a partir de seus resultados.
    
## <a name="generate-a-prioritized-list-of-autodiscover-endpoints"></a>Gerar uma lista de prioridades de pontos de extremidade de descoberta automática
<a name="bk_GenerateList"> </a>

Você pode gerar uma lista de prioridades de URLs de ponto de extremidade de descoberta automática, usando o conjunto de objetos SCP que você localizou, fazendo o seguinte:
  
1. Obtenha o nome do site do Active Directory do computador cliente.
    
2. Verifique a propriedade **palavras-chave** em cada URL SCP no conjunto de objetos SCP encontrada e atribuir uma prioridade para a URL com base nas seguintes regras: 
    
  - Se a propriedade de **palavras-chave** contém um valor de `"Site=<site name>"`, onde `<site name>` é igual a, o nome do diretório ativo do site que você recuperada na etapa anterior, atribua o URL uma prioridade de 1. 
    
  - Se a propriedade de **palavras-chave** não contiver uma entrada com um valor que começa com `"Site="`, atribuir uma prioridade de 2 de URL. 
    
  - Se a propriedade de **palavras-chave** contém um valor de `"Site=<site name>`, onde `<site name>` não igual o nome do site do Active Directory recuperado na etapa anterior, atribuir uma prioridade de 3 de URL. 
    
## <a name="code-example-performing-an-scp-lookup"></a>Exemplo de código: realizando uma pesquisa de SCP
<a name="bk_CodeExample"> </a>

No exemplo de código a seguir, você verá como localizar objetos SCP de descoberta automática e gerar uma lista de prioridades de pontos de extremidade de descoberta automática.
  
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

## <a name="next-steps"></a>Próximas etapas
<a name="bk_NextSteps"> </a>

A próxima etapa do processo de descoberta automática é enviar solicitações de descoberta automática para as URLs que você encontrou, começando com prioridade 1 URLs, e em seguida, URLs de prioridade 2 e finalmente prioridade 3. Para saber mais sobre como enviar solicitações de descoberta automática e controlar as respostas, leia os seguintes artigos:
  
- [Obter configurações de usuário do Exchange usando a descoberta automática](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
- [Manipulação de mensagens de erro de descoberta automática](handling-autodiscover-error-messages.md)
    
## <a name="see-also"></a>Confira também

- [Descoberta Automática do Exchange](autodiscover-for-exchange.md)   
- [Configurando seu aplicativo de EWS](setting-up-your-ews-application.md)
    

