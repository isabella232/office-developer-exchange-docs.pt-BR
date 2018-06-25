---
title: Operação GetDiscoverySearchConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8a54a6dc-110c-4972-a8bc-5ddb43c4b857
description: Encontre informações sobre o EWS GetDiscoverySearchConfiguration operação.
ms.openlocfilehash: a50463e575bf5a4ffdafc357d91563b0ca0486f4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752457"
---
# <a name="getdiscoverysearchconfiguration-operation"></a>Operação GetDiscoverySearchConfiguration

Encontre informações sobre a operação de EWS **GetDiscoverySearchConfiguration** . 
  
A operação **GetDiscoverySearchConfiguration** retorna contém informações de configuração local, salvo pesquisas de descoberta e as caixas de correio que estão habilitadas para pesquisa de descoberta. 
  
This operation was introduced in Exchange Server 2013.
  
## <a name="using-the-getdiscoverysearchconfiguration-operation"></a>Usando a operação GetDiscoverySearchConfiguration

A operação **GetDiscoverySearchConfiguration** fornece informações de configuração de pesquisa de descoberta. Solicitações podem conter um ou mais dos seguintes argumentos: 
  
1. [SearchId](searchid.md) — identifica uma pesquisa de descoberta salvas. Se esse argumento for enviado na solicitação, os valores dos outros argumentos são ignorados. 
    
2. [ExpandGroupMembership](expandgroupmembership.md) — indica se a associação ao grupo for expandida na resposta. Um valor **true** indica que a associação de grupo é expandida para que todas as caixas de correio pesquisáveis são retornadas na resposta. Um valor **false** indica que somente o grupo será retornado na resposta. 
    
3. [InPlaceHoldConfigurationOnly](inplaceholdconfigurationonly.md) — indica se todas as caixas de correio pesquisáveis são retornadas além da configuração de bloqueio in-loco. Um valor **true** indica que apenas as configurações de bloqueio in-loco são devolvidas. Um valor **false** indica que todos os identificadores de caixa de correio pesquisável são retornados além dos identificadores de bloqueio in-loco. Se esse elemento não estiver presente, o comportamento padrão é o equivalente do valor **false**. 
    
### <a name="getdiscoverysearchconfiguration-operation-soap-headers"></a>Cabeçalhos SOAP GetDiscoverySearchConfiguration operação

A operação **GetDiscoverySearchConfiguration** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir. 
  
|**Nome de cabeçalho**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**ManagementRole** <br/> |[ManagementRole](managementrole.md) <br/> |Identifica as funções de servidor necessários para que o chamador para fazer a solicitação. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Este cabeçalho é aplicável a uma resposta.  <br/> |
   
## <a name="getdiscoverysearchconfiguration-operation-request-example-get-the-discovery-search-configuration-for-a-saved-search"></a>Exemplo de solicitação de operação GetDiscoverySearchConfiguration: Obtenha a configuração de pesquisa de descoberta para uma pesquisa salva

O exemplo a seguir de uma solicitação de operação **GetDiscoverySearchConfiguration** mostra como solicitar a configuração de pesquisas salvas chamada "MyDiscSearchFor sbrown". Os argumentos para os elementos de [InPlaceHoldConfigurationOnly](inplaceholdconfigurationonly.md) de [ExpandGroupMembership](expandgroupmembership.md) e serão ignorados. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetDiscoverySearchConfiguration>
         <m:SearchId>MyDiscSearchFor-sbrown</m:SearchId>
         <m:ExpandGroupMembership>true</m:ExpandGroupMembership>
         <m:InPlaceHoldConfigurationOnly>false</m:InPlaceHoldConfigurationOnly>
      </m:GetDiscoverySearchConfiguration>
   </soap:Body>
</soap:Envelope>

