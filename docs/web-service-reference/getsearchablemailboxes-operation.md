---
title: Operação GetSearchableMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 47f8ff57-4835-4d2d-9136-44afb31a4cbe
description: Encontre informações sobre o EWS GetSearchableMailboxes operação.
ms.openlocfilehash: 5e14288280b23e2555eea4fce0f77743d7d210ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752620"
---
# <a name="getsearchablemailboxes-operation"></a>Operação GetSearchableMailboxes

Encontre informações sobre a operação de EWS **GetSearchableMailboxes** . 
  
A operação **GetSearchableMailboxes** obtém um conjunto com escopo de caixas de correio pesquisáveis para pesquisas de descoberta. O escopo de caixas de correio pesquisáveis retornados na resposta é determinado pelo filtro de pesquisa e se a associação de grupo de distribuição é expandida. 
  
This operation was introduced in Exchange Server 2013.
  
## <a name="using-the-getsearchablemailboxes-operation"></a>Usando a operação GetSearchableMailboxes

A operação **GetSearchableMailboxes** obtém informações sobre caixas de correio pesquisáveis. Os seguintes argumentos podem ser passados na solicitação: 
  
- [SearchFilter](searchfilter.md) — aceita um alias de email único como um argumento. 
    
- [ExpandGroupMembership](expandgroupmembership.md) — indica se a associação ao grupo de distribuição é expandida nos resultados retornados na resposta. 
    
Se o alias de email definido no filtro de pesquisa é um grupo de distribuição e a associação ao grupo de distribuição não estiver expandida, a resposta conterá as informações de caixa de correio para o grupo de distribuição. Se o alias de email definido no filtro de pesquisa é um grupo de distribuição e a associação ao grupo de distribuição é expandida, a resposta conterá as informações de caixa de correio para cada caixa de correio que seja membro do grupo de distribuição. Se o filtro de pesquisa contiver um alias de um único usuário, a resposta conterá as informações de caixa de correio para o usuário único. A resposta conterá todas as caixas de correio pesquisáveis se o elemento [GetSearchableMailboxes](getsearchablemailboxes.md) está vazio. Isso é o mesmo como tendo um elemento [SearchFilter](searchfilter.md) vazio e o elemento [ExpandGroupMembership](expandgroupmembership.md) definida como **false**.
  
### <a name="getsearchablemailboxes-operation-soap-headers"></a>Cabeçalhos SOAP GetSearchableMailboxes operação

A operação **GetSearchableMailboxes** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir. 
  
|**Nome de cabeçalho**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**ManagementRole** <br/> |[ManagementRole](managementrole.md) <br/> |Identifica as funções de servidor necessários para que o chamador para fazer a solicitação. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Este cabeçalho é aplicável a uma resposta.  <br/> |
   
## <a name="getsearchablemailboxes-operation-request-example-request-information-about-a-distribution-group"></a>Exemplo de solicitação de operação GetSearchableMailboxes: solicitar informações sobre um grupo de distribuição

O exemplo a seguir de uma solicitação de operação **GetSearchableMailboxes** mostra como obter as informações de caixa de correio para o grupo de distribuição de lolgroup. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetSearchableMailboxes>
         <m:SearchFilter>lolgroup</m:SearchFilter>
         <m:ExpandGroupMembership>false</m:ExpandGroupMembership>
      </m:GetSearchableMailboxes>
   </soap:Body>
</soap:Envelope>

```

A solicitação de corpo SOAP contém os seguintes elementos:
  
- [GetSearchableMailboxes](getsearchablemailboxes.md)
    
- [SearchFilter](searchfilter.md)
    
- [ExpandGroupMembership](expandgroupmembership.md)
    
## <a name="successful-getsearchablemailboxes-operation-response-get-information-about-a-distribution-group"></a>Resposta bem-sucedida de operação GetSearchableMailboxes: obter informações sobre um grupo de distribuição

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **GetSearchableMailboxes** para obter as informações de descoberta para o grupo de distribuição de lolgroup. 
  
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
      <GetSearchableMailboxesResponse ResponseClass="Success" 
                                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <SearchableMailboxes>
            <SearchableMailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <Guid>33a408fe-2574-4e3b-49f5-5e1e000a3035</Guid>
               <PrimarySmtpAddress>LOLgroup@contoso.com</PrimarySmtpAddress>
               <IsExternalMailbox>false</IsExternalMailbox>
               <ExternalEmailAddress/>
               <DisplayName>LOLgroup</DisplayName>
               <IsMembershipGroup>true</IsMembershipGroup>
               <ReferenceId>/o=First/ou=Exchange(FYLT)/cn=Recipients/cn=81213b958a0b5295b13b3f02b812bf1bc-LOLgroup</ReferenceId>
            </SearchableMailbox>
         </SearchableMailboxes>
      </GetSearchableMailboxesResponse>
   </s:Body>
</s:Envelope>

```

