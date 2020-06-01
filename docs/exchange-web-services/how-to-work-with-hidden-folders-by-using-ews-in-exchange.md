---
title: Trabalhar com pastas ocultas usando o EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7ae7c045-cd90-4c9f-baf5-0464d5058f45
description: Saiba como tornar uma pasta oculta e localizar pastas ocultas usando a API gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: d4fa44a0399542350668359e8abb88d2a0a9d579
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456371"
---
# <a name="work-with-hidden-folders-by-using-ews-in-exchange"></a><span data-ttu-id="10b2b-103">Trabalhar com pastas ocultas usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="10b2b-103">Work with hidden folders by using EWS in Exchange</span></span>

<span data-ttu-id="10b2b-104">Saiba como tornar uma pasta oculta e localizar pastas ocultas usando a API gerenciada do EWS ou o EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="10b2b-104">Learn how to make a folder hidden and find hidden folders by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="10b2b-105">Com uma exceção, as pastas na raiz de uma caixa de correio do Exchange (a sub-árvore não-IPM) ficam ocultas do usuário.</span><span class="sxs-lookup"><span data-stu-id="10b2b-105">With one exception, folders in the root of an Exchange mailbox (the non-IPM subtree) are hidden from the user.</span></span> <span data-ttu-id="10b2b-106">Por outro lado, todas as pastas no **MsgFolderRoot** (a sub-árvore IPM) são visíveis para o usuário.</span><span class="sxs-lookup"><span data-stu-id="10b2b-106">Conversely, all folders in the **MsgFolderRoot** (the IPM subtree) are visible to the user.</span></span> <span data-ttu-id="10b2b-107">Então, como você oculta uma pasta no **MsgFolderRoot**?</span><span class="sxs-lookup"><span data-stu-id="10b2b-107">So how do you hide a folder under the **MsgFolderRoot**?</span></span> <span data-ttu-id="10b2b-108">Não é tão complicado – ele é direcionado para apenas uma propriedade, a propriedade estendida [PidTagAttributeHidden](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx) (0x10F4000B).</span><span class="sxs-lookup"><span data-stu-id="10b2b-108">It's not that tricky — it comes down to just one property, the [PidTagAttributeHidden](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx) (0x10F4000B) extended property.</span></span> <span data-ttu-id="10b2b-109">Quando essa propriedade é definida como **true**, o Outlook ou outro cliente que usa a propriedade para determinar a visibilidade da pasta ocultará a pasta do modo de exibição do usuário.</span><span class="sxs-lookup"><span data-stu-id="10b2b-109">When this property is set to **true**, Outlook or another client that uses the property to determine folder visibility will hide the folder from the user's view.</span></span> <span data-ttu-id="10b2b-110">Como esta é uma propriedade estendida, é mais complexo usar que a propriedade de pasta média, portanto, este artigo orientará você pelos principais cenários.</span><span class="sxs-lookup"><span data-stu-id="10b2b-110">Because this is an extended property, it's more complex to use than your average folder property, so this article will walk you through the main scenarios.</span></span>
  
<span data-ttu-id="10b2b-111">**Tabela 1. Métodos da API gerenciada do EWS e operações do EWS para trabalhar com pastas ocultas**</span><span class="sxs-lookup"><span data-stu-id="10b2b-111">**Table 1. EWS Managed API methods and EWS operations for working with hidden folders**</span></span>