```

A solicitação de corpo SOAP contém os seguintes elementos:
  
- [GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration.md)
    
- [SearchId](searchid.md)
    
- [ExpandGroupMembership](expandgroupmembership.md)
    
- [InPlaceHoldConfigurationOnly](inplaceholdconfigurationonly.md)
    
## <a name="successful-getdiscoverysearchconfiguration-operation-response-request-for-a-single-saved-search"></a>Resposta bem-sucedida de operação GetDiscoverySearchConfiguration: solicitar para uma única pesquisa salva

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **GetDiscoverySearchConfiguration** para obter a configuração de pesquisas salvas chamada "MyDiscSearchFor sbrown". 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="526" MinorBuildNumber="0" Version="Exchange2013" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetDiscoverySearchConfigurationResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <DiscoverySearchConfigurations>
        <DiscoverySearchConfiguration xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <SearchId>MyDiscSearchFor-sbrown</SearchId>
          <SearchQuery>test item</SearchQuery>
          <SearchableMailboxes>
            <SearchableMailbox>
              <Guid>3c620d04-8b22-432e-92be-5b9321599576</Guid>
              <PrimarySmtpAddress>SBrown@contoso.com</PrimarySmtpAddress>
              <IsExternalMailbox>false</IsExternalMailbox>
              <ExternalEmailAddress/>
              <DisplayName>Steven Brown</DisplayName>
              <IsMembershipGroup>false</IsMembershipGroup>
              <ReferenceId>/o=First/ou=Exchange(FYDILT)/cn=Recipients/cn=313ecf-Steve</ReferenceId>
            </SearchableMailbox>
          </SearchableMailboxes>
        </DiscoverySearchConfiguration>
      </DiscoverySearchConfigurations>
    </GetDiscoverySearchConfigurationResponse>
  </s:Body>
</s:Envelope>
```

A resposta SOAP body contém os seguintes elementos:
  
