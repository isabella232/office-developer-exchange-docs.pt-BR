---
title: Operação getpersona
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e2146df0-53d0-4caf-9758-b600bbc14b6a
description: Encontre informações sobre a operação do EWS GetPerson.
ms.openlocfilehash: 2b335c694a85f87c96432ea6d7c1c674613d2f17
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460943"
---
# <a name="getpersona-operation"></a>Operação getpersona

Encontre informações sobre a operação do EWS **GetPerson** . 
  
A operação **Getpersona** retorna um conjunto de propriedades que estão associadas a um persona. 
  
This operation was introduced in Exchange Server 2013.
  
## <a name="using-the-getpersona-operation"></a>Usando a operação getpersona

A operação **Getpersona** fornece acesso a informações de contato agregadas no formato de uma pessoa. O elemento [personaid](personaid.md) na solicitação identifica o persona a ser retornado na resposta. A resposta pode conter um conjunto padrão de propriedades persona ou um conjunto de propriedades personalizadas. Recomendamos que você especifique um conjunto de propriedades personalizadas para que as propriedades não usadas não sejam processadas e enviadas do servidor para o cliente. 
  
### <a name="getpersona-operation-soap-headers"></a>Cabeçalhos SOAP de operação getpersona

A operação **Getpersona** pode usar os cabeçalhos SOAP listados na tabela a seguir. 
  
|**Nome de cabeçalho**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**Representação** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifica o usuário que o aplicativo cliente está representando. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Este cabeçalho é aplicável a uma resposta.  <br/> |
   
## <a name="getpersona-operation-request-example-return-a-default-set-of-properties-for-a-persona"></a>Exemplo de solicitação de operação getpersona: retornar um conjunto padrão de propriedades de um persona

O exemplo a seguir de uma solicitação de operação **Getpersona** mostra como retornar um conjunto padrão de propriedades que estão associadas a um persona. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013"/>
   </soap:Header>
   <soap:Body xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <GetPersona>
         <PersonaId Id="AAQkADEzAQAKtOtR/l4MlLqHWORfhSYKU="/>
      </GetPersona>
   </soap:Body>
</soap:Envelope>

```

O corpo SOAP de resposta contém os seguintes elementos:
  
- [Getpersona](getpersona.md)
    
- [Personaid](personaid.md)
    
## <a name="successful-getpersona-operation-response"></a>Resposta de operação getpersona bem-sucedida

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **Getpersona** . 
  
> [!NOTE]
> Todos os identificadores de item e as chaves de alteração deste artigo foram reduzidos para preservar a legibilidade. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="432" 
                           MinorBuildNumber="5" 
                           Version="Exchange2013"
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                     xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
      xmlns:xsd="http://www.w3.org/2001/XMLSchema"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetPersonaResponseMessage ResponseClass="Success"
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <Persona>
            <PersonaId Id="AAQkADEzAQAKtOtR="
              xmlns="https://schemas.microsoft.com/exchange/services/2006/types"/>
            <PersonaType xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Person</PersonaType>
            <CreationTime xmlns="https://schemas.microsoft.com/exchange/services/2006/types">2012-06-01T17:00:34Z</CreationTime>
            <DisplayName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Brian Johnson</DisplayName>
            <DisplayNameFirstLast xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Brian Johnson</DisplayNameFirstLast>
            <DisplayNameLastFirst xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Johnson Brian</DisplayNameLastFirst>
            <FileAs xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Johnson, Brian</FileAs>
            <FileAsId xmlns="https://schemas.microsoft.com/exchange/services/2006/types">None</FileAsId>
            <GivenName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Brian</GivenName>
            <Surname xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Johnsoon</Surname>
            <CompanyName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Contoso</CompanyName>
            <RelevanceScore xmlns="https://schemas.microsoft.com/exchange/services/2006/types">4255550110</RelevanceScore>
            <Attributions xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <Attribution>
                  <Id>0</Id>
                  <SourceId Id="AAMkA =" ChangeKey="EQAAABY+"/>
                  <DisplayName>Outlook</DisplayName>
                  <IsWritable>true</IsWritable>
                  <IsQuickContact>false</IsQuickContact>
                  <IsHidden>false</IsHidden>
                  <FolderId Id="AAMkA=" ChangeKey="AQAAAA=="/>
               </Attribution>
            </Attributions>
            <DisplayNames xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Brian Johnson</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </DisplayNames>
            <FileAses xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Johnson, Brian</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </FileAses>
            <FileAsIds xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>None</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </FileAsIds>
            <GivenNames xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Brian</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </GivenNames>
            <Surnames xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Johnson</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </Surnames>
            <MobilePhones xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <PhoneNumberAttributedValue>
                  <Value>
                     <Number>(425)555-0110</Number>
                     <Type>Mobile</Type>
                  </Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </PhoneNumberAttributedValue>
            </MobilePhones>
            <CompanyNames xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Contoso</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </CompanyNames>
         </Persona>
      </GetPersonaResponseMessage>
   </s:Body>
</s:Envelope>

```

