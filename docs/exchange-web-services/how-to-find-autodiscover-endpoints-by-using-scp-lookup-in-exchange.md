---
title: Localizar os pontos de extremidade de Descoberta Automática usando a pesquisa do SCP no Exchange
manager: kelbow
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: b24228a8-5127-4bac-aef0-9c9e8843c9ff
description: Aprenda a localizar objetos SCP de Descoberta Automática no AD DS (Active Directory Domain Services) e a usá-los para encontrar URLs de pontos de extremidade de descoberta automática para usar com o serviço Descoberta Automática do Exchange.
localization_priority: Priority
ms.openlocfilehash: 5468c18b6d614016915c292c2e02c1a4b570ae37
ms.sourcegitcommit: 37d4ecd4f469690ba1de87baad2f2f58c40c96ba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49348805"
---
# <a name="find-autodiscover-endpoints-by-using-scp-lookup-in-exchange"></a>Localizar os pontos de extremidade de Descoberta Automática usando a pesquisa do SCP no Exchange

Aprenda a localizar objetos SCP de Descoberta Automática no AD DS (Active Directory Domain Services) e a usá-los para encontrar URLs de pontos de extremidade de descoberta automática para usar com o serviço Descoberta Automática do Exchange.
  
A descoberta automática facilita a recuperação de informações necessárias para se conectar às caixas de correio nos servidores Exchange. No entanto, para usar a Descoberta Automática, é preciso encontrar os servidores de Descoberta Automática apropriados para o usuário que você está recuperando as configurações. Os objetos SCP (Ponto de conexão de serviço) no AD DS fornecem uma maneira fácil para os clientes associados ao domínio procurar os servidores de Descoberta Automática. 
  
## <a name="get-set-up-to-find-autodiscover-endpoints"></a>Configurar os pontos de extremidade de Descoberta Automática
<a name="bk_PreReqs"> </a>

Para localizar os objetos SCP de Descoberta Automática no AD DS, você precisa ter acesso aos seguintes:
  
- Um servidor executando uma versão do Exchange local a partir do Exchange 2007 SP1.
    
- Um computador cliente que ingressou no domínio ao qual o servidor Exchange está instalado.
    
- Uma conta de usuário com caixa de correio no servidor Exchange. 
    
Além disso, antes de começar, você vai querer estar familiarizado com alguns conceitos básicos. Veja a seguir alguns recursos úteis.
  
**Tabela 1. Artigos relacionados para localizar pontos de extremidade de Descoberta Automática de objetos SCP**

