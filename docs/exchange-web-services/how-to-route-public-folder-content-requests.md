---
title: Rotear solicitações de conteúdo de pasta pública
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 59d2f05e-90fb-471e-ac06-70becc15b295
description: Todas as solicitações de informações de pasta pública que envolvem o conteúdo da pasta pública precisam ser encaminhadas para a caixa de correio de pasta pública que mantém o conteúdo da pasta de destino. Para encaminhar as solicitações para essa caixa de correio, você precisa definir os cabeçalhos X-AnchorMailbox e X-PublicFolderMailbox como valores específicos.
ms.openlocfilehash: 523b9c8efc65253f7970fffeb5800e451784522d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527731"
---
# <a name="route-public-folder-content-requests"></a><span data-ttu-id="43459-104">Rotear solicitações de conteúdo de pasta pública</span><span class="sxs-lookup"><span data-stu-id="43459-104">Route public folder content requests</span></span>

<span data-ttu-id="43459-105">Todas as solicitações de informações de pasta pública que envolvem o conteúdo da pasta pública precisam ser encaminhadas para a caixa de correio de pasta pública que mantém o conteúdo da pasta de destino.</span><span class="sxs-lookup"><span data-stu-id="43459-105">All requests for public folder information that involve the content of the public folder need to be routed to the public folder mailbox that holds the content for the target folder.</span></span> <span data-ttu-id="43459-106">Para encaminhar as solicitações para essa caixa de correio, você precisa definir os cabeçalhos **x-AnchorMailbox** e **x-PublicFolderMailbox** como valores específicos.</span><span class="sxs-lookup"><span data-stu-id="43459-106">To route the requests to that mailbox, you need to set the **X-AnchorMailbox** and **X-PublicFolderMailbox** headers to specific values.</span></span> 
  
<span data-ttu-id="43459-107">A tabela a seguir fornece uma visão geral do processo:</span><span class="sxs-lookup"><span data-stu-id="43459-107">The following table provides an overview of the process:</span></span>
  
<span data-ttu-id="43459-108">**Visão geral da pasta pública**</span><span class="sxs-lookup"><span data-stu-id="43459-108">**Public folder overview**</span></span>

