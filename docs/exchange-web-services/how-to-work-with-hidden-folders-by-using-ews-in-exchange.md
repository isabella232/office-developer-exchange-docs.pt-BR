---
title: Trabalhar com pastas ocultas usando o EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 7ae7c045-cd90-4c9f-baf5-0464d5058f45
description: Saiba como tornar uma pasta oculta e encontrar pastas ocultas usando a API Gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: 722cc09aa62ae4201362c59f7d7d2b4988e25837
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513070"
---
# <a name="work-with-hidden-folders-by-using-ews-in-exchange"></a>Trabalhar com pastas ocultas usando o EWS no Exchange

Saiba como tornar uma pasta oculta e encontrar pastas ocultas usando a API Gerenciada do EWS ou o EWS no Exchange.
  
Com uma exceção, as pastas na raiz de uma caixa de correio Exchange (a subárvore que não é do IPM) são ocultadas do usuário. Por outro lado, todas as pastas **no MsgFolderRoot** (a subárvore do IPM) ficam visíveis para o usuário. Como ocultar uma pasta sob o **MsgFolderRoot?** Não é tão complicado — ele se resume a apenas uma propriedade, a propriedade estendida [PidTagAttributeHidden](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx) (0x10F4000B). Quando essa propriedade for definida como **true,** Outlook ou outro cliente que usa a propriedade para determinar a visibilidade da pasta ocultará a pasta do ponto de vista do usuário. Como essa é uma propriedade estendida, é mais complexo de usar do que sua propriedade de pasta média, portanto, este artigo o fará passar pelos principais cenários.
  
**Tabela 1. Métodos de API Gerenciada EWS e operações EWS para trabalhar com pastas ocultas**