O corpo SOAP de resposta contém os seguintes elementos:
  
- GetPersonaResponseMessage
    
- [ResponseCode](responsecode.md)
    
- [Pessoal](persona.md)
    
- [Personaid](personaid.md)
    
- [Personatype](personatype.md)
    
- [CreationTime](creationtime.md)
    
- [DisplayNameFirstLast](displaynamefirstlast.md)
    
- [DisplayNameLastFirst](displaynamelastfirst.md)
    
- [FileAs](fileas.md)
    
- [FileAsId](fileasid.md)
    
- [GivenName](givenname.md)
    
- [Sobrenome](surname.md)
    
- [CompanyName](companyname.md)
    
- [RelevanceScore](relevancescore.md)
    
- [Atribuições (ArrayOfValueAttributionsType)](attributions-arrayofvalueattributionstype.md)
    
- [Atribuição (cadeia de caracteres)](attribution-string.md)
    
- [ID (cadeia de caracteres)](id-string.md)
    
- [SourceID](sourceid.md) SourceId 
    
- [DisplayName (cadeia de caracteres)](displayname-string.md)
    
- [Iswritable](iswritable.md)
    
- [IsQuickContact](isquickcontact.md)
    
- [IsHidden](ishidden.md)
    
- [FolderId](folderid.md)
    
- [Displaynames](displaynames.md)
    
- [StringAttributedValue](stringattributedvalue.md)
    
- [Valor (ArrayOfStringValueType)](value-arrayofstringvaluetype.md)
    
- [Atribuições (ArrayOfPersonaAttributionsType)](attributions-arrayofpersonaattributionstype.md)
    
- [Atribuição (PersonaAttributionType)](attribution-personaattributiontype.md)
    
- [FileAses](fileases.md)
    
- [FileAsIds](fileasids.md)
    
- [Dados fornecidos](givennames.md)
    
- [Sobrenomes](surnames.md)
    
- [MobilePhones](mobilephones.md)
    
- [PhoneNumberAttributedValue](phonenumberattributedvalue.md)
    
- [Valor (PersonaPhoneNumberType)](value-personaphonenumbertype.md)
    
- [Número](number.md)
    
- [Tipo (cadeia de caracteres)](type-string.md)
    
- [CompanyNames](companynames.md)
    
## <a name="getpersona-operation-error-response"></a>Resposta de erro de operação getpersona

O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **Getpersona** . Esta é uma resposta a uma solicitação que contém um identificador persona especificado incorretamente. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="578" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetPersonaResponseMessage ResponseClass="Error" 
                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Id is malformed.</MessageText>
         <ResponseCode>ErrorInvalidIdMalformed</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetPersonaResponseMessage>
   </s:Body>
</s:Envelope>
```

O corpo SOAP de resposta de erro contém os seguintes elementos:
  
- [GetPersonaResponseMessage](getpersonaresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
Para obter códigos de erro adicionais genéricos para o EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>Confira também

- [Operações do EWS no Exchange](ews-operations-in-exchange.md)
    
- [Pessoas e contatos no EWS no Exchange](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [Operação FindPeople](findpeople-operation.md)
    

