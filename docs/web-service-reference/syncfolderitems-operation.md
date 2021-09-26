---
title: Operação SyncFolderItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SyncFolderItems
api_type:
- schema
ms.assetid: 7f0de089-8876-47ec-a871-df118ceae75d
description: A operação SyncFolderItems sincroniza itens entre o servidor Exchange e o cliente.
ms.openlocfilehash: 07915f5f9f7ae1fc6f5a743f2e0480a32cb808a7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545829"
---
# <a name="syncfolderitems-operation"></a>Operação SyncFolderItems

A operação SyncFolderItems sincroniza itens entre o servidor Exchange e o cliente.
  
## <a name="remarks"></a>Comentários

A operação SyncFolderItems retornará um máximo de 512 alterações. Solicitações SyncFolderItems subsequentes devem ser executadas para obter alterações adicionais. 
  
SyncFolderItems é semelhante à operação FindItem, na qual não pode retornar propriedades como Body ou Attachments. Se a operação SyncFolderItems não retornar as propriedades de que você precisa, você poderá usar a operação [GetItem](getitem-operation.md) para obter um conjunto específico de propriedades para cada item retornado por SyncFolderItems. 
  
## <a name="syncfolderitems-request-example"></a>Exemplo de solicitação SyncFolderItems

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação SyncFolderItems mostra como sincronizar itens em uma pasta. Este exemplo mostra a sincronização de um item de pasta que não é a primeira sincronização que ocorreu para a pasta Itens Enviados. O [elemento SyncState](syncstate-ex15websvcsotherref.md) não está incluído na solicitação para a primeira tentativa de sincronizar um cliente com o Exchange servidor. A primeira tentativa de sincronizar os itens em uma hierarquia de pastas retornará todos os itens na caixa de correio, excluindo itens identificados no [elemento Ignore.](ignore.md) Essa solicitação SyncFolderItems tentará sincronizar todas as alterações nos itens de pasta desde a última sincronização. Essa solicitação ignorará a tentativa de sincronizar o único item identificado no [elemento Ignore.](ignore.md) 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SyncFolderItems xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>Default</t:BaseShape>
      </ItemShape>
      <SyncFolderId>
        <t:DistinguishedFolderId Id="sentitems"/>
      </SyncFolderId>
      <SyncState>AEbJ94eMOAAA=</SyncState>
      <Ignore>
        <t:ItemId Id="AQApAHRAA==" ChangeKey="CQAAABY"/>
      </Ignore>
      <MaxChangesReturned>100</MaxChangesReturned>
    </SyncFolderItems>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comentários

Os dados codificados pelo elemento [SyncState](syncstate-ex15websvcsotherref.md) com base64 e o atributo **Id** do [elemento ItemId](itemid.md) foram reduzidos para preservar a capacidade de leitura. 
  
### <a name="request-elements"></a>Elementos request

Os seguintes elementos são usados na solicitação:
  
- [SyncFolderItems](syncfolderitems.md)
    
- [ItemShape](itemshape.md)
    
- [BaseShape](baseshape.md)
    
- [SyncFolderId](syncfolderid.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [SyncState](syncstate-ex15websvcsotherref.md)
    
- [Ignore](ignore.md)
    
- [ItemId](itemid.md)
    
- [MaxChangesReturned](maxchangesreturned.md)
    
## <a name="successful-syncfolderitems-response"></a>Resposta SyncFolderItems bem-sucedida

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta bem-sucedida à solicitação SyncFolderItems. Neste exemplo, uma solicitação de reunião é sincronizada da pasta Itens Enviados.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SyncFolderItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SyncFolderItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAAAAA=</m:SyncState>
          <m:IncludesLastItemInRange>true</m:IncludesLastItemInRange>
          <m:Changes>
            <t:Create>
              <t:MeetingRequest>
                <t:ItemId Id="AQApAHRwA==" ChangeKey="CwAAABYA" />
                <t:Subject>Budget Q3</t:Subject>
                <t:Sensitivity>Normal</t:Sensitivity>
                <t:IsOutOfDate>false</t:IsOutOfDate>
                <t:HasBeenProcessed>true</t:HasBeenProcessed>
                <t:ResponseType>NoResponseReceived</t:ResponseType>
                <t:IntendedFreeBusyStatus>Busy</t:IntendedFreeBusyStatus>
                <t:Start>2006-08-02T17:30:00Z</t:Start>
                <t:End>2006-08-02T19:30:00Z</t:End>
                <t:Location>Conference Room 2</t:Location>
                <t:Organizer>
                  <t:Mailbox>
                    <t:Name>Dan Park</t:Name>
                    <t:EmailAddress>dpark@example.com</t:EmailAddress>
                    <t:RoutingType>SMTP</t:RoutingType>
                  </t:Mailbox>
                </t:Organizer>
              </t:MeetingRequest>
            </t:Create>
          </m:Changes>
        </m:SyncFolderItemsResponseMessage>
      </m:ResponseMessages>
    </SyncFolderItemsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comentários

Os dados codificados pelo elemento [SyncState](syncstate-ex15websvcsotherref.md) com base64 e o atributo **Id** do [elemento ItemId](itemid.md) foram reduzidos para preservar a capacidade de leitura. 
  
### <a name="successful-response-elements"></a>Elementos de resposta bem-sucedidos

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [SyncFolderItemsResponse](syncfolderitemsresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [SyncState](syncstate-ex15websvcsotherref.md)
    
- [IncludesLastItemInRange](includeslastiteminrange.md)
    
- [Changes (Items)](changes-items.md)
    
- [Create (ItemSync)](create-itemsync.md)
    
- [MeetingRequest](meetingrequest.md)
    
- [ItemId](itemid.md)
    
- [Assunto](subject.md)
    
- [Sensitivity](sensitivity.md)
    
- [IsOutOfDate](isoutofdate.md)
    
- [HasBeenProcessed](hasbeenprocessed.md)
    
- [ResponseType](responsetype.md)
    
- [IntendedFreeBusyStatus](intendedfreebusystatus.md)
    
- [Start](start.md)
    
- [End ](end-ex15websvcsotherref.md)
    
- [Location](location.md)
    
- [Organizador](organizer.md)
    
- [Caixa de Correio](mailbox.md)
    
- [Name (EmailAddressType)](name-emailaddresstype.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)
    
- [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md)
    
## <a name="syncfolderitems-error-response"></a>Resposta de erro SyncFolderItems

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta de erro a uma solicitação SyncFolderItems. Esse erro foi causado por um SyncState inválido.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SyncFolderItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SyncFolderItemsResponseMessage ResponseClass="Error">
          <m:MessageText>Synchronization state data is corrupt or otherwise invalid.</m:MessageText>
          <m:ResponseCode>ErrorInvalidSyncStateData</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:SyncState />
          <m:IncludesLastItemInRange>true</m:IncludesLastItemInRange>
        </m:SyncFolderItemsResponseMessage>
      </m:ResponseMessages>
    </SyncFolderItemsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Elementos de resposta de erro

Os seguintes elementos são usados na resposta de erro:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [SyncFolderItemsResponse](syncfolderitemsresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [SyncState](syncstate-ex15websvcsotherref.md)
    
- [IncludesLastItemInRange](includeslastiteminrange.md)
    
## <a name="see-also"></a>Confira também



- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

