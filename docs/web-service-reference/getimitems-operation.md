---
title: Operação GetImItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 51186691-46d2-4d5c-b8bc-4ee2bb20fbe7
description: Encontre informações sobre a operação do EWS do GetImItems.
ms.openlocfilehash: 960f4683dd478b0e5f8cf18fa8d1593b7433a249
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456042"
---
# <a name="getimitems-operation"></a>Operação GetImItems

Encontre informações sobre a operação do EWS do **GetImItems** . 
  
A operação **GetImItems** recupera informações sobre grupos de mensagens instantâneas (IM) e pessoas de contato de mensagens instantâneas. 
  
This operation was introduced in Exchange Server 2013.
  
## <a name="using-the-getimitems-operation"></a>Usando a operação GetImItems

A operação **GetImItems** aceita identificadores de item de contato e grupo e retorna um conjunto de informações sobre os grupos e contatos. Os conjuntos de propriedades retornados na resposta são identificados por propriedades estendidas, vários identificadores de contato, identificadores de grupo e definições de propriedades estendidas como argumentos. 
  
### <a name="getimitems-operation-soap-headers"></a>Cabeçalhos SOAP de operação GetImItems

A operação **GetImItems** pode usar os cabeçalhos SOAP listados na tabela a seguir. 
  
|**Nome de cabeçalho**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**Representação** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifica o usuário que o aplicativo cliente está representando. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifica a cultura, conforme definido na RFC 3066, "marcas de identificação de idiomas", a ser usado para acessar a caixa de correio. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Este cabeçalho é aplicável a uma resposta.  <br/> |
   
## <a name="getimitems-operation-request-example-get-detailed-information-about-im-contacts-and-groups"></a>Exemplo de solicitação de operação GetImItems: obter informações detalhadas sobre contatos e grupos de mensagens instantâneas

O exemplo a seguir de uma solicitação de operação do **GetImItems** mostra como solicitar informações detalhadas sobre contatos e grupos de mensagens instantâneas. Uma operação **GetImItems** pode solicitar um ou mais detalhes de contato ou grupo. Você também pode usar propriedades estendidas para obter propriedades personalizadas em grupos e contatos. Se uma propriedade estendida solicitada não existir em um item, a resposta irá ignorar a propriedade solicitada e retornará a resposta para o conjunto de propriedades padrão. Este exemplo mostra como obter o nome de exibição usando propriedades estendidas. 
  
> [!NOTE]
> Todos os identificadores de item e as chaves de alteração deste artigo foram reduzidos para preservar a legibilidade. Observe que as chaves de alteração são ignoradas pelo serviço para esta operação. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
   </soap:Header>
   <soap:Body >
      <m:GetImItems>
         <m:ContactIds>
            <t:ItemId Id="AAMkADEzOTExYACABmEhpSAAA=" ChangeKey="EQAAABBmNDjF"/>
         </m:ContactIds>
         <m:GroupIds>
            <t:ItemId Id="AAMkADEzOTExYjJkBY7+0EAAA=" ChangeKey="EgAAAA=="/>
         </m:GroupIds>         
         <m:ExtendedProperties>
            <t:ExtendedProperty PropertyTag="0x3001" PropertyType="String"/>
         </m:ExtendedProperties>
      </m:GetImItems>
   </soap:Body>
