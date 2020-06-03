---
title: Operação FindPeople
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 446106b7-ff2d-4107-90c1-29f4d38ba128
description: Encontre informações sobre a operação do EWS do FindPeople.
ms.openlocfilehash: ab5edc3f140e34123ce1f009c401ddd61a0e2598
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462905"
---
# <a name="findpeople-operation"></a>Operação FindPeople

Encontre informações sobre a operação do EWS do **FindPeople** . 
  
A operação **FindPeople** retorna todos os objetos persona de uma pasta de contatos especificada ou recupera contatos que correspondem a uma cadeia de caracteres de consulta especificada. 
  
This operation was introduced in Exchange Server 2013.
  
## <a name="using-the-findpeople-operation"></a>Usando a operação FindPeople

A operação **FindPeople** retorna informações de contato agregadas. 
  
A operação **FindPeople** cria a funcionalidade existente dos tipos complexos [Restriction](restriction.md) e [BaseShape](baseshape.md) adicionando uma restrição de agregação e a capacidade de retornar propriedades adicionais. Usando uma restrição, um cliente pode especificar filtros, como "somente resultados de retorno que têm um endereço de mensagens instantâneas". O comportamento de pesquisa padrão é direcionado para a caixa de correio pessoal e a lista de endereços global (GAL) do usuário especificado. Ao pesquisar a GAL como a pasta de pesquisa principal, você deve especificar uma cadeia de caracteres de consulta em vez de uma restrição, porque essa operação não permite a navegação da GAL. 
  
### <a name="findpeople-operation-soap-headers"></a>Cabeçalhos SOAP de operação FindPeople

A operação **FindPeople** pode usar os cabeçalhos SOAP listados na tabela a seguir. 
  
|**Nome de cabeçalho**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**Representação** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifica o usuário que o aplicativo cliente está representando. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Este cabeçalho é aplicável a uma resposta.  <br/> |
   
## <a name="findpeople-operation-request-example"></a>Exemplo de solicitação de operação FindPeople

O exemplo a seguir de uma solicitação de operação **FindPeople** mostra como retornar os primeiros 100 contatos da pasta contatos. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:FindPeople>
         <m:IndexedPageItemView BasePoint="Beginning" MaxEntriesReturned="100" Offset="0"/>
         <m:ParentFolderId>
            <t:DistinguishedFolderId Id="contacts"/>
         </m:ParentFolderId>
      </m:FindPeople>
   </soap:Body>
</soap:Envelope>
```

O corpo SOAP de solicitação contém os seguintes elementos:
  
- [FindPeople](findpeople.md)
    
- [IndexedPageItemView](indexedpageitemview.md)
    
- [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
O exemplo a seguir de uma solicitação de operação **FindPeople** mostra como retornar os primeiros 100 contatos da GAL usando uma cadeia de caracteres de consulta. A configuração do **DistinguishedFolderId** como "Directory" pesquisará a GAL como a principal fonte de personas. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
    <m:FindPeople>
      <m:PersonaShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="persona:DisplayName"/>
          <t:FieldURI FieldURI="persona:Title"/>
        </t:AdditionalProperties>
      </m:PersonaShape>
      <m:IndexedPageItemView BasePoint="Beginning" MaxEntriesReturned="100" Offset="0"/>
      <m:ParentFolderId>
        <t:DistinguishedFolderId Id="directory"/>
      </m:ParentFolderId>
      <m:QueryString>adams</m:QueryString>
    </m:FindPeople>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-findpeople-operation-response"></a>Resposta de operação FindPeople bem-sucedida

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **FindPeople** . 
  
```XML
<?xml version="1.0" encoding="utf-8"?><s:Envelope 
   xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="349" 
                         MinorBuildNumber="0" 
                         Version="Exchange2013" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <FindPeopleResponse ResponseClass="Success" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <People>
        <Persona xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <PersonaId Id="AAQkAGQ1MjJjMTBkLTc4Y2UtNDA5Ny04ZjU5LWI3MTYzNGNkZmRkYQAQAOjFqObcLmtOlzlRnHdXQjo=" />
          <CreationTime>2012-01-11T22:25:37Z</CreationTime>
          <DisplayName>Terry Adams</DisplayName>
          <DisplayNameFirstLast>Terry Adams</DisplayNameFirstLast>
          <DisplayNameLastFirst>Adams Terry</DisplayNameLastFirst>
          <FileAs>Adams, Terry</FileAs>
          <GivenName>Terry</GivenName>
          <Surname>Adams</Surname>
          <EmailAddress>
            <Name>terry@litwareinc.com</Name>
            <EmailAddress>terry@litwareinc.com</EmailAddress>
            <RoutingType>SMTP</RoutingType>
          </EmailAddress>
          <EmailAddresses>
            <EmailAddress>
              <Name>terry@litwareinc.com</Name>
              <EmailAddress>terry@litwareinc.com</EmailAddress>
              <RoutingType>SMTP</RoutingType>
            </EmailAddress>
            <EmailAddress>
              <Name>tadams@contoso.com</Name>
              <EmailAddress>tadams@contoso.com</EmailAddress>
              <RoutingType>SMTP</RoutingType>
            </EmailAddress>
          </EmailAddresses>
          <RelevanceScore>2147483647</RelevanceScore>
        </Persona>
      </People>
      <TotalNumberOfPeopleInView>1</TotalNumberOfPeopleInView>
    </FindPeopleResponse>
  </s:Body>
</s:Envelope>
```

O corpo SOAP de resposta contém os seguintes elementos:
  
- [FindPeopleResponse](findpeopleresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [Pessoas](people.md)
    
- [Pessoal](persona.md)
    
- [Personaid](personaid.md)
    
- [CreationTime](creationtime.md)
    
- [DisplayName (cadeia de caracteres)](displayname-string.md)
    
- [DisplayNameFirstLast](displaynamefirstlast.md)
    
- [DisplayNameLastFirst](displaynamelastfirst.md)
    
- [FileAs](fileas.md)
    
- [GivenName](givenname.md)
    
- [Sobrenome](surname.md)
    
- [EmailAddresses (ArrayOfEmailAddressesType)](emailaddresses-arrayofemailaddressestype.md)
    
- [EmailAddress (EmailAddresstype)](emailaddress-emailaddresstype.md)
    
- [Nome (EmailAddresstype)](name-emailaddresstype.md)
    
- [EmailAddress (EmailAddresstype)](emailaddress-emailaddresstype.md)
    
- [RoutingType (EmailAddresstype)](routingtype-emailaddresstype.md)
    
- [RelevanceScore](relevancescore.md)
    
- [TotalNumberOfPeopleInView](totalnumberofpeopleinview.md)
    
## <a name="findpeople-operation-error-response"></a>Resposta de erro de operação FindPeople

Para códigos de erro genéricos para EWS, confira [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>Confira também

- [Pessoas e contatos no EWS no Exchange](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [Operação getpersona](getpersona-operation.md)
    