|<span data-ttu-id="10b2b-112">**Tarefa**</span><span class="sxs-lookup"><span data-stu-id="10b2b-112">**Task**</span></span>|<span data-ttu-id="10b2b-113">**Método de API gerenciada do EWS**</span><span class="sxs-lookup"><span data-stu-id="10b2b-113">**EWS Managed API method**</span></span>|<span data-ttu-id="10b2b-114">**Operação do EWS**</span><span class="sxs-lookup"><span data-stu-id="10b2b-114">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="10b2b-115">Ocultar uma pasta</span><span class="sxs-lookup"><span data-stu-id="10b2b-115">Hide a folder</span></span>  <br/> |<span data-ttu-id="10b2b-116">[Folder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) seguido por [Folder. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="10b2b-116">[Folder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) followed by [Folder.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="10b2b-117">[GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) seguido por [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="10b2b-117">[GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) followed by [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="10b2b-118">Localizar pastas ocultas</span><span class="sxs-lookup"><span data-stu-id="10b2b-118">Find hidden folders</span></span>  <br/> |[<span data-ttu-id="10b2b-119">FindFolders</span><span class="sxs-lookup"><span data-stu-id="10b2b-119">FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="10b2b-120">FindFolder</span><span class="sxs-lookup"><span data-stu-id="10b2b-120">FindFolder</span></span>](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="10b2b-121">Você está se perguntando o que é a única exceção, ou seja, qual pasta na raiz é visível para os usuários?</span><span class="sxs-lookup"><span data-stu-id="10b2b-121">Are you wondering what the one exception is — that is, what folder in the root IS visible to users?</span></span> <span data-ttu-id="10b2b-122">É a pasta Finder (também conhecida como o valor de enumeração **SearchFolders**[WellKnownFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) ou o valor do elemento **SearchFolders**[DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) ), que contém as pastas de pesquisa dos usuários.</span><span class="sxs-lookup"><span data-stu-id="10b2b-122">It's the Finder folder (also known as the **SearchFolders**[WellKnownFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) enumeration value, or the **searchfolders**[DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) element value), which contains users' search folders.</span></span> <span data-ttu-id="10b2b-123">As pastas de pesquisa criadas na pasta localizador são visíveis para os usuários do Outlook.</span><span class="sxs-lookup"><span data-stu-id="10b2b-123">Search folders created in the Finder folder are visible to Outlook users.</span></span> <span data-ttu-id="10b2b-124">Se você precisar criar uma pasta de pesquisa que não é visível para os usuários, mova-a na pasta raiz para ocultá-la.</span><span class="sxs-lookup"><span data-stu-id="10b2b-124">If you need to create a search folder that is not visible to users, move it under the root folder to hide it.</span></span> <span data-ttu-id="10b2b-125">Diferentemente de outras pastas, a definição da propriedade **PidTagAttributeHidden** como **true** não ocultará uma pasta de pesquisa na pasta Finder.</span><span class="sxs-lookup"><span data-stu-id="10b2b-125">Unlike for other folders, setting the **PidTagAttributeHidden** property to **true** will not hide a search folder in the Finder folder.</span></span> 
  
## <a name="hide-a-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="10b2b-126">Ocultar uma pasta usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="10b2b-126">Hide a folder by using the EWS Managed API</span></span>
<span data-ttu-id="10b2b-127"><a name="bk_hideewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="10b2b-127"><a name="bk_hideewsma"> </a></span></span>

<span data-ttu-id="10b2b-128">Você pode [tornar uma pasta existente](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_createfolderewsma) uma pasta oculta alterando a propriedade estendida [PidTagAttributeHidden](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx) para **true**.</span><span class="sxs-lookup"><span data-stu-id="10b2b-128">You can [make an existing folder](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_createfolderewsma) a hidden folder by changing the [PidTagAttributeHidden](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx) extended property to **true**.</span></span> <span data-ttu-id="10b2b-129">Primeiro, crie uma [definição de propriedade estendida para a propriedade](properties-and-extended-properties-in-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="10b2b-129">First, create an [extended property definition for the property](properties-and-extended-properties-in-ews-in-exchange.md).</span></span> <span data-ttu-id="10b2b-130">Em seguida, use o método [BIND](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) para obter a pasta, atualize o valor da propriedade **PidTagAttributeHidden** para true e use o método [Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) para salvar as alterações.</span><span class="sxs-lookup"><span data-stu-id="10b2b-130">Next, use the [Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) method to get to the folder, then update the value of the **PidTagAttributeHidden** property to true, and use the [Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) method to save the changes.</span></span> 
  
<span data-ttu-id="10b2b-131">Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido para o proprietário da caixa de correio, que o usuário foi autenticado em um servidor Exchange e que **FolderId** é uma [Folder.ID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) válida que identifica a pasta a ser ocultada.</span><span class="sxs-lookup"><span data-stu-id="10b2b-131">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox owner, that the user has been authenticated to an Exchange server, and that **folderId** is a valid [Folder.Id](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) that identifies the folder to hide.</span></span> 
  
```cs
private static void MakeHidden(FolderId folderId, ExchangeService service)
{
    // Create an extended property definition for the PidTagAttributeHidden property.
    ExtendedPropertyDefinition isHiddenProp = new ExtendedPropertyDefinition(0x10f4, MapiPropertyType.Boolean);
    PropertySet propSet = new PropertySet(isHiddenProp);
    // Bind to a folder and retrieve the PidTagAttributeHidden property.
    Folder folder = Folder.Bind(service, folderId, propSet);
    // Set the PidTagAttributeHidden property to true.
    folder.SetExtendedProperty(isHiddenProp, true);
    // Save the changes.
    folder.Update();
}
```

## <a name="hide-a-folder-by-using-ews"></a><span data-ttu-id="10b2b-132">Ocultar uma pasta usando o EWS</span><span class="sxs-lookup"><span data-stu-id="10b2b-132">Hide a folder by using EWS</span></span>
<span data-ttu-id="10b2b-133"><a name="bk_hideews"> </a></span><span class="sxs-lookup"><span data-stu-id="10b2b-133"><a name="bk_hideews"> </a></span></span>

<span data-ttu-id="10b2b-134">Você pode usar o EWS para [tornar uma pasta existente](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_createfolderewsma) uma pasta oculta alterando a propriedade estendida [PidTagAttributeHidden](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx) para **true**.</span><span class="sxs-lookup"><span data-stu-id="10b2b-134">You can use EWS to [make an existing folder](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_createfolderewsma) a hidden folder by changing the [PidTagAttributeHidden](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx) extended property to **true**.</span></span> <span data-ttu-id="10b2b-135">Primeiro, use a operação [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) para acessar a pasta e, em seguida, recuperar a propriedade **PidTagAttributeHidden** incluindo o elemento [ExtendedFieldURI](https://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) e definindo o valor de **PropertyTag** como 4340 e o valor **recordtypepropriedade** como Boolean.</span><span class="sxs-lookup"><span data-stu-id="10b2b-135">First, use the [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) operation to get to the folder, then retrieve the **PidTagAttributeHidden** property by including the [ExtendedFieldURI](https://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) element, and setting the **PropertyTag** value to 4340 and the **PropertyType** value to Boolean.</span></span> 
  
<span data-ttu-id="10b2b-136">Essa é também a solicitação XML que a API gerenciada do EWS envia quando você usa o método **BIND** para obter uma pasta antes [de torná-la uma pasta oculta](#bk_hideewsma).</span><span class="sxs-lookup"><span data-stu-id="10b2b-136">This is also the XML request that the EWS Managed API sends when you use the **Bind** method to get a folder before [making it a hidden folder](#bk_hideewsma).</span></span>
  
<span data-ttu-id="10b2b-137">O valor [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) é reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="10b2b-137">The [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) value is shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:ExtendedFieldURI PropertyTag="4340"
                              PropertyType="Boolean" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:FolderIds>
        <t:FolderId Id="IQywAAAA==" />
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

O servidor responde à solicitação **GetFolder** com uma mensagem [GetFolderResponse](https://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) que inclui um valor de elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica que a pasta foi recuperada com êxito. A resposta também inclui um [valor](https://msdn.microsoft.com/library/196278d4-5e77-4e0a-8af6-8ac065610510%28Office.15%29.aspx) para a [extensão estendida](https://msdn.microsoft.com/library/f9701409-b620-4afe-b9ee-4c1e95507af7%28Office.15%29.aspx). <span data-ttu-id="10b2b-140">Neste exemplo, o **valor** é definido como **false**, o que significa que a pasta não está oculta no momento.</span><span class="sxs-lookup"><span data-stu-id="10b2b-140">In this example, the **Value** is set to **false**, which means that the folder is currently not hidden.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="898"
                         MinorBuildNumber="23"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="IQywAAAA=="
                          ChangeKey="AQAAABYAAAD32nSTjepyT63rYH17n9THAAAAABED" />
              <t:ExtendedProperty>
                <t:ExtendedFieldURI PropertyTag="0x10f4"
                                    PropertyType="Boolean" />
                <t:Value>false</t:Value>
              </t:ExtendedProperty>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="10b2b-141">Para alterar o valor de **Extended** para true, use a operação [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="10b2b-141">To change the value of the **ExtendedProperty** to true, use the [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="10b2b-142">Inclua os elementos **Extended**, **ExtendedFieldURI**e **Value** para a propriedade estendida **PidTagAttributeHidden** e defina o elemento **Value** como **true** para ocultar a pasta.</span><span class="sxs-lookup"><span data-stu-id="10b2b-142">Include the **ExtendedProperty**, **ExtendedFieldURI**, and **Value** elements for the **PidTagAttributeHidden** extended property, and set the **Value** element to **true** to hide the folder.</span></span> 
  
<span data-ttu-id="10b2b-143">Essa é também a solicitação XML que a API gerenciada do EWS envia quando você usa o método **Update** para atualizar uma pasta para [torná-la uma pasta oculta](#bk_hideewsma).</span><span class="sxs-lookup"><span data-stu-id="10b2b-143">This is also the XML request that the EWS Managed API sends when you use the **Update** method to update a folder to [make it a hidden folder](#bk_hideewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateFolder>
      <m:FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="IQywAAAA=="
                      ChangeKey="AQAAABYAAAD32nSTjepyT63rYH17n9THAAAAABED" />
          <t:Updates>
            <t:SetFolderField>
              <t:ExtendedFieldURI PropertyTag="4340"
                                  PropertyType="Boolean" />
              <t:Folder>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="4340"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="10b2b-144">O servidor responde à solicitação **UpdateFolder** com uma mensagem [UpdateFolderResponse](https://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) que inclui um valor de elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica que a pasta foi atualizada com êxito e que agora está oculta.</span><span class="sxs-lookup"><span data-stu-id="10b2b-144">The server responds to the **UpdateFolder** request with an [UpdateFolderResponse](https://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the folder was updated successfully, and is now hidden.</span></span>
  
## <a name="find-all-hidden-folders-by-using-the-ews-managed-api"></a><span data-ttu-id="10b2b-145">Localizar todas as pastas ocultas usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="10b2b-145">Find all hidden folders by using the EWS Managed API</span></span>
<span data-ttu-id="10b2b-146"><a name="bk_findhiddenewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="10b2b-146"><a name="bk_findhiddenewsma"> </a></span></span>

<span data-ttu-id="10b2b-147">Você pode localizar todas as pastas ocultas em uma pasta pai criando [uma definição de propriedade estendida](properties-and-extended-properties-in-ews-in-exchange.md) para a propriedade estendida **PidTagAttributeHidden** e, em seguida, usando o método [FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) para localizar pastas com um valor de **PidTagAttributeHidden** que é definido como **true**.</span><span class="sxs-lookup"><span data-stu-id="10b2b-147">You can find all hidden folders under a parent folder by creating an [extended property definition](properties-and-extended-properties-in-ews-in-exchange.md) for the **PidTagAttributeHidden** extended property, and then using the [FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) method to find folders with a **PidTagAttributeHidden** value that is set to **true**.</span></span> <span data-ttu-id="10b2b-148">Este exemplo usa o MsgFolderRoot, também conhecido como a parte superior do armazenamento de informações, ou a sub-árvore IPM, como a pasta pai a ser pesquisada.</span><span class="sxs-lookup"><span data-stu-id="10b2b-148">This example uses the MsgFolderRoot, also known as the Top of Information Store, or IPM Subtree, as the parent folder to search under.</span></span>
  
<span data-ttu-id="10b2b-149">Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido para o proprietário da caixa de correio e que o usuário foi autenticado em um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="10b2b-149">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox owner, and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
private static void FindHiddenFolders(ExchangeService service)
{
    // Create an extended property definition for the PidTagAttributeHidden property.
    ExtendedPropertyDefinition isHiddenProp = new ExtendedPropertyDefinition(0x10f4, MapiPropertyType.Boolean);
    // Create a folder view to retrieve up to 100 folders and 
    // retrieve only the PidTagAttributeHidden and the display name.
    FolderView folderView = new FolderView(100);
    folderView.PropertySet = new PropertySet(isHiddenProp, FolderSchema.DisplayName);
    // Indicate a Traversal value of Deep, so that all subfolders are retrieved.
    folderView.Traversal = FolderTraversal.Deep;
    // Find all hidden folders under the MsgFolderRoot.
    // This call results in a FindFolder call to EWS.
    FindFoldersResults findFolder = service.FindFolders(WellKnownFolderName.MsgFolderRoot,
            new SearchFilter.IsEqualTo(isHiddenProp, true), folderView);
    // Display the folder ID and display name of each hidden folder.
    foreach (Folder folder in findFolder)
    {
        Console.WriteLine("FolderId: {0}", folder.Id);
        Console.WriteLine("DisplayName: {0}", folder.DisplayName);
        Console.WriteLine("\r\n");
    }
}
```

## <a name="find-all-hidden-folders-by-using-ews"></a><span data-ttu-id="10b2b-150">Localizar todas as pastas ocultas usando o EWS</span><span class="sxs-lookup"><span data-stu-id="10b2b-150">Find all hidden folders by using EWS</span></span>
<span data-ttu-id="10b2b-151"><a name="bk_findhiddenews"> </a></span><span class="sxs-lookup"><span data-stu-id="10b2b-151"><a name="bk_findhiddenews"> </a></span></span>

<span data-ttu-id="10b2b-152">Você pode usar o EWS para localizar todas as pastas ocultas em uma pasta existente chamando a operação [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) e procurando pastas cuja propriedade estendida [PidTagAttributeHidden](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx) está definida como **true**.</span><span class="sxs-lookup"><span data-stu-id="10b2b-152">You can use EWS to find all hidden folders under an existing folder by calling the [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) operation and searching for folders whose [PidTagAttributeHidden](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx) extended property is set to **true**.</span></span> <span data-ttu-id="10b2b-153">Para fazer isso, inclua uma[restrição](https://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) [IsEqualTo](https://msdn.microsoft.com/library/48e7e067-049c-4184-8026-071e6f558e8a%28Office.15%29.aspx)que procura o elemento [ExtendedFieldURI](https://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) para a propriedade **PidTagAttributeHidden** (valor **PropertyTag** como 4243 e o valor **recordtypepropriedade** como Boolean), conforme mostrado na solicitação a seguir.</span><span class="sxs-lookup"><span data-stu-id="10b2b-153">To do this, include an [IsEqualTo](https://msdn.microsoft.com/library/48e7e067-049c-4184-8026-071e6f558e8a%28Office.15%29.aspx)[Restriction](https://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) that searches for the [ExtendedFieldURI](https://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) element for the **PidTagAttributeHidden** property ( **PropertyTag** value to 4243 and the **PropertyType** value to Boolean), as shown in the following request.</span></span> <span data-ttu-id="10b2b-154">Este exemplo usa o MsgFolderRoot, também conhecido como a parte superior do armazenamento de informações, ou a sub-árvore IPM, como a pasta pai a ser pesquisada.</span><span class="sxs-lookup"><span data-stu-id="10b2b-154">This example uses the MsgFolderRoot, also known as the Top of Information Store, or IPM Subtree, as the parent folder to search under.</span></span> 
  
<span data-ttu-id="10b2b-155">Essa é também a solicitação XML que a API gerenciada do EWS envia quando você usa o método **FindFolders** para [Localizar todas as pastas ocultas](#bk_findhiddenewsma).</span><span class="sxs-lookup"><span data-stu-id="10b2b-155">This is also the XML request that the EWS Managed API sends when you use the **FindFolders** method to [find all hidden folders](#bk_findhiddenewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Central Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindFolder Traversal="Deep">
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:ExtendedFieldURI PropertyTag="4340"
                              PropertyType="Boolean" />
          <t:FieldURI FieldURI="folder:DisplayName" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="100"
                               Offset="0"
                               BasePoint="Beginning" />
      <m:Restriction>
        <t:IsEqualTo>
          <t:ExtendedFieldURI PropertyTag="4340"
                              PropertyType="Boolean" />
          <t:FieldURIOrConstant>
            <t:Constant Value="true" />
          </t:FieldURIOrConstant>
        </t:IsEqualTo>
      </m:Restriction>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="msgfolderroot" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="10b2b-156">O servidor responde à solicitação **FindFolder** com uma mensagem [FindFolderResponse](https://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) que inclui um valor de elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica que a pesquisa de pasta foi bem-sucedida, bem como todas as pastas ocultas na pasta de mensagens raiz.</span><span class="sxs-lookup"><span data-stu-id="10b2b-156">The server responds to the **FindFolder** request with a [FindFolderResponse](https://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the folder search was successful, as well as all the hidden folders under the root message folder.</span></span>
  
<span data-ttu-id="10b2b-157">Os valores [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) são reduzidos para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="10b2b-157">The [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) values are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="898"
                         MinorBuildNumber="23"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="6"
                        TotalItemsInView="6"
                        IncludesLastItemInRange="true">
            <t:Folders>
              <t:ContactsFolder>
                <t:FolderId Id="IBHgAAAA=="
                            ChangeKey="AwAAABYAAAD32nSTjepyT63rYH17n9THAAAAAACz" />
                <t:DisplayName>{06967759-274D-40B2-A3EB-D7F9E73727D7}</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:ContactsFolder>
                <t:FolderId Id="IBHwAAAA=="
                            ChangeKey="AwAAABYAAAD32nSTjepyT63rYH17n9THAAAAAAC7" />
                <t:DisplayName>{A9E2BC46-B3A0-4243-B315-60D991004455}</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:ContactsFolder>
                <t:FolderId Id="IBIQAAAA=="
                            ChangeKey="AwAAABYAAAD32nSTjepyT63rYH17n9THAAAAAADO" />
                <t:DisplayName>GAL Contacts</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:ContactsFolder>
                <t:FolderId Id="IBHQAAAA=="
                            ChangeKey="AwAAABYAAAD32nSTjepyT63rYH17n9THAAAAAACa" />
                <t:DisplayName>Recipient Cache</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:Folder>
                <t:FolderId Id="HAAAAA=="
                            ChangeKey="AQAAABYAAAD32nSTjepyT63rYH17n9THAAAAAACS" />
                <t:DisplayName>Conversation Action Settings</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
              <t:Folder>
                <t:FolderId Id="IQywAAAA=="
                            ChangeKey="AQAAABYAAAD32nSTjepyT63rYH17n9THAAAeZIBf" />
                <t:DisplayName>TestFolder</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
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

## 
<span data-ttu-id="10b2b-158"><a name="bk_findhiddenews"> </a></span><span class="sxs-lookup"><span data-stu-id="10b2b-158"><a name="bk_findhiddenews"> </a></span></span>

<span data-ttu-id="10b2b-159">Após ter pastas ocultas ou não ocultas, talvez você queira obter a hierarquia de pastas ou [sincronizar a hierarquia de pastas](how-to-synchronize-folders-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="10b2b-159">After you have hidden or unhidden folders, you might want to get the folder hierarchy or [synchronize the folder hierarchy](how-to-synchronize-folders-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="10b2b-160">Os exemplos que mostram como [obter uma hierarquia de pastas usando a API gerenciada do EWS](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_getfolderhierarchyewsma) ou [obter uma hierarquia de pastas usando o EWS](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_getfolderhierarchyews) também indicam quais pastas da hierarquia estão ocultas.</span><span class="sxs-lookup"><span data-stu-id="10b2b-160">The examples that show you how to [get a folder hierarchy by using the EWS Managed API](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_getfolderhierarchyewsma) or [get a folder hierarchy by using EWS](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_getfolderhierarchyews) also indicate which folders in the hierarchy are hidden.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="10b2b-161">Também consulte</span><span class="sxs-lookup"><span data-stu-id="10b2b-161">See also</span></span>


- [<span data-ttu-id="10b2b-162">Pastas e itens no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="10b2b-162">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)
    
- [<span data-ttu-id="10b2b-163">Trabalhar com pastas usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="10b2b-163">Work with folders by using EWS in Exchange</span></span>](how-to-work-with-folders-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="10b2b-164">Trabalhar com pastas de pesquisa usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="10b2b-164">Work with search folders by using EWS in Exchange</span></span>](how-to-work-with-search-folders-by-using-ews-in-exchange.md)
    

