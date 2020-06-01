---
title: Gerenciar configurações de aplicativos persistentes usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 90f561f2-e40e-4f5b-b321-f86dbf4a1b71
description: Saiba como criar, localizar, obter, atualizar e excluir configurações de aplicativos persistentes usando a API gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: ab7b3ef5f87d8a26a412ca7187dc93c58d73112f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455727"
---
# <a name="manage-persistent-application-settings-by-using-ews-in-exchange"></a><span data-ttu-id="e489a-103">Gerenciar configurações de aplicativos persistentes usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e489a-103">Manage persistent application settings by using EWS in Exchange</span></span>

<span data-ttu-id="e489a-104">Saiba como criar, localizar, obter, atualizar e excluir configurações de aplicativos persistentes usando a API gerenciada do EWS ou o EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="e489a-104">Learn how to create, find, get, update, and delete persistent application settings by using the EWS Managed API or EWS in Exchange.</span></span> 
  
<span data-ttu-id="e489a-105">Os objetos de configuração do usuário são a melhor opção para armazenar definições de configuração para seu aplicativo de cliente do Exchange, principalmente por estarem ocultos dos resultados da pesquisa na maioria dos aplicativos cliente.</span><span class="sxs-lookup"><span data-stu-id="e489a-105">User configuration objects are the best option for storing configuration settings for your Exchange client application, primarily because they are hidden from search results in most client applications.</span></span> <span data-ttu-id="e489a-106">Os aplicativos clientes normalmente ocultam essas configurações porque o usuário final não precisa vê-las e, portanto, o usuário não acessa acidentalmente essas informações.</span><span class="sxs-lookup"><span data-stu-id="e489a-106">Client applications typically hide these settings because the end user doesn't need to see them, and so that the user doesn't accidentally access this information.</span></span> <span data-ttu-id="e489a-107">Os exemplos de código neste artigo mostram como você pode usar os objetos de configuração do usuário para gerenciar as configurações persistentes, incluindo como criar, localizar, obter, atualizar e excluir as configurações de aplicativo persistente que são armazenadas nos objetos de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="e489a-107">The code examples in this article show you how you can use user configuration objects to manage persistent settings, including how to create, find, get, update, and delete persistent application settings that are stored in user configuration objects.</span></span>

<span data-ttu-id="e489a-108"><a name="createconfiguration"> </a></span><span class="sxs-lookup"><span data-stu-id="e489a-108"><a name="createconfiguration"> </a></span></span>

## <a name="create-an-application-setting-by-using-the-ews-managed-api"></a><span data-ttu-id="e489a-109">Criar uma configuração de aplicativo usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="e489a-109">Create an application setting by using the EWS Managed API</span></span>

<span data-ttu-id="e489a-110">Você pode usar o método [userconfiguration. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.save%28v=exchg.80%29.aspx) do EWS Managed API para criar uma configuração personalizada.</span><span class="sxs-lookup"><span data-stu-id="e489a-110">You can use the [UserConfiguration.Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.save%28v=exchg.80%29.aspx) EWS Managed API method to create a custom configuration setting.</span></span> <span data-ttu-id="e489a-111">Um objeto de configuração do usuário pode conter XML, binário, um dicionário de dados ou uma combinação desses três tipos de dados.</span><span class="sxs-lookup"><span data-stu-id="e489a-111">A user configuration object can contain XML, binary, a data dictionary, or a combination of those three data types.</span></span> <span data-ttu-id="e489a-112">O exemplo a seguir mostra como salvar um objeto de configuração do usuário chamado ContosoDraftSettings que contém dados binários na pasta Rascunhos usando a API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="e489a-112">The following example shows how to save a user configuration object named ContosoDraftSettings that contains binary data to your Drafts folder by using the EWS Managed API.</span></span> <span data-ttu-id="e489a-113">Isso pode ser útil se você quiser armazenar informações de configuração sobre como os itens de rascunho são exibidos no aplicativo cliente.</span><span class="sxs-lookup"><span data-stu-id="e489a-113">This might be useful if you want to store configuration information about how draft items are displayed in your client application.</span></span> 
  
```cs
private static void CreateUserConfiguration(ExchangeService service, byte[] binaryData)
{
    // Create the user configuration object.
    UserConfiguration configDrafts = new UserConfiguration(service);
    // Add user configuration data to the BinaryData property.
    configDrafts.BinaryData = binaryData;
    // Name and save the user configuration object on the Drafts folder.
    // This results in a call to EWS.
    configDrafts.Save("ContosoDraftSettings", WellKnownFolderName.Drafts);
}
```