</soap:Envelope>
```

O corpo SOAP de solicitação contém os seguintes elementos:
  
- [GetImItems](getimitems.md)
    
- [ContactIds](contactids.md)
    
- [ItemId](itemid.md)
    
- [GroupIds](groupids.md)
    
- [ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)](extendedproperties-nonemptyarrayofextendedfielduris.md)
    
- [Extended (PathToExtendedFieldType)](extendedproperty-pathtoextendedfieldtype.md)
    
## <a name="successful-getimitems-operation-response"></a>Resposta de operação GetImItems bem-sucedida

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação do **GetImItems** para obter um contato de mensagens instantâneas e um grupo. O nome para exibição é solicitado em uma propriedade estendida. Os contatos de mensagens instantâneas são retornados no formato de uma pessoa. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetImItemsResponse ResponseClass="Success" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <ImItemList>
            <Groups xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <ImGroup>
                  <DisplayName>Exchange SDK Team</DisplayName>
                  <GroupType>IPM.DistList.MOC.UserGroup</GroupType>
                  <ExchangeStoreId Id="AAMkADEzQrAABY7+0EAAA=" ChangeKey="EgAAAA=="/>
                  <MemberCorrelationKey>
                     <ItemId Id="AAMkADEzOTExYjeGgGqm4QrAABmEhpSAAA=" ChangeKey="EQAAAA=="/>
                  </MemberCorrelationKey>
                  <ExtendedProperties>
                     <ExtendedProperty>
                        <ExtendedFieldURI PropertyTag="0x3001" PropertyType="String"/>
                        <Value>Exchange SDK Team</Value>
                     </ExtendedProperty>
                  </ExtendedProperties>
               </ImGroup>
            </Groups>
            <Personas xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <Persona>
                  <PersonaId Id="AAQkADEzOTBZImBzN5J/uHXc="/>
                  <PersonaType>Person</PersonaType>
                  <CreationTime>2012-11-07T00:10:35Z</CreationTime>
                  <DisplayName>Tony Smith</DisplayName>
                  <DisplayNameFirstLast>Tony Smith</DisplayNameFirstLast>
                  <DisplayNameLastFirst>Tony Smith</DisplayNameLastFirst>
                  <FileAs/>
                  <FileAsId>None</FileAsId>
                  <ImAddress>tsmith@contoso.com</ImAddress>
                  <RelevanceScore>2147483647</RelevanceScore>
                  <Attributions>
                     <Attribution>
                        <Id>0</Id>
                        <SourceId Id="AAMkADEzhQaoeGgGqm4QrAABmEhpSAAA=" ChangeKey="EQArAABmNDjF"/>
                        <DisplayName>Lync Contacts</DisplayName>
                        <IsWritable>false</IsWritable>
                        <IsQuickContact>true</IsQuickContact>
                        <IsHidden>false</IsHidden>
                     </Attribution>
                  </Attributions>
                  <DisplayNames>
                     <StringAttributedValue>
                        <Value>Tony Smith</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </DisplayNames>
                  <FileAsIds>
                     <StringAttributedValue>
                        <Value>None</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </FileAsIds>
                  <ImAddresses>
                     <StringAttributedValue>
                        <Value>tsmith@contoso.com</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </ImAddresses>
                  <ExtendedProperties>
                     <ExtendedPropertyAttributedValue>
                        <Value>
                           <ExtendedFieldURI PropertyTag="0x3001" PropertyType="String"/>
                           <Value>Tony Smith</Value>
                        </Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </ExtendedPropertyAttributedValue>
                  </ExtendedProperties>
               </Persona>
            </Personas>
         </ImItemList>
      </GetImItemsResponse>
   </s:Body>
</s:Envelope>
```

O corpo SOAP de resposta contém os seguintes elementos:
  
- [GetImItemsResponse](getimitemsresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [Imitemlist](imitemlist.md)
    
- [Grupos (ArrayOfImGroupType)](groups-arrayofimgrouptype.md)
    
- [Imgroup](imgroup.md)
    
- [DisplayName (cadeia de caracteres)](displayname-string.md)
    
- [GroupType](grouptype.md)
    
- [ExchangeStoreId](exchangestoreid.md)
    
- [MemberCorrelationKey](membercorrelationkey.md)
    
- [ItemId](itemid.md)
    
- [ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)](extendedproperties-nonemptyarrayofextendedfielduris.md)
    
- [Extended (PathToExtendedFieldType)](extendedproperty-pathtoextendedfieldtype.md)
    
- [Personas](personas-ex15websvcsotherref.md)
    
- [Personaid](personaid.md)
    
- [Personatype](personatype.md)
    
- [CreationTime](creationtime.md)
    
- [DisplayNameFirstLast](displaynamefirstlast.md)
    
- [DisplayNameLastFirst](displaynamelastfirst.md)
    
- [FileAs](fileas.md)
    
- [FileAsId](fileasid.md) FileAsId 
    
- [IMAddress (cadeia de caracteres)](imaddress-string.md)
    
- [RelevanceScore](relevancescore.md)
    
- [Atribuições (ArrayOfPersonaAttributionsType)](attributions-arrayofpersonaattributionstype.md)
    
- [Atribuição (PersonaAttributionType)](attribution-personaattributiontype.md)
    
- [ID (cadeia de caracteres)](id-string.md)
    
- [SourceId](sourceid.md)
    
- [Iswritable](iswritable.md)
    
- [IsQuickContact](isquickcontact.md)
    
- [IsHidden](ishidden.md)
    
- [StringAttributedValue](stringattributedvalue.md)
    
- [FileAsIds](fileasids.md)
    
- [Imendereços](imaddresses.md)
    
- [Valor (ExtendedPropertyType)](value-extendedpropertytype.md)
    
## <a name="getimitems-operation-error-response"></a>Resposta de erro de operação GetImItems

A operação **GetImItems** não valida identificadores e não retornará a resposta de erro **ErrorInvalidImContactId** ou **ErrorInvalidImGroupId** esperada se um identificador de contato ou de grupo inválido for fornecido ao serviço. 
  
## <a name="see-also"></a>Confira também

- [Operações do EWS no Exchange](ews-operations-in-exchange.md)
    
- [Operação GetImItemList](getimitemlist-operation.md)
    

