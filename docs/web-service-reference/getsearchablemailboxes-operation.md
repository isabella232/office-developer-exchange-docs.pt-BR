---
title: Operação GetSearchableMailboxes
manager: sethgros
ms.date: 01/24/2020
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 47f8ff57-4835-4d2d-9136-44afb31a4cbe
description: Encontre informações sobre a operação GetSearchableMailboxes EWS.
ms.openlocfilehash: 385a1e317069641c51249c9522cf404ecf961722
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523080"
---
# <a name="getsearchablemailboxes-operation"></a>Operação GetSearchableMailboxes

> [!IMPORTANT]
> A partir de 1º de abril de 2020, a operação GetSearchableMailboxes não estará mais disponível no Exchange Online. Essa operação não será afetada em versões locais do Exchange Server. Para obter mais informações, [consulte Retirement of legacy eDiscovery tools in Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#getsearchablemailboxes-setholdonmailboxes-and-getholdonmailboxes-operations-in-the-ews-api).

Encontre informações sobre a **operação GetSearchableMailboxes** EWS. 
  
A **operação GetSearchableMailboxes** obtém um conjunto com escopo de caixas de correio pesquisáveis para pesquisas de descoberta. O escopo de caixas de correio pesquisáveis retornadas na resposta é determinado pelo filtro de pesquisa e se a associação ao grupo de distribuição é expandida. 

> [!NOTE] 
> Essa operação destina-se a ser usada com o filtro de pesquisa e recuperar apenas os primeiros milhares; não se destina a recuperação exaustiva.
  
This operation was introduced in Exchange Server 2013.
  
## <a name="using-the-getsearchablemailboxes-operation"></a>Usando a operação GetSearchableMailboxes

A **operação GetSearchableMailboxes** obtém informações sobre caixas de correio pesquisáveis. Os seguintes argumentos podem ser passados na solicitação: 
  
- [SearchFilter](searchfilter.md) - Aceita um único alias de email como argumento. 
    
- [ExpandGroupMembership](expandgroupmembership.md) - Indica se a associação ao grupo de distribuição é expandida nos resultados retornados na resposta. 
    
Se o alias de email definido no filtro de pesquisa for um grupo de distribuição e a associação ao grupo de distribuição não for expandida, a resposta conterá as informações de caixa de correio do grupo de distribuição. Se o alias de email definido no filtro de pesquisa for um grupo de distribuição e a associação ao grupo de distribuição for expandida, a resposta conterá as informações de caixa de correio para cada caixa de correio que é membro do grupo de distribuição. Se o filtro de pesquisa contiver um único alias de usuário, a resposta conterá as informações de caixa de correio para o usuário único. A resposta conterá todas as caixas de correio pesquisáveis se [o elemento GetSearchableMailboxes](getsearchablemailboxes.md) estiver vazio. Isso é o mesmo que ter um elemento [SearchFilter](searchfilter.md) vazio e o [elemento ExpandGroupMembership](expandgroupmembership.md) definido como **false**.
  
### <a name="getsearchablemailboxes-operation-soap-headers"></a>Headers soap da operação GetSearchableMailboxes

A **operação GetSearchableMailboxes** pode usar os headers SOAP listados na tabela a seguir. 
  
|Nome de cabeçalho|Elemento|Descrição|
|:-----|:-----|:-----|
|**ManagementRole** <br/> |[ManagementRole](managementrole.md) <br/> |Identifica as funções de servidor necessárias para que o chamador faça a solicitação. Esse header é aplicável a uma solicitação.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Esse header é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Esse header é aplicável a uma resposta.  <br/> |
   
## <a name="getsearchablemailboxes-operation-request-example-request-information-about-a-distribution-group"></a>Exemplo da solicitação de operação GetSearchableMailboxes: Solicitar informações sobre um grupo de distribuição

O exemplo a seguir de uma solicitação de operação **GetSearchableMailboxes** mostra como obter as informações de caixa de correio para o grupo de distribuição de lolgroup. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

O corpo SOAP de solicitação contém os seguintes elementos:
  
- [GetSearchableMailboxes](getsearchablemailboxes.md)   
- [SearchFilter](searchfilter.md)    
- [ExpandGroupMembership](expandgroupmembership.md)
    
## <a name="successful-getsearchablemailboxes-operation-response-get-information-about-a-distribution-group"></a>Resposta bem-sucedida da operação GetSearchableMailboxes: Obter informações sobre um grupo de distribuição

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **GetSearchableMailboxes** para obter as informações de descoberta do grupo de distribuição lolgroup. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetSearchableMailboxesResponse ResponseClass="Success" 
                                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <SearchableMailboxes>
            <SearchableMailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

O corpo SOAP de resposta contém os seguintes elementos:
  
- [GetSearchableMailboxesResponse](getsearchablemailboxesresponse.md)   
- [ResponseCode](responsecode.md)   
- [SearchableMailboxes](searchablemailboxes.md)    
- [SearchableMailbox](searchablemailbox.md)    
- [Guid](guid-ex15websvcsotherref.md)    
- [PrimarySmtpAddress](primarysmtpaddress.md)    
- [IsExternalMailbox](isexternalmailbox.md)   
- [ExternalEmailAddress](externalemailaddress.md)    
- [DisplayName (cadeia de caracteres)](displayname-string.md)    
- [IsMembershipGroup](ismembershipgroup.md)    
- [ReferenceId](referenceid.md)
    
## <a name="successful-getsearchablemailboxes-operation-response-get-information-about-an-expanded-distribution-group"></a>Resposta bem-sucedida da operação GetSearchableMailboxes: obter informações sobre um grupo de distribuição expandido

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **GetSearchableMailboxes** para obter as informações de descoberta sobre membros do grupo de distribuição de lolgroup expandido. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="526" MinorBuildNumber="0" Version="Exchange2013" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetSearchableMailboxesResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <SearchableMailboxes>
        <SearchableMailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>e2d42cdf-a227-1ec3-486b-6fa0ebaadb9f5</Guid>
          <PrimarySmtpAddress>JSmith@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Julia Smith</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=0a1fc86f883846152405d60956dd02e7-Julia</ReferenceId>
        </SearchableMailbox>
        <SearchableMailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>45d0fff1-6541-459a-a343-52453b30e12ca</Guid>
          <PrimarySmtpAddress>LMoore@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Laura Moore</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=2910d8f8316f4378bbf9338d8f9d714b-Laura</ReferenceId>
        </SearchableMailbox>
        <SearchableMailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

O corpo SOAP de resposta contém os seguintes elementos:
  
- [GetSearchableMailboxesResponse](getsearchablemailboxesresponse.md)    
- [ResponseCode](responsecode.md)   
- [SearchableMailboxes](searchablemailboxes.md)    
- [SearchableMailbox](searchablemailbox.md)    
- [Guid](guid-ex15websvcsotherref.md)    
- [PrimarySmtpAddress](primarysmtpaddress.md)    
- [IsExternalMailbox](isexternalmailbox.md)    
- [ExternalEmailAddress](externalemailaddress.md)    
- [DisplayName (cadeia de caracteres)](displayname-string.md)    
- [IsMembershipGroup](ismembershipgroup.md)    
- [ReferenceId](referenceid.md)
    
## <a name="getsearchablemailboxes-operation-error-response"></a>Resposta de erro da operação GetSearchableMailboxes

O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **GetSearchableMailboxes.** Esta é uma resposta a uma solicitação para obter todas as caixas de correio pesquisáveis quando o **argumento ExpandGroupMembership** for definido como **true**. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526"
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetSearchableMailboxesResponse ResponseClass="Error" 
                                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Cannot use wildcard or empty query when auto group expansion is enabled.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         <SearchableMailboxes/>
      </GetSearchableMailboxesResponse>
   </s:Body>
</s:Envelope>

```

O corpo SOAP da resposta de erro contém os seguintes elementos:
  
- [GetSearchableMailboxesResponse](getsearchablemailboxesresponse.md)  
- [MessageText](messagetext.md)   
- [ResponseCode](responsecode.md)   
- [DescriptiveLinkKey](descriptivelinkkey.md) 
- [SearchableMailboxes](searchablemailboxes.md)
    
Para obter códigos de erro adicionais genéricos para EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>Confira também

- [Operações EWS em Exchange](ews-operations-in-exchange.md)   
- [Operação SetHoldOnMailboxes](setholdonmailboxes-operation.md)   
- [Operação SearchMailboxes](searchmailboxes-operation.md)   
- [Operação GetHoldOnMailboxes](getholdonmailboxes-operation.md)    
- [Operação GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration-operation.md)   
- [Operação GetNonIndexableItemDetails](getnonindexableitemdetails-operation.md)   
- [Operação GetNonIndexableItemStatistics](getnonindexableitemstatistics-operation.md)
    