- [GetDiscoverySearchConfigurationResponse](getdiscoverysearchconfigurationresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [DiscoverySearchConfigurations](discoverysearchconfigurations.md)
    
- [DiscoverySearchConfiguration](discoverysearchconfiguration.md)
    
- [SearchId](searchid.md)
    
- [SearchQuery](searchquery.md)
    
- [SearchableMailboxes](searchablemailboxes.md)
    
- [SearchableMailbox](searchablemailbox.md)
    
- [GUID](guid-ex15websvcsotherref.md)
    
- [PrimarySmtpAddress (string)](primarysmtpaddress-string.md)
    
- [IsExternalMailbox](isexternalmailbox.md)
    
- [ExternalEmailAddress](externalemailaddress.md)
    
- [DisplayName (string)](displayname-string.md)
    
- [IsMembershipGroup](ismembershipgroup.md)
    
- [ID de referência](referenceid.md)
    
## <a name="successful-getdiscoverysearchconfiguration-operation-response-request-for-in-place-holds"></a>Resposta bem-sucedida de operação GetDiscoverySearchConfiguration: a solicitação de retenções locais

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **GetDiscoverySearchConfiguration** obter somente in-loco contém. 
  
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
      <GetDiscoverySearchConfigurationResponse ResponseClass="Success" 
                                               xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <DiscoverySearchConfigurations>
            <DiscoverySearchConfiguration xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <SearchId>MyDiscSearchFor-sbrown</SearchId>
               <SearchQuery>test item</SearchQuery>
               <InPlaceHoldIdentity>3f37d90f53144558a80814ef0272749a9</InPlaceHoldIdentity>
               <ManagedByOrganization/>
            </DiscoverySearchConfiguration>
            <DiscoverySearchConfiguration xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <SearchId>MyDiscSearch</SearchId>
               <SearchQuery>test</SearchQuery>
               <InPlaceHoldIdentity>6ea486f0f3f140efb044682a2e782abdf</InPlaceHoldIdentity>
               <ManagedByOrganization/>
            </DiscoverySearchConfiguration>
         </DiscoverySearchConfigurations>
      </GetDiscoverySearchConfigurationResponse>
   </s:Body>
</s:Envelope>

```

A resposta SOAP body contém os seguintes elementos:
  
- [GetDiscoverySearchConfigurationResponse](getdiscoverysearchconfigurationresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [DiscoverySearchConfigurations](discoverysearchconfigurations.md)
    
- [DiscoverySearchConfiguration](discoverysearchconfiguration.md)
    
- [SearchId](searchid.md)
    
- [SearchQuery](searchquery.md)
    
- [InPlaceHoldIdentity](inplaceholdidentity.md)
    
- [ManagedByOrganization](managedbyorganization.md)
    
## <a name="successful-getdiscoverysearchconfiguration-operation-response-request-for-all-saved-discovery-search-configurations"></a>Resposta bem-sucedida de operação GetDiscoverySearchConfiguration: a solicitação de todas as salvas descoberta de configurações de pesquisa

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **GetDiscoverySearchConfiguration** para obter todas as pesquisas de descoberta salvas. 
  
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
      <GetDiscoverySearchConfigurationResponse ResponseClass="Success" 
                                               xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <DiscoverySearchConfigurations>
            <DiscoverySearchConfiguration xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <SearchId>MyDiscSearchFor-sbrown</SearchId>
               <SearchQuery>test item</SearchQuery>
               <SearchableMailboxes>
                  <SearchableMailbox>
                     <Guid>3c620d04-8b33-435e-95be-5b9351599576</Guid>
                     <PrimarySmtpAddress>SBrown@contoso.com</PrimarySmtpAddress>
                     <IsExternalMailbox>false</IsExternalMailbox>
                     <ExternalEmailAddress/>
                     <DisplayName>Steven Brown</DisplayName>
                     <IsMembershipGroup>false</IsMembershipGroup>
                     <ReferenceId>/o=First/ou=Exchange (FYLT)/cn=Recipients/cn=35381a742f0e47e395c8601a60d13ecz-Steve</ReferenceId>
                  </SearchableMailbox>
               </SearchableMailboxes>
            </DiscoverySearchConfiguration>
            <DiscoverySearchConfiguration xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <SearchId>MyDiscSearch</SearchId>
               <SearchQuery>test</SearchQuery>
               <SearchableMailboxes>
                  <SearchableMailbox>
                     <Guid>e788c4b0-54a2-458c-83b2-22d5bb02b23f</Guid>
                     <PrimarySmtpAddress>Administrator@contoso.com</PrimarySmtpAddress>
                     <IsExternalMailbox>false</IsExternalMailbox>
                     <ExternalEmailAddress/>
                     <DisplayName>Administrator</DisplayName>
                     <IsMembershipGroup>false</IsMembershipGroup>
                     <ReferenceId>/o=First/ou=Exchange (FYLT)/cn=Recipients/cn=ebez7871332d4595abe1c62962911a58-Admin</ReferenceId>
                  </SearchableMailbox>
                  <SearchableMailbox>
                     <Guid>6f6cff39-8967-4a60-b43f-328413c25199</Guid>
                     <PrimarySmtpAddress>ADavis@contoso.com</PrimarySmtpAddress>
                     <IsExternalMailbox>false</IsExternalMailbox>
                     <ExternalEmailAddress/>
                     <DisplayName>Anthony Davis</DisplayName>
                     <IsMembershipGroup>false</IsMembershipGroup>
                     <ReferenceId>/o=First/ou=Exchange (FYLT)/cn=Recipients/cn=f10c9f70519844beb04101d8f40c572z-Antho</ReferenceId>
                  </SearchableMailbox>
               </SearchableMailboxes>
            </DiscoverySearchConfiguration>
         </DiscoverySearchConfigurations>
      </GetDiscoverySearchConfigurationResponse>
   </s:Body>
</s:Envelope>
```

A resposta SOAP body contém os seguintes elementos:
  
- [GetDiscoverySearchConfigurationResponse](getdiscoverysearchconfigurationresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [DiscoverySearchConfigurations](discoverysearchconfigurations.md)
    
- [DiscoverySearchConfiguration](discoverysearchconfiguration.md)
    
- [SearchId](searchid.md)
    
- [SearchQuery](searchquery.md)
    
- [SearchableMailboxes](searchablemailboxes.md)
    
- [SearchableMailbox](searchablemailbox.md)
    
- [GUID](guid-ex15websvcsotherref.md)
    
- [PrimarySmtpAddress (string)](primarysmtpaddress-string.md)
    
- [IsExternalMailbox](isexternalmailbox.md)
    
- [ExternalEmailAddress](externalemailaddress.md)
    
- [DisplayName (string)](displayname-string.md)
    
- [IsMembershipGroup](ismembershipgroup.md)
    
- [ID de referência](referenceid.md)
    
## <a name="getdiscoverysearchconfiguration-operation-error-response"></a>Resposta de erro de operação GetDiscoverySearchConfiguration

O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **GetDiscoverySearchConfiguration** . Esta é uma resposta a uma solicitação para fazer uma pesquisa salva que não for encontrada no servidor. 
  
```XML
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
      <GetDiscoverySearchConfigurationResponse ResponseClass="Error" 
                                               xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Search configuration corresponding to the search id was not found.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         <DiscoverySearchConfigurations/>
      </GetDiscoverySearchConfigurationResponse>
   </s:Body>
</s:Envelope>

```

A resposta de erro corpo SOAP contém os seguintes elementos:
  
- [GetDiscoverySearchConfigurationResponse](getdiscoverysearchconfigurationresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [DiscoverySearchConfigurations](discoverysearchconfigurations.md)
    
Para códigos de erro adicionais que são genérica do EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>Confira também

- [Operações do EWS no Exchange](ews-operations-in-exchange.md)
    
- [GetSearchableMailboxes](getsearchablemailboxes.md)
    
- [SearchMailboxes](searchmailboxes.md)
    
- [GetHoldOnMailboxes](getholdonmailboxes.md)
    
- [SetHoldOnMailboxes](setholdonmailboxes.md)
    
- [GetNonIndexableItemDetails](getnonindexableitemdetails.md)
    
- [GetNonIndexableItemStatistics](getnonindexableitemstatistics.md)
    