|<span data-ttu-id="43459-109">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="43459-109">Header</span></span>|<span data-ttu-id="43459-110">O que eu preciso?</span><span class="sxs-lookup"><span data-stu-id="43459-110">What do I need?</span></span>|<span data-ttu-id="43459-111">Como posso obtê-lo?</span><span class="sxs-lookup"><span data-stu-id="43459-111">How do I get it?</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="43459-112">**X-AnchorMailbox**</span><span class="sxs-lookup"><span data-stu-id="43459-112">**X-AnchorMailbox**</span></span> <br/> |<span data-ttu-id="43459-113">1. [os valores x-AnchorMailbox e x-PublicFolderInformation](how-to-route-public-folder-hierarchy-requests.md) da caixa de correio de hierarquia de pasta pública.</span><span class="sxs-lookup"><span data-stu-id="43459-113">1. [The X-AnchorMailbox and X-PublicFolderInformation values ](how-to-route-public-folder-hierarchy-requests.md) for the public folder hierarchy mailbox.</span></span><br/><br/><span data-ttu-id="43459-114">2. o GUID da caixa de correio de pasta pública que contém o conteúdo da caixa de correio, que é enviado para o serviço de descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="43459-114">2. The GUID of the public folder mailbox that contains the mailbox content, which is sent to the Autodiscover service.</span></span><br/><br/>  <span data-ttu-id="43459-115">O **AutoDiscoverSMTPAddress** na resposta Autodisover se torna o valor do cabeçalho **X-AnchorMailbox** .</span><span class="sxs-lookup"><span data-stu-id="43459-115">The **AutoDiscoverSMTPAddress** in the Autodisover response becomes the value of the **X-AnchorMailbox** header.</span></span>  <br/> <span data-ttu-id="43459-116">![FAZER](media/Ex15_PF_PFContent.png)</span><span class="sxs-lookup"><span data-stu-id="43459-116">![TODO](media/Ex15_PF_PFContent.png)</span></span>| <span data-ttu-id="43459-117">1. Use o exemplo de código neste artigo, que [implementa a API gerenciada do EWS](#bk_determineguidewsma).</span><span class="sxs-lookup"><span data-stu-id="43459-117">1. Use the code example in this article, which [implements the EWS Managed API](#bk_determineguidewsma).</span></span> <span data-ttu-id="43459-118">Ou [use o EWS](#bk_determineguidews) e converta seus resultados para obter um GUID.</span><span class="sxs-lookup"><span data-stu-id="43459-118">Or [use EWS](#bk_determineguidews) and convert your results to obtain a GUID.</span></span><br/><br/><span data-ttu-id="43459-119">2. [faça uma solicitação de descoberta automática](#bk_makeautodrequest) usando o GUID mais o nome de domínio.</span><span class="sxs-lookup"><span data-stu-id="43459-119">2. [Make an Autodiscover request](#bk_makeautodrequest) by using the GUID plus the domain name.</span></span><br/><br/><span data-ttu-id="43459-120">3. Use o valor do elemento **AutoDiscoverSMTPAddress** retornado na resposta de descoberta automática para [preencher o valor dos cabeçalhos](#bk_setheadervalues).</span><span class="sxs-lookup"><span data-stu-id="43459-120">3. Use the value of the **AutoDiscoverSMTPAddress** element returned in the Autodiscover response to [populate the value of the headers](#bk_setheadervalues).</span></span>  <br/> |
|<span data-ttu-id="43459-121">**X-PublicFolderMailbox**</span><span class="sxs-lookup"><span data-stu-id="43459-121">**X-PublicFolderMailbox**</span></span> <br/> |<span data-ttu-id="43459-122">Seu trabalho é concluído, o valor X-PublicFolderMailbox é o mesmo que o valor X-AnchorMailbox!</span><span class="sxs-lookup"><span data-stu-id="43459-122">Your work is done, the X-PublicFolderMailbox value is the same as the X-AnchorMailbox value!</span></span>  <br/> |<span data-ttu-id="43459-123">Você já tem!</span><span class="sxs-lookup"><span data-stu-id="43459-123">You already have it!</span></span>  <br/> |
   
<span data-ttu-id="43459-124">Depois de determinar os valores de cabeçalho, inclua-os [quando fizer solicitações de conteúdo de pasta pública](#bk_setheadervalues).</span><span class="sxs-lookup"><span data-stu-id="43459-124">After you have determined the header values, include them [when you make public folder content requests](#bk_setheadervalues).</span></span>
  
<span data-ttu-id="43459-125">As etapas neste artigo são específicas para solicitações de conteúdo de pasta pública.</span><span class="sxs-lookup"><span data-stu-id="43459-125">The steps in this article are specific to public folder content requests.</span></span> <span data-ttu-id="43459-126">Para determinar se sua solicitação é uma hierarquia de pasta pública ou uma solicitação de conteúdo, consulte [Routing Public Folder](public-folder-access-with-ews-in-exchange.md#bk_routing)requests.</span><span class="sxs-lookup"><span data-stu-id="43459-126">To determine whether your request is a public folder hierarchy or content request, see [Routing public folder requests](public-folder-access-with-ews-in-exchange.md#bk_routing).</span></span>

<span data-ttu-id="43459-127"><a name="bk_determineguidewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="43459-127"><a name="bk_determineguidewsma"> </a></span></span>

## <a name="determine-the-guid-of-the-public-folder-mailbox-by-using-the-ews-managed-api"></a><span data-ttu-id="43459-128">Determinar o GUID da caixa de correio de pasta pública usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="43459-128">Determine the GUID of the public folder mailbox by using the EWS Managed API</span></span>


<span data-ttu-id="43459-129">Para determinar o GUID da caixa de correio de conteúdo de pasta pública, use o exemplo de código a seguir, que faz o seguinte:</span><span class="sxs-lookup"><span data-stu-id="43459-129">To determine the GUID of the public folder content mailbox, use the following code example, which does the following:</span></span> 
  
- <span data-ttu-id="43459-130">Usa os cabeçalhos **x-AnchorMailbox** e **x-PublicFolderInformation** que você recuperou por [solicitações de hierarquia de pasta pública de roteamento](how-to-route-public-folder-hierarchy-requests.md).</span><span class="sxs-lookup"><span data-stu-id="43459-130">Uses the **X-AnchorMailbox** and **X-PublicFolderInformation** headers you retrieved by [routing public folder hierarchy requests](how-to-route-public-folder-hierarchy-requests.md).</span></span>
    
- <span data-ttu-id="43459-131">Chama o método [FindFolders](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) da API gerenciada do EWS e inclui uma solicitação para a propriedade **PR_REPLICA_LIST** (0x66980102)</span><span class="sxs-lookup"><span data-stu-id="43459-131">Calls the EWS Managed API [FindFolders](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) method, and includes a request for the **PR_REPLICA_LIST** (0x66980102) property</span></span> 
    
<span data-ttu-id="43459-132">O valor **PR_REPLICA_LIST** identifica o GUID da caixa de correio da pasta pública que tem o conteúdo da pasta.</span><span class="sxs-lookup"><span data-stu-id="43459-132">The **PR_REPLICA_LIST** value identifies the mailbox GUID of the public folder mailbox that has the content for the folder.</span></span> <span data-ttu-id="43459-133">A propriedade **PR_REPLICA_LIST** é uma matriz de bytes, mas é convertida como um GUID para este cenário.</span><span class="sxs-lookup"><span data-stu-id="43459-133">The **PR_REPLICA_LIST** property is a byte array, but is cast as a GUID for this scenario.</span></span> <span data-ttu-id="43459-134">O GUID e o nome de domínio são concatenados para formar o endereço em que a descoberta automática deve ser chamada.</span><span class="sxs-lookup"><span data-stu-id="43459-134">The GUID and the domain name are concatenated to form the address on which to call Autodiscover.</span></span> 
  
<span data-ttu-id="43459-135">Este exemplo pressupõe que `service` é o objeto [ExchangeService](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) para o usuário da caixa de correio `PFHAnchorHeader` e que `PFHMailboxHeader` são os valores dos cabeçalhos **x-AnchorMailbox** e **x-PublicFolderMailbox** , e o domínio é o nome do domínio usado pelo locatário.</span><span class="sxs-lookup"><span data-stu-id="43459-135">This example assumes that  `service` is the [ExchangeService](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox user,  `PFHAnchorHeader` and  `PFHMailboxHeader` are the values of the **X-AnchorMailbox** and **X-PublicFolderMailbox** headers, and domain is the domain name used by the tenant.</span></span> 
  
```cs
public static string GetMailboxGuidAddress(ExchangeService service, String PFHAnchorHeader, String PFHMailboxHeader, String domain)
{
    // Create a new folder view, and pass in the maximum number of folders to return.
    FolderView view = new FolderView(10);
    // Create an extended property definition for the PR_REPLICA_LIST property.
    ExtendedPropertyDefinition PR_REPLICA_LIST = new ExtendedPropertyDefinition(0x6698, MapiPropertyType.Binary);
    // As a best practice, limit the properties returned to only those required.
    // In this case, return the folder ID, the folder display name, and 
    // the value of the PR_REPLICA_LIST extended property definition.
    view.PropertySet = new PropertySet(BasePropertySet.IdOnly, FolderSchema.DisplayName, PR_REPLICA_LIST);
    service.HttpHeaders.Add("X-AnchorMailbox", PFHAnchorHeader);
    service.HttpHeaders.Add("X-PublicFolderMailbox", PFHMailboxHeader);
    // Add a call to the CertificateValidationCallback method here if needed.
    // ServicePointManager.ServerCertificateValidationCallback = CertificateValidationCallBack;
    // Call FindFolders to retrieve the folder hierarchy, starting with the PublicFolderRoot folder.
    // This method call results in a FindFolder call to EWS.
    FindFoldersResults findResults = service.FindFolders(WellKnownFolderName.PublicFoldersRoot, view);
    string GuidAsString = null;
    List<string> Guids = new List<string>();
    // For each folder under the root, display the name, and copy the value of the 
    // PR_REPLICA_LIST byte array to a string value. 
    foreach (Folder folder in findResults.Folders)
    {
        Console.WriteLine("Public folder display name: {0}", folder.DisplayName);
        byte[] ByteArr = (byte[])folder.ExtendedProperties[0].Value;
        GuidAsString = System.Text.Encoding.ASCII.GetString(ByteArr, 0, 36);
        Guids.Add(GuidAsString);
        Console.WriteLine("Address for Autodiscover: {0}.{1}\r\n", GuidAsString, domain);
    }
    // Concatenate the GUID value of the PR_REPLICA_LIST with the domain name to generate the 
    // SMTP address to use for the AutoDiscover request for the public folder content mailbox.
    string AutoDSMTPAddress = GuidAsString + "@" + domain;
    // Check that all folders have the same GUID value. If they do not, use the GUID value of the
    // folder that you're requesting content for.
    string commonGuid = CompareGuidsForEquality(Guids);
    if (commonGuid == "Not Equal")
    {
        Console.WriteLine("The GUIDs for all the folders in the hierarchy are not the same. Run the Autodiscover sample using the address returned above that is associated with the folder in your hierarchy request.", AutoDSMTPAddress);
        return null;
    }
    else
    {
        Console.WriteLine("The GUIDs for all public folders in the hierarchy are the same. Run the Autodiscover sample using the {0} address.", AutoDSMTPAddress);
        return AutoDSMTPAddress;
    }
}
// Method to compare the GUID for each folder under the public folder root.
// If each GUID is the same, return the GUID.
// If the GUIDs are not the same, return "Not equal".
public static string CompareGuidsForEquality(List<string> list)
{
    string NotEqual = "Not equal";
    string first = list.First();
    return list.All(x => x == first) ? first : NotEqual;
}
```

<span data-ttu-id="43459-136">Se você recebeu o erro "a solicitação falhou.</span><span class="sxs-lookup"><span data-stu-id="43459-136">If you received the error "The request failed.</span></span> <span data-ttu-id="43459-137">A conexão subjacente foi fechada: não foi possível estabelecer uma relação de confiança para o canal seguro de SSL/TLS ", você precisará [Adicionar uma chamada a um método de retorno de chamada de validação](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span><span class="sxs-lookup"><span data-stu-id="43459-137">The underlying connection was closed: Could not establish trust relationship for the SSL/TLS secure channel", you'll need to [add a call to a validation callback method](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span></span> <span data-ttu-id="43459-138">Um espaço reservado e um comentário para esse método estão incluídos no exemplo de código.</span><span class="sxs-lookup"><span data-stu-id="43459-138">A placeholder and comment for that method is included in the code example.</span></span>
  
<span data-ttu-id="43459-139">Se o GUID da caixa de correio for o mesmo para todas as pastas públicas na raiz da pasta pública, o exemplo indicará o endereço a ser usado ao [chamar a descoberta automática](#bk_makeautodrequest) na saída do console e como o valor de retorno.</span><span class="sxs-lookup"><span data-stu-id="43459-139">If the mailbox GUID is the same for all the public folders under the public folder root, the example indicates the address to use when [calling Autodiscover](#bk_makeautodrequest) in the console output and as the return value.</span></span> <span data-ttu-id="43459-140">Se o GUID da caixa de correio não for o mesmo para todas as pastas públicas na raiz da pasta pública, você precisará [fazer uma solicitação de descoberta automática](#bk_makeautodrequest) no endereço associado à pasta em sua solicitação de conteúdo.</span><span class="sxs-lookup"><span data-stu-id="43459-140">If the mailbox GUID is not the same for all public folders under the public folder root, you need to [Make an Autodiscover request](#bk_makeautodrequest) on the address associated with the folder in your content request.</span></span> 

<span data-ttu-id="43459-141"><a name="bk_determineguidews"> </a></span><span class="sxs-lookup"><span data-stu-id="43459-141"><a name="bk_determineguidews"> </a></span></span>

## <a name="determine-the-guid-of-the-public-folder-mailbox-by-using-ews"></a><span data-ttu-id="43459-142">Determinar o GUID da caixa de correio de pasta pública usando o EWS</span><span class="sxs-lookup"><span data-stu-id="43459-142">Determine the GUID of the public folder mailbox by using EWS</span></span>

<span data-ttu-id="43459-143">O exemplo de código a seguir mostra como recuperar o valor da propriedade **PR_REPLICA_LIST** (0x66980102) usando a operação EWS [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="43459-143">The following code example shows how retrieve the value of the **PR_REPLICA_LIST** (0x66980102) property by using the EWS [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="43459-144">Para o elemento [ExtendedFieldURI](https://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) , o atributo **PropertyTag** é definido como o valor decimal (26264) da propriedade **PR_REPLICA_LIST** e o atributo **recordtypepropriedade** é definido como **Binary**.</span><span class="sxs-lookup"><span data-stu-id="43459-144">For the [ExtendedFieldURI](https://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) element, the **PropertyTag** attribute is set to the decimal value (26264) of the **PR_REPLICA_LIST** property, and the **PropertyType** attribute is set to **Binary**.</span></span>
  
<span data-ttu-id="43459-145">Essa é também a solicitação XML que a API gerenciada do EWS envia quando você usa o método **FindFolders** para [determinar o GUID da caixa de correio de pasta pública usando a API gerenciada do EWS](#bk_determineguidewsma).</span><span class="sxs-lookup"><span data-stu-id="43459-145">This is also the XML request that the EWS Managed API sends when you use the **FindFolders** method to [determine the GUID of the public folder mailbox by using the EWS Managed API](#bk_determineguidewsma).</span></span>
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0913.015
Accept-Encoding: gzip,deflate
Authorization: Basic c29ueWFmQGNvbnRvc28xMDAwLm9ubWljcm9zb2Z0LmNvbTpFWENIIzIwMTQ=
Host: outlook.office365.com
Cookie: ClientId=KZPBLKA9ZMPXAQDW
Content-Length: 1005
Expect: 100-continue
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindFolder Traversal="Shallow">
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="folder:DisplayName" />
          <t:ExtendedFieldURI PropertyTag="26264" PropertyType="Binary" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="10" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="publicfoldersroot" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="43459-146">O servidor responde à solicitação **FindFolder** com uma mensagem [FindFolderResponse](https://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) que inclui o valor da propriedade estendida **PR_REPLICA_LIST** .</span><span class="sxs-lookup"><span data-stu-id="43459-146">The server responds to the **FindFolder** request with a [FindFolderResponse](https://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) message that includes the value of the **PR_REPLICA_LIST** extended property.</span></span> <span data-ttu-id="43459-147">Observe que o valor da propriedade aparece na resposta do EWS como o formato de cadeia de caracteres de uma matriz de bytes codificada em base 64.</span><span class="sxs-lookup"><span data-stu-id="43459-147">Note that the value of the property appears on the EWS response as the string format of a base-64 encoded byte array.</span></span> <span data-ttu-id="43459-148">Alguns valores de cabeçalho na resposta são reduzidos para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="43459-148">Some header values in the response are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?><s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="1019" MinorBuildNumber="15" Version="V2_17" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body>
    <m:FindFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="2" TotalItemsInView="2" IncludesLastItemInRange="true">
            <t:Folders>
              <t:ContactsFolder>
                <t:FolderId Id="AAEuAAAAAADL8shaNEKnQYVvRbpoY9vDAQBGDloItRzyTrAt+XVzRr/YAABdofPkAAA=" ChangeKey="AwAAABYAAABGDloItRzyTrAt+XVzRr/YAABdo/2h"/>
                <t:DisplayName>My Public Contacts</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x6698" PropertyType="Binary"/>
                  <t:Value>MWVjMmEyMzYtZWQ5My00Zjg4LWI5YzYtMzNlNjNmYTRhYTQ0AA==</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:Folder>
                <t:FolderId Id="AQEuAAADy/LIWjRCp0GFb0W6aGPbwwEARg5aCLUc8k6wLfl1c0a/2AAAAxEAAAA=" ChangeKey="AQAAABYAAABGDloItRzyTrAt+XVzRr/YAABdo/W/"/>
                <t:DisplayName>SampleFolder</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x6698" PropertyType="Binary"/>
                  <t:Value>MWVjMmEyMzYtZWQ5My00Zjg4LWI5YzYtMzNlNjNmYTRhYTQ0AA==</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </m:FindFolderResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="43459-149">Para usar o valor do **PR_REPLICA_LIST** RETORNADO no XML, MWVjMmEyMzYtZWQ5My00Zjg4LWI5YzYtMzNlNjNmYTRhYTQ0AA = =, para determinar o GUID da caixa de correio, o valor deve ser convertido em um GUID em um formato semelhante à forma como o valor é convertido no [exemplo de código de API gerenciada do EWS](#bk_determineguidewsma).</span><span class="sxs-lookup"><span data-stu-id="43459-149">In order to use the value of the **PR_REPLICA_LIST** returned in the XML, MWVjMmEyMzYtZWQ5My00Zjg4LWI5YzYtMzNlNjNmYTRhYTQ0AA==, to determine the mailbox GUID, the value must be converted into a GUID in a format similar to how the value is converted in the [EWS Managed API code example](#bk_determineguidewsma).</span></span> <span data-ttu-id="43459-150">O GUID é concatenado com o nome de domínio para criar um endereço SMTP, que é incluído na [solicitação de descoberta automática](#bk_makeautodrequest).</span><span class="sxs-lookup"><span data-stu-id="43459-150">The GUID is then concatenated with the domain name to create an SMTP address, which is included in the [Autodiscover request](#bk_makeautodrequest).</span></span>
  
## <a name="make-an-autodiscover-request"></a><span data-ttu-id="43459-151">Fazer uma solicitação de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="43459-151">Make an Autodiscover request</span></span>
<span data-ttu-id="43459-152"><a name="bk_makeautodrequest"> </a></span><span class="sxs-lookup"><span data-stu-id="43459-152"><a name="bk_makeautodrequest"> </a></span></span>

<span data-ttu-id="43459-153">Use o endereço retornado pelo `GetMailboxGuidAddress` método para chamar a descoberta automática.</span><span class="sxs-lookup"><span data-stu-id="43459-153">Use the address returned by the  `GetMailboxGuidAddress` method to call Autodiscover.</span></span> <span data-ttu-id="43459-154">Recomendamos que você use o [Exchange 2013: obter as configurações do usuário com](https://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e) o exemplo de código de descoberta automática para chamar o serviço de descoberta automática porque ele simplifica o processo de descoberta automática para você.</span><span class="sxs-lookup"><span data-stu-id="43459-154">We recommend that you use the [Exchange 2013: Get user settings with Autodiscover](https://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e) code sample to call the Autodiscover service because it streamlines the Autodiscover process for you.</span></span> <span data-ttu-id="43459-155">Este exemplo de código usa os argumentos de linha de comando listados na tabela a seguir para chamar o serviço de descoberta automática do POX para recuperar o valor do [AutoDiscoverSMTPAddress](https://msdn.microsoft.com/library/office/dn750991%28v=exchg.150%29.aspx) associado ao GUID da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="43459-155">This code sample uses the command-line arguments listed in the following table to call the POX Autodiscover service to retrieve the [AutoDiscoverSMTPAddress](https://msdn.microsoft.com/library/office/dn750991%28v=exchg.150%29.aspx) value associated with the mailbox GUID.</span></span> 

  
|<span data-ttu-id="43459-156">**Argumento**</span><span class="sxs-lookup"><span data-stu-id="43459-156">**Argument**</span></span>|<span data-ttu-id="43459-157">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="43459-157">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="43459-158">emailAddress</span><span class="sxs-lookup"><span data-stu-id="43459-158">emailAddress</span></span>  <br/> |<span data-ttu-id="43459-159">O endereço retornado pelo `GetMailboxGuidAddress` método em [determine o GUID da caixa de correio de pasta pública](#bk_determineguidewsma).</span><span class="sxs-lookup"><span data-stu-id="43459-159">The address returned by the  `GetMailboxGuidAddress` method in [Determine the GUID of the public folder mailbox](#bk_determineguidewsma).</span></span>  <br/> |
|<span data-ttu-id="43459-160">-skipSOAP</span><span class="sxs-lookup"><span data-stu-id="43459-160">-skipSOAP</span></span>  <br/> |<span data-ttu-id="43459-161">Indica que as solicitações de descoberta automática do POX são obrigatórias.</span><span class="sxs-lookup"><span data-stu-id="43459-161">Indicates that POX Autodiscover requests are required.</span></span>  <br/> |
|<span data-ttu-id="43459-162">-auth authEmailAddress</span><span class="sxs-lookup"><span data-stu-id="43459-162">-auth authEmailAddress</span></span>  <br/> |<span data-ttu-id="43459-163">O endereço de email do usuário da caixa de correio, que é usado para autenticação.</span><span class="sxs-lookup"><span data-stu-id="43459-163">The mailbox user's email address, which is used for authentication.</span></span> <span data-ttu-id="43459-164">Você será solicitado a inserir a senha do usuário da caixa de correio quando executar o exemplo.</span><span class="sxs-lookup"><span data-stu-id="43459-164">You will be prompted to enter the mailbox user's password when you run the sample.</span></span>  <br/> |
   
<span data-ttu-id="43459-165">Por exemplo, os argumentos de linha de comando devem ter a seguinte aparência:</span><span class="sxs-lookup"><span data-stu-id="43459-165">For example, the command-line arguments should look like this:</span></span>
  
`1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com -skipSOAP -auth sonyaf@contoso.com`

<span data-ttu-id="43459-166">Em que `1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com` é o endereço retornado pelo método **GetMailboxGuidAddress** e `sonyaf@contoso.com` é o usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="43459-166">Where `1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com` is the address returned by the **GetMailboxGuidAddress** method, and `sonyaf@contoso.com` is the mailbox user.</span></span> 
  
<span data-ttu-id="43459-167">Quando você executa o **Exchange 2013: obter as configurações de usuário com** o exemplo de descoberta automática, a última resposta de descoberta automática deve ser bem-sucedida e incluir todas as configurações de usuário associadas ao GUID da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="43459-167">When you run the **Exchange 2013: Get user settings with Autodiscover** sample, the last Autodiscover response should be successful and include all the user settings associated with the mailbox GUID.</span></span> <span data-ttu-id="43459-168">Salve a configuração de usuário do **AutoDiscoverSMTPAddress** localmente, pois você usará isso na próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="43459-168">Save the **AutoDiscoverSMTPAddress** user setting locally, as you'll use that in the next step.</span></span> 
  
<span data-ttu-id="43459-169">Como alternativa, se você não deseja usar o **Exchange 2013: obter configurações do usuário com** o exemplo de descoberta automática, você pode obter a configuração de usuário do **AutoDiscoverSMTPAddress** [gerando uma lista de pontos de extremidade de descoberta automática](how-to-generate-a-list-of-autodiscover-endpoints.md)e, em seguida, enviando a seguinte solicitação de descoberta automática do Pox para cada URL até receber uma resposta bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="43459-169">Alternatively, if you do not want to use **Exchange 2013: Get user settings with Autodiscover** sample, you can get the **AutoDiscoverSMTPAddress** user setting by [generating a list of Autodiscover endpoints](how-to-generate-a-list-of-autodiscover-endpoints.md), and then sending the following POX Autodiscover request to each URL until you receive a successful response.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
  <Request>
    <EMailAddress>1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com</EMailAddress>
    <AcceptableResponseSchema>https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
  </Request>
</Autodiscover>
```

<span data-ttu-id="43459-170">Para obter mais informações sobre o processo de descoberta automática, consulte [descoberta automática do Exchange](autodiscover-for-exchange.md), [gerar uma lista de pontos de extremidade de descoberta automática](how-to-generate-a-list-of-autodiscover-endpoints.md)e [obter as configurações de usuário do Exchange usando a descoberta automática](how-to-get-user-settings-from-exchange-by-using-autodiscover.md).</span><span class="sxs-lookup"><span data-stu-id="43459-170">For more information about the Autodiscover process, see [Autodiscover for Exchange](autodiscover-for-exchange.md), [Generate a list of Autodiscover endpoints](how-to-generate-a-list-of-autodiscover-endpoints.md), and [Get user settings from Exchange by using Autodiscover](how-to-get-user-settings-from-exchange-by-using-autodiscover.md).</span></span>
  
## <a name="set-the-values-of-the-x-anchormailbox-and-x-publicfoldermailbox-headers"></a><span data-ttu-id="43459-171">Definir os valores dos cabeçalhos X-AnchorMailbox e X-PublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="43459-171">Set the values of the X-AnchorMailbox and X-PublicFolderMailbox headers</span></span>
<span data-ttu-id="43459-172"><a name="bk_setheadervalues"> </a></span><span class="sxs-lookup"><span data-stu-id="43459-172"><a name="bk_setheadervalues"> </a></span></span>

<span data-ttu-id="43459-173">Usando o valor do **AutoDiscoverSMTPAddress** adquirido em [fazer uma solicitação de descoberta automática](#bk_makeautodrequest), defina os valores dos cabeçalhos **x-AnchorMailbox** e **x-PublicFolderMailbox** em sua solicitação de conteúdo de pasta pública.</span><span class="sxs-lookup"><span data-stu-id="43459-173">Using the value for the **AutoDiscoverSMTPAddress** acquired in [Make an Autodiscover request](#bk_makeautodrequest), set the values of the **X-AnchorMailbox** and **X-PublicFolderMailbox** headers in your public folder content request.</span></span> 
  
<span data-ttu-id="43459-174">Por exemplo, dado um AutoDiscoverSMTPAddress de NewPublicFolder@contoso.com, inclua os seguintes cabeçalhos ao fazer chamadas para os seguintes métodos ou operações.</span><span class="sxs-lookup"><span data-stu-id="43459-174">For example, given an AutoDiscoverSMTPAddress of NewPublicFolder@contoso.com, include the following headers when making calls to the following methods or operations.</span></span>
  
`X-AnchorMailbox: NewPublicFolder@contoso.com`<br/>
`X-PublicFolderMailbox: NewPublicFolder@contoso.com`

<span data-ttu-id="43459-175">**Chamadas de pasta pública que exigem os cabeçalhos X-AncorMailbox e X-PublicFolder**</span><span class="sxs-lookup"><span data-stu-id="43459-175">**Public folder calls that require the X-AncorMailbox and X-PublicFolder headers**</span></span>

|<span data-ttu-id="43459-176">**Métodos da API gerenciada do EWS**</span><span class="sxs-lookup"><span data-stu-id="43459-176">**EWS Managed API methods**</span></span>|<span data-ttu-id="43459-177">**Operações do EWS**</span><span class="sxs-lookup"><span data-stu-id="43459-177">**EWS operations**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="43459-178">Item. bind</span><span class="sxs-lookup"><span data-stu-id="43459-178">Item.Bind</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="43459-179">Item. Update</span><span class="sxs-lookup"><span data-stu-id="43459-179">Item.Update</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="43459-180">Item. Copy</span><span class="sxs-lookup"><span data-stu-id="43459-180">Item.Copy</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="43459-181">Item. move</span><span class="sxs-lookup"><span data-stu-id="43459-181">Item.Move</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="43459-182">Item. Delete</span><span class="sxs-lookup"><span data-stu-id="43459-182">Item.Delete</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="43459-183">Folder. bind</span><span class="sxs-lookup"><span data-stu-id="43459-183">Folder.Bind</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="43459-184">Folder. FindItems</span><span class="sxs-lookup"><span data-stu-id="43459-184">Folder.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="43459-185">CreateItem</span><span class="sxs-lookup"><span data-stu-id="43459-185">CreateItem</span></span>](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> [<span data-ttu-id="43459-186">GetItem</span><span class="sxs-lookup"><span data-stu-id="43459-186">GetItem</span></span>](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> [<span data-ttu-id="43459-187">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="43459-187">UpdateItem</span></span>](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> [<span data-ttu-id="43459-188">CopyItem</span><span class="sxs-lookup"><span data-stu-id="43459-188">CopyItem</span></span>](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> [<span data-ttu-id="43459-189">MoveItem</span><span class="sxs-lookup"><span data-stu-id="43459-189">MoveItem</span></span>](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> [<span data-ttu-id="43459-190">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="43459-190">DeleteItem</span></span>](../web-service-reference/deleteitem-operation.md) <br/> [<span data-ttu-id="43459-191">GetFolder</span><span class="sxs-lookup"><span data-stu-id="43459-191">GetFolder</span></span>](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> [<span data-ttu-id="43459-192">FindItem</span><span class="sxs-lookup"><span data-stu-id="43459-192">FindItem</span></span>](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="43459-193">Para adicionar esses cabeçalhos usando a API gerenciada do EWS, use o método [HttpHeaders. Add](https://msdn.microsoft.com/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="43459-193">To add these headers by using the EWS Managed API, use the [HttpHeaders.Add](https://msdn.microsoft.com/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) method.</span></span> 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", "NewPublicFolder@contoso.com");
service.HttpHeaders.Add("X-PublicFolderMailbox", "NewPublicFolder@contoso.com");
```

<span data-ttu-id="43459-194">O código a seguir mostra uma solicitação [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) com o cabeçalho **x-AnchorMailbox** e **x-PublicFolderMailbox** definidos para os valores recuperados nos exemplos deste artigo.</span><span class="sxs-lookup"><span data-stu-id="43459-194">The following code shows a [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) request with the **X-AnchorMailbox** and **X-PublicFolderMailbox** header set to the values retrieved in the examples in this article.</span></span> 
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
User-Agent: SoapSender1.0
X-AnchorMailbox: NewPublicFolder@contoso.com
X-PublicFolderMailbox: NewPublicFolder@contoso.com
Authorization: Basic c29ueWFmQGNvbnRvc28xMDAwLm9ubWljcm9zb2Z0LmNvbTpFWENIIzIwMTQ=
Host: outlook.office365.com
Content-Length: 688
Expect: 100-continue
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </m:FolderShape>
      <m:FolderIds>
        <t:DistinguishedFolderId Id="publicfoldersroot" />
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="43459-195">Confira também</span><span class="sxs-lookup"><span data-stu-id="43459-195">See also</span></span>

- [<span data-ttu-id="43459-196">Acesso a pastas públicas com o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="43459-196">Public folder access with EWS in Exchange</span></span>](public-folder-access-with-ews-in-exchange.md)    
- [<span data-ttu-id="43459-197">Descoberta Automática do Exchange</span><span class="sxs-lookup"><span data-stu-id="43459-197">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md)    
- [<span data-ttu-id="43459-198">Gerar uma lista de pontos de extremidade de Descoberta Automática</span><span class="sxs-lookup"><span data-stu-id="43459-198">Generate a list of Autodiscover endpoints</span></span>](how-to-generate-a-list-of-autodiscover-endpoints.md)   
- [<span data-ttu-id="43459-199">Obter as configurações de usuário do Exchange usando a Descoberta Automática</span><span class="sxs-lookup"><span data-stu-id="43459-199">Get user settings from Exchange by using Autodiscover</span></span>](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
  