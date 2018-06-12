---
title: Operação SetHoldOnMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9015a0d8-3495-461b-aa79-797d23169585
description: Encontre informações sobre o EWS SetHoldOnMailboxes operação.
ms.openlocfilehash: 1091ed14ceb25dfd275499b9db47ae4e41b5f1a0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825412"
---
# <a name="setholdonmailboxes-operation"></a>Operação SetHoldOnMailboxes

Encontre informações sobre a operação de EWS **SetHoldOnMailboxes** . 
  
A operação **SetHoldOnMailboxes** define uma política de retenção de caixa de correio em caixas de correio. 
  
This operation was introduced in Exchange Server 2013.
  
## <a name="using-the-setholdonmailboxes-operation"></a>Usando a operação SetHoldOnMailboxes

A operação de **SetHoldOnMailboxes** define uma isenção de caixa de correio em uma ou mais caixas de correio. 
  
### <a name="setholdonmailboxes-operation-soap-headers"></a>Cabeçalhos SOAP SetHoldOnMailboxes operação

A operação **SetHoldOnMailboxes** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir. 
  
|**Nome de cabeçalho**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**ManagementRole** <br/> |[ManagementRole](managementrole.md) <br/> |Identifica as funções de servidor necessários para que o chamador para fazer a solicitação. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Este cabeçalho é aplicável a uma resposta.  <br/> |
   
## <a name="setholdonmailboxes-operation-request-example-apply-a-hold-on-a-mailbox"></a>Exemplo de solicitação de operação SetHoldOnMailboxes: aplicar uma retenção em uma caixa de correio

O exemplo a seguir de uma solicitação de operação **SetHoldOnMailboxes** mostra como aplicar uma retenção em duas caixas de correio. A retenção de caixa de correio foi criada usando o comando [New-MailboxSearch](http://technet.microsoft.com/en-us/library/dd298064.aspx) . 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:SetHoldOnMailboxes>
         <m:ActionType>Create</m:ActionType>
         <m:HoldId>HoldId2</m:HoldId>
         <m:Query>test</m:Query>
         <m:Mailboxes>
            <t:String>/o=First/ou=Exchange(DLT)/cn=Recipients/cn=1fa441ff5e4749ba43ecc0fd94c21adf-Willi</t:String>
            <t:String>/o=First/ou=Exchange(DLT)/cn=Recipients/cn=aed2346adaa34ffc9f0f339917e8de95-Micha</t:String>
         </m:Mailboxes>
         <m:Language>English</m:Language>
         <m:IncludeNonIndexableItems>false</m:IncludeNonIndexableItems>
         <m:Deduplication>true</m:Deduplication>
      </m:SetHoldOnMailboxes>
   </soap:Body>
</soap:Envelope>

```

A solicitação de corpo SOAP contém os seguintes elementos:
  
- [SetHoldOnMailboxes](setholdonmailboxes.md)
    
- [ActionType (HoldActionType)](actiontype-holdactiontype.md)
    
- [HoldId](holdid.md)
    
- [Query](query.md)
    
- [Caixas de correio (ArrayOfStringsType)](mailboxes-arrayofstringstype.md)
    
- [String](string.md)
    
- [Idioma](language.md)
    
- [IncludeNonIndexableItems](includenonindexableitems.md)
    
- [Eliminação da duplicação](deduplication.md)
    
## <a name="successful-setholdonmailboxes-operation-response"></a>Resposta de operação SetHoldOnMailboxes bem-sucedida

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **SetHoldOnMailboxes** para colocar as duas caixas de correio em espera. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <SetHoldOnMailboxesResponse ResponseClass="Success" 
                                  xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <MailboxHoldResult>
            <HoldId xmlns="http://schemas.microsoft.com/exchange/services/2006/types">HoldId2</HoldId>
            <Query xmlns="http://schemas.microsoft.com/exchange/services/2006/types">test</Query>
            <MailboxHoldStatuses xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <MailboxHoldStatus>
                  <Mailbox>o=First/ou=Exchange(DLT)/cn=Recipients/cn=1fa441ff5e4749ba43ecc0fd94c21adf-Willi</Mailbox>
                  <Status>Pending</Status>
                  <AdditionalInfo/>
               </MailboxHoldStatus>
               <MailboxHoldStatus>
                  <Mailbox>/o=First/ou=Exchange(DLT)/cn=Recipients/cn=aed2346adaa34ffc9f0f339917e8de95-Micha</Mailbox>
                  <Status>Pending</Status>
                  <AdditionalInfo/>
               </MailboxHoldStatus>
            </MailboxHoldStatuses>
         </MailboxHoldResult>
      </SetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

A resposta SOAP body contém os seguintes elementos:
  
- [SetHoldOnMailboxesResponse](setholdonmailboxesresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [MailboxHoldResult](mailboxholdresult.md)
    
- [HoldId](holdid.md)
    
- [Query](query.md)
    
- [MailboxHoldStatuses](mailboxholdstatuses.md)
    
- [MailboxHoldStatus](mailboxholdstatus.md)
    
- [Caixa de correio (string)](mailbox-string.md)
    
- [Status (HoldStatusType)](status-holdstatustype.md)
    
- [AdditionalInfo](additionalinfo.md)
    
## <a name="setholdonmailboxes-operation-error-response"></a>Resposta de erro de operação SetHoldOnMailboxes

O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **SetHoldOnMailboxes** . Esta é uma resposta a uma solicitação que contém um identificador de caixa de correio especificada incorretamente. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013"
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <SetHoldOnMailboxesResponse ResponseClass="Error" 
                                  xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>No mailbox is specified for hold operation. If specified in the request, then it could be the object does not exist in AD or is a Distribution Group.</MessageText>
         <ResponseCode>ErrorInvalidOperation</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </SetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

A resposta de erro corpo SOAP contém os seguintes elementos:
  
- [SetHoldOnMailboxesResponse](setholdonmailboxesresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
Para códigos de erro adicionais que são genérica do EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>Confira também

- [Operações do EWS no Exchange](ews-operations-in-exchange.md)
    
- [Operação GetSearchableMailboxes](getsearchablemailboxes-operation.md)
    
- [Operação SearchMailboxes](searchmailboxes-operation.md)
    
- [Operação GetHoldOnMailboxes](getholdonmailboxes-operation.md)
    
- [Operação GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration-operation.md)
    
- [Operação GetNonIndexableItemDetails](getnonindexableitemdetails-operation.md)
    
- [Operação GetNonIndexableItemStatistics](getnonindexableitemstatistics-operation.md)
    

