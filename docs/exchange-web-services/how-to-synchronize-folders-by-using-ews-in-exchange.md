---
title: Sincronizar pastas usando o EWS em Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: d3bbacd1-8e4b-4fd0-8d27-4cbbc045ec3f
description: Saiba como usar a API Gerenciada do EWS ou o EWS para obter uma lista de pastas ou uma lista de pastas que foram alteradas para sincronizar seu cliente.
ms.openlocfilehash: f22cb3b4ba92da9c044e08e7164d116293cf43ff
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521089"
---
# <a name="synchronize-folders-by-using-ews-in-exchange"></a>Sincronizar pastas usando o EWS em Exchange

Saiba como usar a API Gerenciada do EWS ou o EWS para obter uma lista de pastas ou uma lista de pastas que foram alteradas para sincronizar seu cliente.
  
O EWS no Exchange usa a sincronização de itens e a sincronização de pastas para sincronizar o conteúdo da caixa de correio entre o cliente e o servidor. A sincronização de pastas obtém a lista inicial de pastas de uma pasta raiz e, com o passar do tempo, obtém alterações feitas nessas pastas e obtém novas pastas também.
  
Se você estiver executando a sincronização de pastas usando a API Gerenciada do EWS, primeiro você obterá a lista [inicial](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma) de pastas na pasta raiz usando o [método ExchangeService.SyncFolderHierarchy.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) Em seguida, atualize o valor do parâmetro  _cSyncState_ durante as chamadas subsequentes para obter a lista de pastas novas e alteradas. 
  