|**Leia este artigo**|**Saiba mais...**|
|:-----|:-----|
|[Descoberta Automática do Exchange](autodiscover-for-exchange.md) <br/> |Como funciona o serviço Descoberta Automática.  <br/> |
|[Publicação com Pontos de Conexão de Serviço](https://msdn.microsoft.com/library/3544aa64-ecb0-48a1-ae49-05247a983842%28Office.15%29.aspx) <br/> |Como os objetos SCP são usados para publicar dados específicos do serviço.  <br/> |
   
## <a name="locate-autodiscover-scp-objects-in-ad-ds"></a>Localizar objetos SCP de Descoberta Automática no AD DS
<a name="bk_LocateScpObjects"> </a>

O primeira etapa para encontrar os pontos de extremidade de Descoberta Automática publicados no AD DS é localizar os objetos SCP de Descoberta Automática. O Exchange publica dois tipos de objetos SCP para a Descoberta Automática:
  
- **Ponteiros SCP**: contém informações que apontam para servidores LDAP específicos que devem ser usados para localizar os objetos SCP de Descoberta Automática para o domínio do usuário. Os ponteiros SCP são marcados com o seguinte GUID: 67661d7F-8FC4-4fa7-BFAC-E1D7794C1F68. 
    
- **URLs SCP**: contêm URLs para pontos de extremidade de Descoberta Automática. As URLs SCP são marcadas com o seguinte GUID: 77378F46-2C66-4aa9-A6A6-3E7A48B19596. 
    
### <a name="to-locate-autodiscover-scp-objects"></a>Localizar objetos SCP de Descoberta Automática

1. Leia a propriedade **configurationNamingContext** da entrada RootDSE no AD DS para obter o caminho para o contexto de nomenclatura de configuração do domínio. Faça isso usando a classe [DirectoryEntry](https://msdn2.microsoft.com/library/z9cddzaa), ou qualquer outra API que possa acessar o AD DS. 
    
2. Procure por objetos SCP no contexto de nomenclatura de configuração que tenham o GUID do ponteiro SCP ou o GUID de URL SCP na propriedade **keywords**. 
    
3. Verifique os objetos SCP encontrados de um ponteiro SCP cujo escopo é definido para o domínio do usuário, verificando a propriedade **keywords** de uma entrada igual a `"Domain=<domain>"`. Por exemplo, se o endereço de email do usuário for alberto@contoso.com, procure um ponteiro SCP com uma entrada na propriedade **keywords** que seja igual a `"Domain=contoso.com"`. Se um ponteiro SCP correspondente for encontrado, descarte o conjunto de objetos SCP e recomece na etapa 1 usando o valor da propriedade **serviceBindingInformation** como servidor a ser conectado à entrada RootDSE. 
    
4. Caso não encontre ponteiros SCP com escopo para o domínio do usuário, verifique os ponteiros SCP que não estejam com escopo para nenhum domínio, e salve o valor da propriedade **serviceBindingInformation** como servidor "fallback", caso o servidor atual não dê nenhum resultado. 
    
5. Caso não encontre ponteiros SCP com escopo para o domínio, você está pronto para passar para a próxima etapa: gerar uma lista prioritária de pontos de extremidade de Descoberta Automática a partir dos resultados.
    
## <a name="generate-a-prioritized-list-of-autodiscover-endpoints"></a>Gerar uma lista prioritária de pontos de extremidade de Descoberta Automática
<a name="bk_GenerateList"> </a>

Gere uma lista prioritária de URLs de pontos de extremidade de Descoberta Automática, usando o conjunto de objetos SCP que você localizou, fazendo o seguinte:
  
1. Obtenha o nome do site do Active Directory do computador cliente.
    
2. Verifique a propriedade **keywords** em cada URL de SCP no conjunto de objetos SCP encontrados, e atribua uma prioridade à URL com base nas seguintes regras: 
    
  - Se a propriedade **keywords** contém um valor de `"Site=<site name>"`, onde `<site name>` é igual ao nome do site do Active Directory que você recuperou na etapa anterior, atribua à URL uma prioridade 1. 
    
  - Se a propriedade **keywords** não contiver uma entrada com um valor que comece com `"Site="`, atribua à URL uma prioridade 2. 
    
  - Se a propriedade **keywords** contém um valor de `"Site=<site name>`, onde `<site name>` é diferente do nome do site do Active Directory que você recuperou na etapa anterior, atribua à URL uma prioridade 3. 
    
## <a name="code-example-performing-an-scp-lookup"></a>Exemplo de código: executando uma pesquisa SCP
<a name="bk_CodeExample"> </a>

No exemplo de código a seguir, você verá como localizar objetos SCP de Descoberta Automática e gerar uma lista prioritária de pontos de extremidade de Descoberta Automática.
  
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
                        if (entryKeywords.Count == 1 && string.IsNullOrEmpty(fallBackLdapPath))
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
                if (scpUrlList.Count == 0 && fallBackLdapPath != null)
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

A próxima etapa no processo de Descoberta Automática é enviar solicitações de Descoberta Automática para as URLs encontradas, começando com as URLs de prioridade 1, depois com as URLs de prioridade 2 e finalmente com as URLs de prioridade 3. Para saber mais sobre como enviar solicitações de Descoberta Automática e lidar com as respostas, leia os seguintes artigos:
  
- [Obter as configurações de usuário do Exchange usando a Descoberta Automática](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
- [Manipulação de mensagens de erro de Descoberta Automática](handling-autodiscover-error-messages.md)
    
## <a name="see-also"></a>Confira também

- [Descoberta Automática do Exchange](autodiscover-for-exchange.md)   
- [Como configurar o aplicativo EWS](setting-up-your-ews-application.md)
    

