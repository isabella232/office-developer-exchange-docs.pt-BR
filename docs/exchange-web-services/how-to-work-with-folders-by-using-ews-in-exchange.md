---
title: Trabalhar com pastas usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 4b3eb746-74c4-42a0-aa2c-742c147f1871
description: Saiba como criar, obter, atualizar e excluir pastas usando a API gerenciada do EWS ou o EWS no Exchange.
localization_priority: Priority
ms.openlocfilehash: a184d8da4d6949f01f47afc6a9fb7ed30729fd3b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456378"
---
# <a name="work-with-folders-by-using-ews-in-exchange"></a>Trabalhar com pastas usando o EWS no Exchange

Saiba como criar, obter, atualizar e excluir pastas usando a API gerenciada do EWS ou o EWS no Exchange.
  
O EWS no Exchange usa pastas para estruturar e organizar caixas de correio. Você pode criar novas pastas, obter, atualizar e excluir pastas usando a API gerenciada do EWS ou o EWS. Cada um dos métodos ou operações listados na tabela a seguir é executado em um objeto [Folder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) , um tipo de [pasta](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) ou [um dos tipos ou classes de pasta derivadas](folders-and-items-in-ews-in-exchange.md#bk_folders).
  
**Tabela 1. Métodos e operações para criar, obter, atualizar e excluir pastas**

|**Para...**|**Método de API gerenciada do EWS**|**Operação do EWS**|
|:-----|:-----|:-----|
|Criar uma pasta  <br/> |[Folder. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) <br/> |[CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
|Criar uma hierarquia de pastas  <br/> |Não disponível  <br/> |[Createfolderpath](https://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |
|Obter uma pasta  <br/> |[Folder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> |[GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |
|Obter uma hierarquia de pastas  <br/> |[Folder. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> |[FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |
|Atualizar uma pasta  <br/> |[Pasta. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> |[UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|Excluir uma pasta  <br/> |[Pasta. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> |[DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |

<a name="bk_createfolderewsma"> </a>

## <a name="create-a-folder-by-using-the-ews-managed-api"></a>Criar uma pasta usando a API gerenciada do EWS

O exemplo de código a seguir mostra como usar a classe [Folder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) para criar uma nova pasta genérica com um [DisplayName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) de "pasta personalizada" e um valor de propriedade [FolderClass](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.folderclass%28v=exchg.80%29.aspx) de IPF. Observação. O método [Folder. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) salva a pasta como uma pasta filho da pasta caixa de entrada. 
  
Estes exemplos pressupõem que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário foi autenticado em um servidor Exchange. 
  
```cs
// Create a custom folder.
Folder folder = new Folder(service);
folder.DisplayName = "Custom Folder";
folder.FolderClass = "IPF.Note";
// Save the folder as a child folder of the Inbox.
folder.Save(WellKnownFolderName.Inbox);
```

Para criar um tipo diferente de pasta, como [CalendarFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx), [ContactsFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx), [SearchFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx)ou [TasksFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx), crie uma nova instância da classe específica (em vez da classe de **pasta** genérica) e não defina a propriedade **FolderClass** . Por exemplo, o exemplo de código a seguir mostra como criar um novo [TasksFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx).
  
```cs
// Create a custom Tasks folder.
TasksFolder folder = new TasksFolder(service);
folder.DisplayName = "Custom Tasks";
// Save the folder as a child folder in the Inbox folder.
// This method call results in a CreateFolder call to EWS.
folder.Save(WellKnownFolderName.Inbox);
```

Se você tentar criar uma instância de uma classe específica e também definir a propriedade **FolderClass** , o erro [ErrorNoFolderClassOverride](https://msdn.microsoft.com/library/exchangewebservices.responsecodetype%28v=exchg.80%29.aspx) será gerado. 
  
Observe que você não pode criar um lote para a criação de várias pastas em uma única chamada de método usando a API gerenciada do EWS.
  
## <a name="create-a-folder-by-using-ews"></a>Criar uma pasta usando o EWS
<a name="bk_createfolderews"> </a>

Você pode criar uma única pasta ou várias pastas usando o EWS.
  
Para criar uma única pasta, envie uma mensagem de solicitação de operação [CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) . A solicitação de operação **CreateFolder** indica que a pasta pai é a caixa de entrada, o [DisplayName](https://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx) é "Custom Folder" e o valor do elemento [FolderClass](https://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) é IPF. Observação. 
  
Essa é também a solicitação XML que a API gerenciada do EWS envia quando você cria uma nova pasta e chama o método [Folder. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) . 
  
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
    <m:CreateFolder>
      <m:ParentFolderId>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderId>
      <m:Folders>
        <t:Folder>
          <t:FolderClass>IPF.Note</t:FolderClass>
          <t:DisplayName>Custom Folder</t:DisplayName>
        </t:Folder>
      </m:Folders>
    </m:CreateFolder>
  </soap:Body>
</soap:Envelope>
```

O servidor responde à solicitação **CreateFolder** com uma mensagem [CreateFolderResponse](https://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) que inclui um valor [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) de **NOERROR**, que indica que a pasta foi criada com êxito e o [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) da mensagem recém-criada. 
  
Para criar várias pastas, inclua vários elementos de [pasta](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) na mensagem de solicitação de operação **CreateFolder** . Todas as novas pastas devem estar na mesma pasta pai. 
  
## <a name="create-a-folder-hierarchy-by-using-ews"></a>Criar uma hierarquia de pastas usando o EWS
<a name="bk_createfolderhierarchy"> </a>

Você pode criar uma hierarquia de pastas em uma única chamada usando a operação EWS [createfolderpath](https://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) . A mesma funcionalidade não está disponível na API gerenciada do EWS. Em vez disso, se você estiver usando a API gerenciada do EWS, você pode criar pastas um por um, conforme mostrado em [criar uma pasta usando o EWS](#bk_createfolderews).
  
> [!NOTE]
> A API gerenciada EWS não implementa essa funcionalidade. 
  
## <a name="get-a-folder-by-using-the-ews-managed-api"></a>Obter uma pasta usando a API gerenciada do EWS
<a name="bk_getfolderewsma"> </a>

O exemplo de código a seguir mostra como usar o método [Folder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) para obter a pasta caixa de entrada. Como prática recomendada, limite as propriedades retornadas somente para as necessárias para o aplicativo. Este exemplo limita as propriedades de retorno para incluir apenas a propriedade [ID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) , criando um objeto [PropertySet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) e aplicando o valor [IdOnly](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) à propriedade [BasePropertySet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset.basepropertyset%28v=exchg.80%29.aspx) . 
  
Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário foi autenticado em um servidor Exchange. 
  
```cs
// As a best practice, limit the properties returned to only those that are required.
// In this scenario, you only need the FolderId.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly);
// Bind to an existing folder and get only the properties specified in the PropertySet.
// This method call results in a GetFolder call to EWS.
Folder rootfolder = Folder.Bind(service, WellKnownFolderName.Inbox, propSet);
```

Se você precisar retornar propriedades adicionais, adicione as propriedades da classe [FolderSchema](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderschema%28v=exchg.80%29.aspx) ao **PropertySet**ou use um dos métodos [BIND](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) sobrecarregado que retorna todas as propriedades de primeira classe. 
  
Observe que você não pode obter várias pastas ao mesmo tempo usando a API gerenciada do EWS. Você precisa chamar o método **BIND** em cada pasta separadamente. 
  
## <a name="get-a-folder-by-using-ews"></a>Obter uma pasta usando o EWS
<a name="bk_getfolderews"> </a>

Você pode obter uma única pasta ou várias pastas usando o EWS.
  
Para obter uma única pasta, envie uma mensagem de solicitação de operação [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) para o servidor. No exemplo a seguir, o [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) é definido como **IdOnly**, de modo que somente [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) da pasta especificada é retornado. O elemento [FolderIds](https://msdn.microsoft.com/library/3ff9d15a-7220-4785-ae6b-583a7eb82005%28Office.15%29.aspx) indica que a pasta a ser recuperada é a pasta caixa de entrada. 
  
Essa é também a solicitação XML que a API gerenciada do EWS envia quando você associa a uma pasta usando o método [Folder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) . 
  
Para obter várias pastas, inclua vários elementos [FolderIds](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) na mensagem de solicitação de operação **GetFolder** . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
      </m:FolderShape>
      <m:FolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

O exemplo de XML a seguir mostra a mensagem [GetFolderResponse](https://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) que é enviada do servidor para o cliente em resposta à solicitação de operação **GetFolder** . Ele contém apenas o valor [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) da pasta caixa de entrada. Os valores de alguns atributos e elementos foram reduzidos para facilitar a leitura. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="800"
                         MinorBuildNumber="16"
                         Version="V2_6"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
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
              <t:FolderId Id="AAAENAAA=" ChangeKey="AQAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAEkbCr"/>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

## <a name="get-a-folder-hierarchy-by-using-the-ews-managed-api"></a>Obter uma hierarquia de pastas usando a API gerenciada do EWS
<a name="bk_getfolderhierarchyewsma"> </a>

O exemplo de código a seguir mostra como recuperar as subpastas de uma pasta raiz especificada. Este exemplo recupera as subpastas da pasta **MsgFolderRoot** , que é a raiz da sub-árvore IPM (onde as pastas e os itens da caixa de correio são armazenados). 
  
Neste exemplo, um objeto de classe [folderview](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) é criado para limitar os resultados da resposta do método [Folder. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) . Este cenário limita as propriedades para retornar ao seguinte: [ID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx), [DisplayName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx)e a propriedade estendida que indica se a pasta é uma pasta oculta. Defina o valor [folderview. Traversal](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview.traversal%28v=EXCHG.80%29.aspx) como profundo para executar uma pesquisa recursiva para que o servidor recupere as subpastas e defina a pasta raiz para **MsgFolderRoot**, de modo que o servidor retorne todas as pastas do usuário (e o servidor não retorne pastas de sistema na subárvore não-IPM).
  
Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário foi autenticado em um servidor Exchange. 
  
```XML
// Create a new folder view, and pass in the maximum number of folders to return.
FolderView view = new FolderView(folderViewSize);
// Create an extended property definition for the PR_ATTR_HIDDEN property,
// so that your results will indicate whether the folder is a hidden folder.
ExtendedPropertyDefinition isHiddenProp = new ExtendedPropertyDefinition(0x10f4, MapiPropertyType.Boolean);
// As a best practice, limit the properties returned to only those required.
// In this case, return the folder ID, DisplayName, and the value of the isHiddenProp
// extended property.
view.PropertySet = new PropertySet(BasePropertySet.IdOnly, FolderSchema.DisplayName, isHiddenProp);
// Indicate a Traversal value of Deep, so that all subfolders are retrieved.
view.Traversal = FolderTraversal.Deep;
// Call FindFolders to retrieve the folder hierarchy, starting with the MsgFolderRoot folder.
// This method call results in a FindFolder call to EWS.
FindFoldersResults findFolderResults = service.FindFolders(WellKnownFolderName.MsgFolderRoot, view);
```

## <a name="get-a-folder-hierarchy-by-using-ews"></a>Obter uma hierarquia de pastas usando o EWS
<a name="bk_getfolderhierarchyews"> </a>

Os exemplos de XML a seguir mostram como usar a operação [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) para recuperar uma hierarquia de pastas usando o EWS. Este exemplo recupera a pasta **msgfolderroot** , que é a raiz da sub-árvore IPM e todas as suas subpastas. O atributo de **passagem** é definido como **profundo** para que o servidor execute uma pesquisa recursiva da hierarquia de pastas e só retorne pastas e subpastas na raiz especificada na resposta. Neste exemplo, o elemento [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) é definido como **IdOnly** para que o servidor retorne apenas o elemento [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) . Para facilitar a compreensão da saída, inclua o elemento **DisplayName** nos resultados, incluindo-o no elemento [AdditionalProperties](https://msdn.microsoft.com/library/7a269aed-dcfd-4c3e-9e14-094e53828101%28Office.15%29.aspx) na solicitação, junto com o valor **ExtendedFieldURI** para a propriedade **PR_ATTR_HIDDEN** , para que você saiba se as pastas estão ocultas. 
  
Essa é também a solicitação XML que a API gerenciada do EWS envia quando você chama o método [FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) . 
  
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
    <m:FindFolder Traversal="Deep">
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="folder:DisplayName" />
          <t:ExtendedFieldURI PropertyTag="4340"
                              PropertyType="Boolean" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="100"
                               Offset="0"
                               BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="msgfolderroot" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

O exemplo de XML a seguir mostra a mensagem [FindFolderResponse](https://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) que é enviada do servidor para o cliente em resposta à solicitação de operação **FindFolder** . Ele contém apenas [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx), [DisplayName](https://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx)e o valor da propriedade estendida **PR_ATTR_HIDDEN** para todas as subpastas na pasta **msgrootfolder** Se o elemento [Value](https://msdn.microsoft.com/library/9a30cadd-909e-41b1-b4e9-291643dd89c6%28Office.15%29.aspx) for definido como true, a pasta deverá estar oculta no modo de exibição do cliente. 
  
Essa é também a resposta XML que a API gerenciada do EWS envia quando você obtém várias pastas usando o método [FindFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) . Os valores de alguns atributos e elementos foram reduzidos para legibilidade, e algumas pastas não foram incluídas por brevidade. 
  
```XML
<?xml version="1.0" encoding="utf-8"?><s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="815"
                         MinorBuildNumber="6"
                         Version="V2_7"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="16"
                        TotalItemsInView="16"
                        IncludesLastItemInRange="true">
            <t:Folders>
              <t:CalendarFolder>
                <t:FolderId Id="AAAEOAAA="
                            ChangeKey="AgAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAAAAA3"/>
                <t:DisplayName>Calendar</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean"/>
                  <t:Value>false</t:Value>
                </t:ExtendedProperty>
              </t:CalendarFolder>
              <t:ContactsFolder>
                <t:FolderId Id="AAAEPAAA="
                            ChangeKey="AwAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAAAAA4"/>
                <t:DisplayName>Contacts</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean"/>
                  <t:Value>false</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:ContactsFolder>
                <t:FolderId Id="AAAUKAAA="
                            ChangeKey="AwAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAAAAS5"/>
                <t:DisplayName>Recipient Cache</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean"/>
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:Folder>
                <t:FolderId Id="AAAUJAAA="
                            ChangeKey="AQAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAAAASx"/>
                <t:DisplayName>Conversation Action Settings</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean"/>
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
…
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </m:FindFolderResponse>
  </s:Body>
</s:Envelope>
```

## <a name="update-a-folder-by-using-the-ews-managed-api"></a>Atualizar uma pasta usando a API gerenciada do EWS
<a name="bk_updatefolderewsma"> </a>

O exemplo de código a seguir mostra como atualizar o nome de exibição de uma pasta usando a API gerenciada do EWS.
  
Primeiro, crie um [PropertySet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) para limitar o número de propriedades que o servidor retorna na resposta [Folder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) . Recomendamos que você use o **IdOnly** **BasePropertySet** do IdOnly para reduzir as chamadas para o banco de dados do Exchange. Em seguida, use o método **BIND** para vincular à pasta a ser atualizada. Em seguida, atualize a propriedade [DisplayName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) e use o método [Folder. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) para salvar as alterações. 
  
Neste exemplo, presumimos que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário foi autenticado em um servidor Exchange. A variável local *FolderId* é a [ID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) da pasta a ser atualizada. 
  
```cs
// As a best practice, only include the ID value in the PropertySet.
PropertySet propertySet = new PropertySet(BasePropertySet.IdOnly);
// Bind to an existing folder and get the FolderId.
// This method call results in a GetFolder call to EWS.
Folder folder = Folder.Bind(service, folderId, propertySet);
// Update the display name of the folder.
folder.DisplayName = "Updated folder name";
// Save the updates.
// This method call results in an UpdateFolder call to EWS.
folder.Update();

```

## <a name="update-a-folder-by-using-ews"></a>Atualizar uma pasta usando o EWS
<a name="bk_updatefolderews"> </a>

Os exemplos de XML a seguir mostram como atualizar o nome de exibição de uma pasta usando o EWS.
  
Primeiro, envie uma mensagem de solicitação de operação [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) para obter a pasta a ser atualizada, conforme mostrado em [obter uma hierarquia de pastas usando o EWS](#bk_getfolderhierarchyews).
  
Em seguida, envie uma mensagem de solicitação de operação do [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) para o servidor para atualizar uma pasta. A solicitação de operação **UpdateFolder** atualiza o [DisplayName](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) para "pasta personalizada atualizada". 
  
Essa é também a solicitação XML que a API gerenciada do EWS envia quando você atualiza uma pasta usando o método [Folder. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) . Os valores de alguns atributos e elementos foram reduzidos para facilitar a leitura. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateFolder>
      <m:FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="OrV9ZAAA=" ChangeKey="AQAAABYAAABVzRdyy/cHS4XTC9itCRdUAAAOrXWb" />
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:DisplayName" />
              <t:Folder>
                <t:DisplayName>Updated Custom Folder</t:DisplayName>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

O servidor responde à solicitação **UpdateFolder** com uma mensagem [UpdateFolderResponse](https://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) que inclui o valor de [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) de **NOERROR**e [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) da pasta que foi atualizada com um valor de atributo **ChangeKey** atualizado. 
  
## <a name="delete-a-folder-by-using-the-ews-managed-api"></a>Excluir uma pasta usando a API gerenciada do EWS
<a name="bk_deletefolderewsma"> </a>

Este artigo fornece um exemplo básico que mostra como excluir uma pasta usando a API gerenciada do EWS. Para obter mais detalhes sobre como excluir pastas, consulte [excluindo itens usando o EWS no Exchange](deleting-items-by-using-ews-in-exchange.md).
  
Para excluir uma pasta usando a API gerenciada do EWS, primeiro use o método [Folder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) para vincular o objeto Service à pasta a ser excluída. Em seguida, use o método [Folder. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) para excluir a pasta usando o modo de exclusão [HardDelete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.deletemode%28v=exchg.80%29.aspx) . 
  
Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário foi autenticado em um servidor Exchange. A variável local *FolderId* é a [ID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) da pasta a ser excluída. 
  
```cs
// Bind to an existing folder and get all its properties.
// This method call results in a GetFolder call to EWS.
Folder folder = Folder.Bind(service, folderId);
// HardDelete the folder.
// This method call results in a DeleteFolder call to EWS.
folder.Delete(DeleteMode.HardDelete);
```

## <a name="delete-a-folder-by-using-ews"></a>Excluir uma pasta usando o EWS
<a name="bk_deletefolderews"> </a>

Este artigo fornece um exemplo de XML básico que mostra como excluir uma pasta usando o EWS. Para obter mais detalhes sobre como excluir pastas, consulte [excluindo itens usando o EWS no Exchange](deleting-items-by-using-ews-in-exchange.md).
  
Para excluir uma pasta usando o EWS, primeiro, envie uma mensagem de solicitação de operação [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) para obter a pasta a ser atualizada, conforme mostrado em [obter uma pasta usando o EWS](#bk_getfolderews). 
  
Em seguida, envie uma mensagem de solicitação de operação do [DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) para o servidor para excluir a pasta. A solicitação de operação **DeleteFolder** indica que o **DeleteType** é **HardDelete** e inclui o [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) da pasta a ser excluída. 
  
Essa é também a solicitação XML que a API gerenciada do EWS envia quando você exclui uma pasta usando o método [Folder. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) . Os valores de alguns atributos e elementos foram reduzidos para facilitar a leitura. 
  
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
    <m:DeleteFolder DeleteType="HardDelete">
      <m:FolderIds>
        <t:FolderId Id="OrV9ZAAA=" ChangeKey="AQAAABYAAABVzRdyy/cHS4XTC9itCRdUAAAOrXWf" />
      </m:FolderIds>
    </m:DeleteFolder>
  </soap:Body>
</soap:Envelope>
```

O servidor responde à solicitação **DeleteFolder** com uma mensagem [DeleteFolderResponse](https://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) que inclui o valor de [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) de **NOERROR**, que indica que a exclusão da pasta foi bem-sucedida.
  
## <a name="next-steps"></a>Próximas etapas
<a name="bk_nextsteps"> </a>

Após recuperar as pastas no servidor ou fazer alterações em pastas, talvez você queira [sincronizar sua hierarquia de pastas](how-to-synchronize-folders-by-using-ews-in-exchange.md) ou [assinar notificações sobre alterações de pasta](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) no servidor. 
  
## <a name="see-also"></a>Confira também

- [Pastas e itens no EWS no Exchange](folders-and-items-in-ews-in-exchange.md)   
- [Trabalhar com itens de caixa de correio do Exchange usando o EWS no Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)    
- [Excluir itens usando o EWS no Exchange](deleting-items-by-using-ews-in-exchange.md)   
- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    