Para executar a sincronização de pastas usando [](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncewsrequest) o EWS, você solicita a lista inicial de pastas na pasta raiz usando a operação [SyncFolderHierarchy,](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) analisar a resposta e, em algum momento no futuro, obter as alterações nas pastas na raiz [e](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncrespews)analisar a resposta. Depois que o cliente recebe a lista de pastas iniciais ou alteradas, ele [faz atualizações localmente](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps). Como e quando você recuperar alterações no futuro depende do padrão de design de [sincronização](mailbox-synchronization-and-ews-in-exchange.md#bk_syncpatterns) que seu aplicativo está usando. 
  
## <a name="get-the-list-of-all-folders-or-changed-folders-by-using-the-ews-managed-api"></a>Obter a lista de todas as pastas ou pastas alteradas usando a API Gerenciada do EWS
<a name="bk_cesyncinitialewsma"> </a>

O exemplo de código a seguir mostra como obter uma lista inicial de pastas em uma pasta raiz e obter uma lista de alterações nas pastas na pasta raiz que ocorreram desde a sincronização anterior. Durante a chamada inicial para o [método ExchangeService.SyncFolderHierarchy,](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.syncfolderhierarchy%28v=exchg.80%29.aspx) de definir o  _valor cSyncState_ como null. Quando o método for concluído, salve o valor _cSyncState_ localmente a ser usado na próxima chamada do método **SyncFolderHierarchy.** Na chamada inicial e nas chamadas subsequentes, as pastas são recuperadas em lotes de dez, usando chamadas sucessivas para o método **SyncFolderHierarchy,** até que não permaneçam mais alterações. Este exemplo define o _parâmetro propertySet_ como IdOnly para reduzir as chamadas para o banco de dados Exchange, que é uma prática de [sincronização.](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices) Neste exemplo, presumimos  que o serviço é uma associação válida de objeto **exchangeService** e que _cSyncState_ representa o estado de sincronização retornado por uma chamada anterior para **SyncFolderHierarchy**. 
  
```cs
// Get a list of all folders in the mailbox by calling SyncFolderHierarchy.
// The folderId parameter must be set to the root folder to synchronize. 
// The propertySet parameter is set to IdOnly to reduce calls to the Exchange database
// because any additional properties result in additional calls to the Exchange database. 
// The syncState parameter is set to cSyncState, which should be null in the initial call, 
// and should be set to the sync state returned by the previous SyncFolderHierarchy call 
// in subsequent calls.
ChangeCollection<FolderChange> fcc = service.SyncFolderHierarchy(new FolderId(WellKnownFolderName.Root), PropertySet.IdOnly, cSyncState);
// If the count of changes is zero, there are no changes to synchronize.
if (fcc.Count == 0)
{
    Console.WriteLine("There are no folders to synchronize.");
}
// Otherwise, write all the changes included in the response 
// to the console. 
// For the initial synchronization, all the changes will be of type
// ChangeType.Create.
else
{
    foreach (FolderChange fc in fcc)
    {
        Console.WriteLine("ChangeType: " + fc.ChangeType.ToString());
        Console.WriteLine("FolderId: " + fc.FolderId);
        Console.WriteLine("===========");
    }
}
// Save the sync state for use in future SyncFolderItems requests.
// The sync state is used by the server to determine what changes to report
// to the client.
string fSyncState = fcc.SyncState;

```

Depois de recuperar a lista de pastas novas ou alteradas no servidor, [crie ou atualize](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps)as pastas no cliente .
  
## <a name="get-the-initial-list-of-folders-by-using-ews"></a>Obter a lista inicial de pastas usando o EWS
<a name="bk_cesyncewsrequest"> </a>

O exemplo a seguir mostra uma solicitação XML para obter a hierarquia de pastas inicial usando a [operação SyncFolderHierarchy.](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) Esta também é a solicitação XML que a API Gerenciada do EWS envia ao recuperar a lista de pastas iniciais usando o [método SyncFolderHierarchy](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma). O [elemento SyncState](https://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) da operação [SyncFolderHierarchy](https://msdn.microsoft.com/library/7f0de089-8876-47ec-a871-df118ceae75d%28Office.15%29.aspx) não está incluído porque essa é a sincronização inicial. Este exemplo define o [elemento BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) como **IdOnly** para reduzir as chamadas para o banco de dados Exchange, que é uma prática de [sincronização.](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices)
  
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
    <m:SyncFolderHierarchy>
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
      </m:FolderShape>
      <m:SyncFolderId>
        <t:DistinguishedFolderId Id="root" />
      </m:SyncFolderId>
    </m:SyncFolderHierarchy>
  </soap:Body>
</soap:Envelope>
```

O exemplo a seguir mostra a resposta XML retornada pelo servidor depois que ele processa a solicitação de operação [SyncFolderHierarchy.](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) A resposta inicial inclui [Criar](https://msdn.microsoft.com/library/6b463d0a-70e9-40c5-ade4-c7d9a5f36bc1%28Office.15%29.aspx) elementos para todas as pastas porque todas as pastas são consideradas novas durante uma sincronização inicial. Os valores de alguns atributos e elementos foram reduzidos para a capacidade de leitura, e alguns **blocos** de elemento Create foram removidos para brevidade. 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="785"
                         MinorBuildNumber="6"
                         Version="V2_6"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SyncFolderHierarchyResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                                   xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SyncFolderHierarchyResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAA==</m:SyncState>
          <m:IncludesLastFolderInRange>true</m:IncludesLastFolderInRange>
          <m:Changes>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkADM="
                            ChangeKey="AQAAABYA"/>
              </t:Folder>
            </t:Create>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkADMzM="
                            ChangeKey="AQAAABY"/>
              </t:Folder>
            </t:Create>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkAD/AAA="
                            ChangeKey="AQAAABYA"/>
              </t:Folder>
            </t:Create>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkADBh="
                            ChangeKey="AQAAABYA"/>
              </t:Folder>
            </t:Create>
            ...
          </m:Changes>
        </m:SyncFolderHierarchyResponseMessage>
      </m:ResponseMessages>
    </m:SyncFolderHierarchyResponse>
  </s:Body>
</s:Envelope>
```

Depois de recuperar a lista de novas pastas no servidor, [crie as pastas no cliente](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_nextsteps).
  
## <a name="get-the-changes-since-the-last-sync-by-using-ews"></a>Obter as alterações desde a última sincronização usando o EWS
<a name="bk_cesyncrespews"> </a>

O exemplo a seguir mostra a solicitação XML para obter a lista de alterações nas pastas na pasta raiz usando a [operação SyncFolderHierarchy.](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) Essa também é a solicitação XML que a API Gerenciada do EWS envia ao recuperar a lista de [alterações na pasta raiz](how-to-synchronize-folders-by-using-ews-in-exchange.md#bk_cesyncinitialewsma). Este exemplo define o valor do elemento [SyncState](https://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) como o valor retornado na resposta anterior. E para fins de demonstração, este exemplo define o [elemento BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) como **AllProperties** em vez de **IdOnly** para mostrar as propriedades adicionais retornadas. Definir o [elemento BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) como **IdOnly** é uma prática prática [de sincronização.](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices) O valor de **SyncState** foi reduzido para a capacidade de leitura. 
  
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
    <m:SyncFolderHierarchy>
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </m:FolderShape>
      <m:SyncFolderId>
        <t:DistinguishedFolderId Id="root" />
      </m:SyncFolderId>
      <m:SyncState>H4sIAA==</m:SyncState>
    </m:SyncFolderHierarchy>
  </soap:Body>
</soap:Envelope>
```

O exemplo a seguir mostra a resposta XML retornada pelo servidor depois que ele processa a solicitação de operação [SyncFolderHierarchy](https://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) do cliente. Essa resposta indica que uma pasta foi atualizada, uma pasta foi criada e uma pasta foi excluída desde a sincronização anterior. O valor do elemento [SyncState,](https://msdn.microsoft.com/library/e5ebaae3-0f07-481d-ac67-d9687a3c7ac3%28Office.15%29.aspx) atributos **de Id** e **atributos ChangeKey** foram reduzidos para a capacidade de leitura. 
  
Lembre-se de que a solicitação incluiu **AllProperties**[BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx). Isso é apenas para fins de demonstração. Recomendamos definir o elemento **BaseShape** como **IdOnly** em produção. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
<h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="745" MinorBuildNumber="21" Version="V2_3" 
           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SyncFolderHierarchyResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
            xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SyncFolderHierarchyResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAAA</m:SyncState>
          <m:IncludesLastFolderInRange>true</m:IncludesLastFolderInRange>
          <m:Changes>
            <t:Update>
              <t:Folder>
                <t:FolderId Id="AAMkADM=" ChangeKey="AQAAABY" />
                <t:ParentFolderId Id="AQMkADMzADI1==" ChangeKey="AQAAAA==" />
                <t:FolderClass>IPF.Note</t:FolderClass>
                <t:DisplayName>Meeting Notes</t:DisplayName>
                <t:TotalCount>3</t:TotalCount>
                <t:ChildFolderCount>0</t:ChildFolderCount>
                <t:EffectiveRights>
                  <t:CreateAssociated>true</t:CreateAssociated>
                  <t:CreateContents>true</t:CreateContents>
                  <t:CreateHierarchy>true</t:CreateHierarchy>
                  <t:Delete>true</t:Delete>
                  <t:Modify>true</t:Modify>
                  <t:Read>true</t:Read>
                  <t:ViewPrivateItems>true</t:ViewPrivateItems>
                </t:EffectiveRights>
                <t:UnreadCount>0</t:UnreadCount>
              </t:Folder>
            </t:Update>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AAMkADMzM=" ChangeKey="AQAAABYAA" />
                <t:ParentFolderId Id="AQMkO67A==" ChangeKey="AQAAAA==" />
                <t:FolderClass>IPF.Note</t:FolderClass>
                <t:DisplayName>Schedules</t:DisplayName>
                <t:TotalCount>0</t:TotalCount>
                <t:ChildFolderCount>0</t:ChildFolderCount>
                <t:EffectiveRights>
                  <t:CreateAssociated>true</t:CreateAssociated>
                  <t:CreateContents>true</t:CreateContents>
                  <t:CreateHierarchy>true</t:CreateHierarchy>
                  <t:Delete>true</t:Delete>
                  <t:Modify>true</t:Modify>
                  <t:Read>true</t:Read>
                  <t:ViewPrivateItems>true</t:ViewPrivateItems>
                </t:EffectiveRights>
                <t:UnreadCount>0</t:UnreadCount>
              </t:Folder>
            </t:Create>
            <t:Delete>
              <t:FolderId Id="AAMkAD/AAA=" ChangeKey="AQAAAA==" />
            </t:Delete>
          </m:Changes>
        </m:SyncFolderHierarchyResponseMessage>
      </m:ResponseMessages>
    </m:SyncFolderHierarchyResponse>
  </s:Body>
</s:Envelope>

```

## <a name="update-the-client"></a>Atualizar o cliente
<a name="bk_nextsteps"> </a>

Se você estiver usando a API Gerenciada do EWS, depois de obter a lista de pastas novas ou alteradas, use o método [Folder.Load](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.load%28v=exchg.80%29.aspx) para obter propriedades nos itens novos ou alterados, compare as propriedades com os valores locais e atualize ou crie as pastas no cliente. 
  
Se você estiver usando o EWS, use a operação [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) para obter propriedades nas pastas novas ou alteradas e atualizar ou criar as pastas no cliente. 
  
## <a name="see-also"></a>Confira também

- [Sincronização de caixa de correio e EWS no Exchange](mailbox-synchronization-and-ews-in-exchange.md)   
- [Sincronizar itens usando o EWS no Exchange](how-to-synchronize-items-by-using-ews-in-exchange.md)   
- [Lidar com erros relacionados à sincronização no EWS no Exchange](handling-synchronization-related-errors-in-ews-in-exchange.md)
    