A resposta SOAP body contém os seguintes elementos:
  
- [GetSearchableMailboxesResponse](getsearchablemailboxesresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [SearchableMailboxes](searchablemailboxes.md)
    
- [SearchableMailbox](searchablemailbox.md)
    
- [GUID](guid-ex15websvcsotherref.md)
    
- [PrimarySmtpAddress](primarysmtpaddress.md)
    
- [IsExternalMailbox](isexternalmailbox.md)
    
- [ExternalEmailAddress](externalemailaddress.md)
    
- [DisplayName (string)](displayname-string.md)
    
- [IsMembershipGroup](ismembershipgroup.md)
    
- [ID de referência](referenceid.md)
    
## <a name="successful-getsearchablemailboxes-operation-response-get-information-about-an-expanded-distribution-group"></a>Resposta bem-sucedida de operação GetSearchableMailboxes: obter informações sobre um grupo de distribuição expandido

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **GetSearchableMailboxes** para obter as informações de descoberta sobre membros do grupo de distribuição expandido lolgroup. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="526" MinorBuildNumber="0" Version="Exchange2013" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetSearchableMailboxesResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <SearchableMailboxes>
        <SearchableMailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>e2d42cdf-a227-1ec3-486b-6fa0ebaadb9f5</Guid>
          <PrimarySmtpAddress>JSmith@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Julia Smith</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=0a1fc86f883846152405d60956dd02e7-Julia</ReferenceId>
        </SearchableMailbox>
        <SearchableMailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>45d0fff1-6541-459a-a343-52453b30e12ca</Guid>
          <PrimarySmtpAddress>LMoore@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Laura Moore</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=2910d8f8316f4378bbf9338d8f9d714b-Laura</ReferenceId>
        </SearchableMailbox>
        <SearchableMailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>3c620d04-8b33-435a-95be-5b939375576</Guid>
          <PrimarySmtpAddress>SBrown@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Steven Brown</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=90312341a742f0e47e392c80a60d13ecf-Steve</ReferenceId>
        </SearchableMailbox>
      </SearchableMailboxes>
    </GetSearchableMailboxesResponse>
  </s:Body>
</s:Envelope>
```

A resposta SOAP body contém os seguintes elementos:
  
- [GetSearchableMailboxesResponse](getsearchablemailboxesresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [SearchableMailboxes](searchablemailboxes.md)
    
- [SearchableMailbox](searchablemailbox.md)
    
- [GUID](guid-ex15websvcsotherref.md)
    
- [PrimarySmtpAddress](primarysmtpaddress.md)
    
- [IsExternalMailbox](isexternalmailbox.md)
    
- [ExternalEmailAddress](externalemailaddress.md)
    
- [DisplayName (string)](displayname-string.md)
    
- [IsMembershipGroup](ismembershipgroup.md)
    
- [ID de referência](referenceid.md)
    
## <a name="getsearchablemailboxes-operation-error-response"></a>Resposta de erro de operação GetSearchableMailboxes

O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **GetSearchableMailboxes** . Esta é uma resposta a uma solicitação para obter todas as caixas de correio pesquisáveis quando o argumento **ExpandGroupMembership** estiver definido como **true**. 
  
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
      <GetSearchableMailboxesResponse ResponseClass="Error" 
                                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Cannot use wildcard or empty query when auto group expansion is enabled.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         <SearchableMailboxes/>
      </GetSearchableMailboxesResponse>
   </s:Body>
</s:Envelope>

```

A resposta de erro corpo SOAP contém os seguintes elementos:
  
- [GetSearchableMailboxesResponse](getsearchablemailboxesresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [SearchableMailboxes](searchablemailboxes.md)
    
Para códigos de erro adicionais que são genérica do EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>Confira também

- [Operações do EWS no Exchange](ews-operations-in-exchange.md)
    
- [Operação SetHoldOnMailboxes](setholdonmailboxes-operation.md)
    
- [Operação SearchMailboxes](searchmailboxes-operation.md)
    
- [Operação GetHoldOnMailboxes](getholdonmailboxes-operation.md)
    
- [Operação GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration-operation.md)
    
- [Operação GetNonIndexableItemDetails](getnonindexableitemdetails-operation.md)
    
- [Operação GetNonIndexableItemStatistics](getnonindexableitemstatistics-operation.md)
    