## <a name="create-an-application-setting-by-using-ews"></a><span data-ttu-id="e489a-114">Criar uma configuração de aplicativo usando o EWS</span><span class="sxs-lookup"><span data-stu-id="e489a-114">Create an application setting by using EWS</span></span>
<span data-ttu-id="e489a-115"><a name="bk_createEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="e489a-115"><a name="bk_createEWS"> </a></span></span>

<span data-ttu-id="e489a-116">Você pode usar a operação [CreateUserConfiguration](https://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) EWS para criar uma configuração personalizada.</span><span class="sxs-lookup"><span data-stu-id="e489a-116">You can use the [CreateUserConfiguration](https://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) EWS operation to create a custom configuration setting.</span></span> <span data-ttu-id="e489a-117">O exemplo a seguir mostra a solicitação de XML para a criação de um objeto de configuração do usuário chamado ContosoDraftSettings.</span><span class="sxs-lookup"><span data-stu-id="e489a-117">The following example shows the request XML for creating a user configuration object named ContosoDraftSettings.</span></span> <span data-ttu-id="e489a-118">A solicitação tenta salvar um fluxo binário em um objeto de configuração do usuário na pasta Rascunhos.</span><span class="sxs-lookup"><span data-stu-id="e489a-118">The request attempts to save a binary stream to a user configuration object on the Drafts folder.</span></span> <span data-ttu-id="e489a-119">Este é o mesmo XML que é gerado pelo exemplo de API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="e489a-119">This is the same XML that is generated by the EWS Managed API example.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:CreateUserConfiguration>
      <m:UserConfiguration>
        <t:UserConfigurationName Name="ContosoDraftSettings">
          <t:DistinguishedFolderId Id="drafts" />
        </t:UserConfigurationName>
        <t:BinaryData>iVBORw0KGH5UhKquRSzaeAAAAAElFTkSuQmCC</t:BinaryData>
      </m:UserConfiguration>
    </m:CreateUserConfiguration>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="e489a-120">O [XML de resposta](https://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) é simples e indica se a solicitação de criação foi bem-sucedida ou se ocorreu um erro.</span><span class="sxs-lookup"><span data-stu-id="e489a-120">The [response XML](https://msdn.microsoft.com/library/eb5b8ab6-9743-481c-aac9-f9aa889bd353%28Office.15%29.aspx) is simple and indicates whether the create request was successful or whether an error occurred.</span></span> 
  
## <a name="find-an-application-setting-by-using-the-ews-managed-api"></a><span data-ttu-id="e489a-121">Localizar uma configuração de aplicativo usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="e489a-121">Find an application setting by using the EWS Managed API</span></span>
<span data-ttu-id="e489a-122"><a name="findconfiguration"> </a></span><span class="sxs-lookup"><span data-stu-id="e489a-122"><a name="findconfiguration"> </a></span></span>

<span data-ttu-id="e489a-123">Você pode usar o método [Folder. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) EWS Managed API com a opção transversal associada para localizar objetos de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="e489a-123">You can use the [Folder.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) EWS Managed API method with the associated traversal option to find user configuration objects.</span></span> <span data-ttu-id="e489a-124">O exemplo de código a seguir mostra como localizar objetos de configuração do usuário armazenados na pasta Rascunhos usando a API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="e489a-124">The following code example shows you how to find user configuration objects stored on the Drafts folder by using the EWS Managed API.</span></span> 
  
```cs
private static void FindAssociated(ExchangeService service)
{
    // This is the ItemClass prefix of user configuration objects that are created by using EWS.
    const string userConfigPrefix = "IPM.Configuration.";
            
    // This is the name of a configuration setting created by using EWS.
    string userConfigName = "TestConfig";
    // Return the first five items. 
    ItemView view = new ItemView(5);
    // Request only the properties that you need. Because all the results will be user configuration 
    // objects, you won't need to request the ItemSchema.IsAssociated property, which identifies 
    // user configuration objects.
    PropertySet props = new PropertySet(BasePropertySet.IdOnly, 
                                        ItemSchema.ItemClass);
    view.PropertySet = props;
            
    // Set the traversal to find user configuration objects. 
    view.Traversal = ItemTraversal.Associated;
    // Send the request to search the Drafts folder for all the user configuration objects 
    // in the folder. You do not have to use a search restriction because you will not return
    // a large number of search results. For this scenario, it is better to sort the results
    // on the client. This method results in a call to EWS.
    FindItemsResults<Item> findResults = service.FindItems(WellKnownFolderName.Drafts, view);
    // Output a list of the item classes for the associated items. 
    foreach (Item item in findResults)
    {
        if (item.ItemClass == userConfigPrefix + userConfigName)
        {
            Console.WriteLine("You found the configuration: " + userConfigPrefix + userConfigName);
        }
    }
}
```

## <a name="find-an-application-setting-by-using-ews"></a><span data-ttu-id="e489a-125">Localizar uma configuração de aplicativo usando o EWS</span><span class="sxs-lookup"><span data-stu-id="e489a-125">Find an application setting by using EWS</span></span>
<span data-ttu-id="e489a-126"><a name="bk_findEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="e489a-126"><a name="bk_findEWS"> </a></span></span>

<span data-ttu-id="e489a-127">Você pode usar a operação [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) EWS para localizar objetos de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="e489a-127">You can use the [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) EWS operation to find user configuration objects.</span></span> 
  
<span data-ttu-id="e489a-128">O exemplo a seguir mostra a solicitação de XML para localizar objetos de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="e489a-128">The following example shows the request XML for finding user configuration objects.</span></span> <span data-ttu-id="e489a-129">Este é o mesmo XML que é gerado pelo exemplo de API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="e489a-129">This is the same XML that is generated by the EWS Managed API example.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Associated">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:ItemClass" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="5" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="drafts" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="e489a-130">O exemplo a seguir mostra o XML de resposta bem-sucedido para localizar objetos de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="e489a-130">The following example shows the successful response XML for finding user configuration objects.</span></span> <span data-ttu-id="e489a-131">Este é o mesmo XML processado pelo exemplo de API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="e489a-131">This is the same XML that is processed by the EWS Managed API example.</span></span> <span data-ttu-id="e489a-132">Observe o seguinte neste XML de resposta:</span><span class="sxs-lookup"><span data-stu-id="e489a-132">Note the following in this response XML:</span></span> 
  
- <span data-ttu-id="e489a-133">Reduzimos o identificador e alteramos as chaves para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="e489a-133">We shortened the identifier and change keys for readability.</span></span>
    
- <span data-ttu-id="e489a-134">Os dois objetos de configuração do usuário são retornados como mensagens.</span><span class="sxs-lookup"><span data-stu-id="e489a-134">The two user configuration objects are returned as messages.</span></span> <span data-ttu-id="e489a-135">Isso ocorre porque a operação **FindItem** retorna todos os itens que não estão definidos no esquema do EWS como itens de mensagem.</span><span class="sxs-lookup"><span data-stu-id="e489a-135">This is because the **FindItem** operation returns all items that are not defined in the EWS schema as message items.</span></span> 
    
- <span data-ttu-id="e489a-136">As propriedades de @ [Class](https://msdn.microsoft.com/library/56020078-50b4-4880-894a-a9f234033cfb%28Office.15%29.aspx) para os dois objetos de configuração do usuário são diferentes.</span><span class="sxs-lookup"><span data-stu-id="e489a-136">The [ItemClass](https://msdn.microsoft.com/library/56020078-50b4-4880-894a-a9f234033cfb%28Office.15%29.aspx) properties for the two user configuration objects are different.</span></span> <span data-ttu-id="e489a-137">O primeiro objeto de configuração do usuário foi criado usando o EWS.</span><span class="sxs-lookup"><span data-stu-id="e489a-137">The first user configuration object was created by using EWS.</span></span> <span data-ttu-id="e489a-138">O segundo objeto foi criado por outra API.</span><span class="sxs-lookup"><span data-stu-id="e489a-138">The second object was created by another API.</span></span> 
    
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="800" 
                         MinorBuildNumber="5" 
                         Version="V2_6" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="2" 
                        TotalItemsInView="2" 
                        IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkDEY9M6AAA=" ChangeKey="CQAAACYnYF5aFMwP0T" />
                <t:ItemClass>IPM.Configuration.TestConfig</t:ItemClass>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAkADEzOzFAAA=" ChangeKey="CQAAABQAAABAByOw==" />
                <t:ItemClass>IPM.Microsoft.FolderDesign.NamedView</t:ItemClass>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="get-and-update-application-settings-by-using-the-ews-managed-api"></a><span data-ttu-id="e489a-139">Obter e atualizar as configurações de aplicativo usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="e489a-139">Get and update application settings by using the EWS Managed API</span></span>
<span data-ttu-id="e489a-140"><a name="getconfiguration"> </a></span><span class="sxs-lookup"><span data-stu-id="e489a-140"><a name="getconfiguration"> </a></span></span>

<span data-ttu-id="e489a-141">Depois de encontrar um objeto de configuração do usuário, você pode usar o método [userconfiguration. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) da API gerenciada do EWS para obter o objeto de configuração da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e489a-141">After you find a user configuration object, you can use the [UserConfiguration.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) EWS Managed API method to get the configuration object from the mailbox.</span></span> <span data-ttu-id="e489a-142">Depois de obter o objeto de configuração, você pode usar o método [userconfiguration. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) para atualizá-lo.</span><span class="sxs-lookup"><span data-stu-id="e489a-142">After you get the configuration object, you can use the [UserConfiguration.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.bind%28v=exchg.80%29.aspx) method to update it.</span></span> <span data-ttu-id="e489a-143">O exemplo a seguir mostra como obter e atualizar um objeto de configuração do usuário usando a API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="e489a-143">The following example shows how to get and update a user configuration object by using the EWS Managed API.</span></span> 
  
```cs
private static void GetAndUpdateUserConfiguration(ExchangeService service)
{
    // Binds to a user configuration object named "TestConfig" in the user's mailbox. 
    // Results in a call to EWS. You can also use the Load method to get the latest
    // server version of the user configuration object.
    UserConfiguration usrConfig = UserConfiguration.Bind(service,
                                                         "TestConfig",
                                                         WellKnownFolderName.Drafts,
                                                         UserConfigurationProperties.All);
            
    // Display the returned configuration object property values.
    if (usrConfig.XmlData != null)
    {
        Console.WriteLine("XmlData: " + Encoding.UTF8.GetString(usrConfig.XmlData));
    }
    if (usrConfig.BinaryData != null)
    {
        Console.WriteLine("BinaryData: " + Encoding.UTF8.GetString(usrConfig.BinaryData));
    }
    if (usrConfig.Dictionary.Count > 0)
    {
        Console.WriteLine("Contains {0} dictionary entries", usrConfig.Dictionary.Count);
    }
    // Add dictionary property values to the local copy of the object.
    usrConfig.Dictionary.Add("Key5", 1);
    // Updates the server version of the user configuration object 
    // if it has changed on the client. Results in a call to EWS.
    if (usrConfig.IsDirty)
    {
        usrConfig.Update();
    }
}
```

## <a name="get-and-update-application-settings-by-using-ews"></a><span data-ttu-id="e489a-144">Obter e atualizar as configurações de aplicativo usando o EWS</span><span class="sxs-lookup"><span data-stu-id="e489a-144">Get and update application settings by using EWS</span></span>
<span data-ttu-id="e489a-145"><a name="bk_getEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="e489a-145"><a name="bk_getEWS"> </a></span></span>

<span data-ttu-id="e489a-146">Você pode usar a operação [GetUserConfiguration](https://msdn.microsoft.com/library/71d50e3c-92bd-435f-8118-b28bb85f8138%28Office.15%29.aspx) EWS para recuperar o objeto de configuração da caixa de correio e o [UpdateUserConfiguration](https://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx) para atualizar o objeto.</span><span class="sxs-lookup"><span data-stu-id="e489a-146">You can use the [GetUserConfiguration](https://msdn.microsoft.com/library/71d50e3c-92bd-435f-8118-b28bb85f8138%28Office.15%29.aspx) EWS operation to retrieve the configuration object from the mailbox, and the [UpdateUserConfiguration](https://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx) to update the object.</span></span> <span data-ttu-id="e489a-147">O exemplo a seguir mostra o XML da solicitação para obter um objeto de configuração do usuário chamado TestConfig.</span><span class="sxs-lookup"><span data-stu-id="e489a-147">The following example shows the request XML for getting a user configuration object named TestConfig.</span></span> <span data-ttu-id="e489a-148">A solicitação afirma que todas as configurações devem ser retornadas na resposta.</span><span class="sxs-lookup"><span data-stu-id="e489a-148">The request states that all configurations should be returned in the response.</span></span> <span data-ttu-id="e489a-149">Este é o mesmo XML que é gerado pelo exemplo de API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="e489a-149">This is the same XML that is generated by the EWS Managed API example.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:GetUserConfiguration>
      <m:UserConfigurationName Name="TestConfig">
        <t:DistinguishedFolderId Id="drafts" />
      </m:UserConfigurationName>
      <m:UserConfigurationProperties>All</m:UserConfigurationProperties>
    </m:GetUserConfiguration>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="e489a-150">O exemplo a seguir mostra o XML de resposta bem-sucedido para obter os objetos de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="e489a-150">The following example shows the successful response XML for getting a user configuration objects.</span></span> <span data-ttu-id="e489a-151">A resposta contém um dicionário de dados.</span><span class="sxs-lookup"><span data-stu-id="e489a-151">The response contains a data dictionary.</span></span> <span data-ttu-id="e489a-152">Este é o mesmo XML processado pelo exemplo de API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="e489a-152">This is the same XML that is processed by the EWS Managed API example.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="800" 
                         MinorBuildNumber="5" 
                         Version="V2_6" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetUserConfigurationResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetUserConfigurationResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:UserConfiguration>
            <t:UserConfigurationName Name="TestConfig">
              <t:DistinguishedFolderId Id="drafts" />
            </t:UserConfigurationName>
            <t:ItemId Id="AAMkDEY9M6AAA=" ChangeKey="CQAAACYnYF5aFMwP0T" />
            <t:Dictionary>
              <t:DictionaryEntry>
                <t:DictionaryKey>
                  <t:Type>String</t:Type>
                  <t:Value>Key1</t:Value>
                </t:DictionaryKey>
                <t:DictionaryValue>
                  <t:Type>Integer32</t:Type>
                  <t:Value>1</t:Value>
                </t:DictionaryValue>
              </t:DictionaryEntry>
              <t:DictionaryEntry>
                <t:DictionaryKey>
                  <t:Type>String</t:Type>
                  <t:Value>PhoneNumber</t:Value>
                </t:DictionaryKey>
                <t:DictionaryValue>
                  <t:Type>String</t:Type>
                  <t:Value>555-555-1111</t:Value>
                </t:DictionaryValue>
              </t:DictionaryEntry>
            </t:Dictionary>
          </m:UserConfiguration>
        </m:GetUserConfigurationResponseMessage>
      </m:ResponseMessages>
    </m:GetUserConfigurationResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="e489a-153">O exemplo a seguir mostra a solicitação de XML para atualização de um objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="e489a-153">The following example shows the request XML for updating a user configuration object.</span></span> <span data-ttu-id="e489a-154">A solicitação afirma que todas as configurações devem ser retornadas na resposta.</span><span class="sxs-lookup"><span data-stu-id="e489a-154">The request states that all configurations should be returned in the response.</span></span> <span data-ttu-id="e489a-155">Este é o mesmo XML que é gerado pelo exemplo de API gerenciada do EWS que chama o método **userconfiguration. Update** .</span><span class="sxs-lookup"><span data-stu-id="e489a-155">This is the same XML that is generated by the EWS Managed API example that calls the **UserConfiguration.Update** method.</span></span> <span data-ttu-id="e489a-156">Você pode ver que o XML de atualização contém as entradas de dicionário existentes e outra que foi adicionada antes da atualização.</span><span class="sxs-lookup"><span data-stu-id="e489a-156">You can see that the update XML contains the existing dictionary entries and the additional one that was added before the update.</span></span> 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:UpdateUserConfiguration>
      <m:UserConfiguration>
        <t:UserConfigurationName Name="TestConfig">
          <t:DistinguishedFolderId Id="drafts" />
        </t:UserConfigurationName>
        <t:Dictionary>
          <t:DictionaryEntry>
            <t:DictionaryKey>
              <t:Type>String</t:Type>
              <t:Value>Key1</t:Value>
            </t:DictionaryKey>
            <t:DictionaryValue>
              <t:Type>Integer32</t:Type>
              <t:Value>1</t:Value>
            </t:DictionaryValue>
          </t:DictionaryEntry>
          <t:DictionaryEntry>
            <t:DictionaryKey>
              <t:Type>String</t:Type>
              <t:Value>PhoneNumber</t:Value>
            </t:DictionaryKey>
            <t:DictionaryValue>
              <t:Type>String</t:Type>
              <t:Value>555-555-1111</t:Value>
            </t:DictionaryValue>
          </t:DictionaryEntry>
          <t:DictionaryEntry>
            <t:DictionaryKey>
              <t:Type>String</t:Type>
              <t:Value>Key5</t:Value>
            </t:DictionaryKey>
            <t:DictionaryValue>
              <t:Type>Integer32</t:Type>
              <t:Value>1</t:Value>
            </t:DictionaryValue>
          </t:DictionaryEntry>
        </t:Dictionary>
      </m:UserConfiguration>
    </m:UpdateUserConfiguration>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="e489a-157">O [XML de resposta](https://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx) é simples e indica se a atualização foi bem-sucedida ou se ocorreu um erro.</span><span class="sxs-lookup"><span data-stu-id="e489a-157">The [response XML](https://msdn.microsoft.com/library/eda73b62-6a3a-43ae-8fd9-f30892811f27%28Office.15%29.aspx) is simple and indicates whether the update was successful or whether an error occurred.</span></span> 
  
## <a name="delete-an-application-setting-by-using-the-ews-managed-api"></a><span data-ttu-id="e489a-158">Excluir uma configuração de aplicativo usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="e489a-158">Delete an application setting by using the EWS Managed API</span></span>
<span data-ttu-id="e489a-159"><a name="deleteconfiguration"> </a></span><span class="sxs-lookup"><span data-stu-id="e489a-159"><a name="deleteconfiguration"> </a></span></span>

<span data-ttu-id="e489a-160">Você pode usar o método [userconfiguration. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) EWS Managed API para excluir os objetos de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="e489a-160">You can use the [UserConfiguration.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.userconfiguration.delete%28v=exchg.80%29.aspx) EWS Managed API method to delete user configuration objects.</span></span> <span data-ttu-id="e489a-161">O exemplo de código a seguir mostra como excluir o objeto de configuração do usuário ContosoDraftSettings usando a API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="e489a-161">The following code example shows you how to delete the ContosoDraftSettings user configuration object by using the EWS Managed API.</span></span> 
  
```cs
private static void DeleteUserConfiguration(ExchangeService service)
{
    // Binds to a user configuration object. Results in a call to EWS.
    UserConfiguration usrConfig = UserConfiguration.Bind(service,
                                                        "ContosoDraftSettings",
                                                        WellKnownFolderName.Drafts,
                                                        UserConfigurationProperties.Id);
    // Deletes the user configuration object.
    // Results in a call to EWS.
    usrConfig.Delete();
}
```

## <a name="delete-an-application-setting-by-using-ews"></a><span data-ttu-id="e489a-162">Excluir uma configuração de aplicativo usando o EWS</span><span class="sxs-lookup"><span data-stu-id="e489a-162">Delete an application setting by using EWS</span></span>
<span data-ttu-id="e489a-163"><a name="bk_deleteEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="e489a-163"><a name="bk_deleteEWS"> </a></span></span>

<span data-ttu-id="e489a-164">Você pode usar a operação [DeleteUserConfiguration](https://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) EWS para excluir objetos de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="e489a-164">You can use the [DeleteUserConfiguration](https://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) EWS operation to delete user configuration objects.</span></span> 
  
<span data-ttu-id="e489a-165">O exemplo a seguir mostra o XML da solicitação para excluir um objeto de configuração do usuário chamado ContosoDraftSettings que foi aplicado à pasta Rascunhos.</span><span class="sxs-lookup"><span data-stu-id="e489a-165">The following example shows the request XML for deleting a user configuration object named ContosoDraftSettings that was applied to the Drafts folder.</span></span> <span data-ttu-id="e489a-166">Este é o mesmo XML que é gerado pelo exemplo de API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="e489a-166">This is the same XML that is generated by the EWS Managed API example.</span></span>
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:DeleteUserConfiguration>
      <m:UserConfigurationName Name="ContosoDraftSettings">
        <t:DistinguishedFolderId Id="drafts" />
      </m:UserConfigurationName>
    </m:DeleteUserConfiguration>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="e489a-167">O [XML de resposta](https://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) é simples e indica se a solicitação de exclusão foi bem-sucedida ou se ocorreu um erro.</span><span class="sxs-lookup"><span data-stu-id="e489a-167">The [response XML](https://msdn.microsoft.com/library/93e44690-be2d-4fdb-96a8-4ded3c193aed%28Office.15%29.aspx) is simple and indicates whether the delete request was a success or whether an error occurred.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="e489a-168">Também consulte</span><span class="sxs-lookup"><span data-stu-id="e489a-168">See also</span></span>

- [<span data-ttu-id="e489a-169">Configurações de aplicativo persistente no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e489a-169">Persistent application settings in EWS in Exchange</span></span>](persistent-application-settings-in-ews-in-exchange.md)
- [<span data-ttu-id="e489a-170">Visão geral do design de cliente do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="e489a-170">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)   
- [<span data-ttu-id="e489a-171">Develop web service clients for Exchange</span><span class="sxs-lookup"><span data-stu-id="e489a-171">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    