|**Tarefa**|**Método da API Gerenciada do EWS**|**Operação do EWS**|
|:-----|:-----|:-----|
|Ocultar uma pasta  <br/> |[Folder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) seguido por [Folder.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> |[GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) seguido [por UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|Encontrar pastas ocultas  <br/> |[FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) <br/> |[FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |
   
Você está se perguntando qual é a única exceção , ou seja, qual pasta na raiz está visível para os usuários? É a pasta Finder (também conhecida como o valor de enumeração **SearchFolders**[WellKnownFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) ou o valor do elemento [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) de **searchfolders),** que contém as pastas de pesquisa dos usuários. As pastas de pesquisa criadas na pasta Finder ficam visíveis para Outlook usuários. Se você precisar criar uma pasta de pesquisa que não seja visível para os usuários, movê-la para baixo da pasta raiz para o ocultar. Ao contrário de outras pastas, definir a propriedade **PidTagAttributeHidden** como **true** não ocultará uma pasta de pesquisa na pasta Finder. 
  
## <a name="hide-a-folder-by-using-the-ews-managed-api"></a>Ocultar uma pasta usando a API Gerenciada do EWS
<a name="bk_hideewsma"> </a>

Você pode [tornar uma pasta existente uma](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_createfolderewsma) pasta oculta alterando a propriedade estendida [PidTagAttributeHidden](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx) como **true**. Primeiro, crie uma [definição de propriedade estendida para a propriedade](properties-and-extended-properties-in-ews-in-exchange.md). Em seguida, use o método [Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) para chegar à pasta e atualize o valor da propriedade **PidTagAttributeHidden** como true e use o método [Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) para salvar as alterações. 
  
Este exemplo pressupõe que o serviço é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido para o proprietário da caixa de correio, [](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) que o usuário foi autenticado para um servidor Exchange e que **folderId** é um Folder.Id válido que identifica a pasta a ser ocultada.  
  
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

## <a name="hide-a-folder-by-using-ews"></a>Ocultar uma pasta usando o EWS
<a name="bk_hideews"> </a>

Você pode usar o EWS para [tornar](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_createfolderewsma) uma pasta existente uma pasta oculta alterando a propriedade estendida [PidTagAttributeHidden](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx) como **true**. Primeiro, use a operação [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) para chegar à pasta e, em seguida, recupere a propriedade **PidTagAttributeHidden** incluindo o [elemento ExtendedFieldURI](https://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) e definindo o valor **PropertyTag** como 4340 e o **valor PropertyType** como Boolean. 
  
Essa também é a solicitação XML que a API Gerenciada do EWS envia quando você usa o método **Bind** para obter uma pasta antes de tornar [uma pasta oculta.](#bk_hideewsma)
  
O [valor FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) é reduzido para capacidade de leitura. 
  
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

O servidor responde à solicitação **GetFolder** com uma mensagem [GetFolderResponse](https://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) que inclui um valor de elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **de NoError**, que indica que a pasta foi recuperada com êxito. A resposta também inclui um [Valor](https://msdn.microsoft.com/library/196278d4-5e77-4e0a-8af6-8ac065610510%28Office.15%29.aspx) para [ExtendedProperty](https://msdn.microsoft.com/library/f9701409-b620-4afe-b9ee-4c1e95507af7%28Office.15%29.aspx). Neste exemplo, **Value** é definido como **false**, o que significa que a pasta não está oculta no momento.
  
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

Para alterar o valor da **Propriedade Estendida** para true, use a [operação UpdateFolder.](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) Inclua os **elementos ExtendedProperty,** **ExtendedFieldURI** e **Value** para a propriedade estendida **PidTagAttributeHidden** e de definir o elemento **Value** como **true** para ocultar a pasta. 
  
Essa também é a solicitação XML que a API Gerenciada do EWS envia quando você usa o método **Update** para atualizar uma pasta para [torná-la uma pasta oculta.](#bk_hideewsma)
  
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

O servidor responde à solicitação **UpdateFolder** com uma mensagem [UpdateFolderResponse](https://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) que inclui um valor de elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **de NoError**, que indica que a pasta foi atualizada com êxito e agora está oculta.
  
## <a name="find-all-hidden-folders-by-using-the-ews-managed-api"></a>Encontre todas as pastas ocultas usando a API Gerenciada do EWS
<a name="bk_findhiddenewsma"> </a>

Você pode encontrar todas as pastas ocultas [](properties-and-extended-properties-in-ews-in-exchange.md) em uma pasta pai criando uma definição de propriedade estendida para a propriedade estendida **PidTagAttributeHidden** e usando o método [FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) para encontrar pastas com um valor **PidTagAttributeHidden** definido como **true**. Este exemplo usa o MsgFolderRoot, também conhecido como o Armazenamento de Informações Superior ou Subárvore do IPM, como a pasta pai a ser pesquisada.
  
Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido para o proprietário da caixa de correio e que o usuário foi autenticado para um servidor Exchange. 
  
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

## <a name="find-all-hidden-folders-by-using-ews"></a>Encontre todas as pastas ocultas usando o EWS
<a name="bk_findhiddenews"> </a>

Você pode usar o EWS para encontrar todas as pastas ocultas em uma pasta existente chamando a operação [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) e procurando pastas cuja propriedade estendida [PidTagAttributeHidden](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx) está definida como **true**. Para fazer isso, inclua uma Restrição [IsEqualTo](https://msdn.microsoft.com/library/48e7e067-049c-4184-8026-071e6f558e8a%28Office.15%29.aspx)[](https://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) que pesquisa o elemento [ExtendedFieldURI](https://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) para a propriedade **PidTagAttributeHidden** ( **valor PropertyTag** para 4243 e o valor **PropertyType** para Boolean), conforme mostrado na solicitação a seguir. Este exemplo usa o MsgFolderRoot, também conhecido como o Armazenamento de Informações Superior ou Subárvore do IPM, como a pasta pai a ser pesquisada. 
  
Essa também é a solicitação XML que a API Gerenciada do EWS envia quando você usa o método **FindFolders** para [encontrar todas as pastas ocultas.](#bk_findhiddenewsma)
  
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

O servidor responde à solicitação **FindFolder** com uma mensagem [FindFolderResponse](https://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) que inclui um valor de elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **de NoError**, que indica que a pesquisa de pasta foi bem-sucedida, bem como todas as pastas ocultas na pasta de mensagem raiz.
  
Os [valores FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) são reduzidos para capacidade de leitura. 
  
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
<a name="bk_findhiddenews"> </a>

Depois de ter pastas ocultas ou não ativas, talvez você queira obter a hierarquia de pastas ou [sincronizar a hierarquia de pastas.](how-to-synchronize-folders-by-using-ews-in-exchange.md) Os exemplos que mostram como obter uma hierarquia de pastas usando a API Gerenciada do [EWS](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_getfolderhierarchyewsma) ou obter uma hierarquia de pastas usando [o EWS](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_getfolderhierarchyews) também indicam quais pastas na hierarquia estão ocultas. 
  
## <a name="see-also"></a>Confira também


- [Pastas e itens no EWS em Exchange](folders-and-items-in-ews-in-exchange.md)
    
- [Trabalhar com pastas usando o EWS no Exchange](how-to-work-with-folders-by-using-ews-in-exchange.md)
    
- [Trabalhar com pastas de pesquisa usando o EWS no Exchange](how-to-work-with-search-folders-by-using-ews-in-exchange.md)
    

