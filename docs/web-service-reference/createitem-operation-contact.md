---
title: Operação CreateItem (contato)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CreateItem
api_type:
- schema
ms.assetid: 417e994b-0a17-4c24-9527-04796b80b029
description: A operação CreateItem é usada para criar contatos no Exchange store.
ms.openlocfilehash: ced103046214830db868f4c62583e73297146d25
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545500"
---
# <a name="createitem-operation-contact"></a>Operação CreateItem (contato)

A operação CreateItem é usada para criar contatos no Exchange store.
  
## <a name="remarks"></a>Comentários

Não há suporte para a criação de listas de distribuição privadas. Todas as propriedades dentro do contêiner [CompleteName](completename.md) são somente leitura e não podem ser definidas em um item de contato. 
  
## <a name="createitem-request-example"></a>Exemplo de solicitação CreateItem

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação CreateItem SOAP válida mostra como criar um contato na pasta contatos padrão.
  
### <a name="code"></a>Código

```XML
<soap:Envelope
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" >
      <SavedItemFolderId>
        <t:DistinguishedFolderId Id="contacts"/>
      </SavedItemFolderId>
      <Items>
        <t:Contact>
          <t:FileAs>SampleContact</t:FileAs>
          <t:GivenName>Tanja</t:GivenName>
          <t:CompanyName>Blue Yonder Airlines</t:CompanyName>
          <t:EmailAddresses>
            <t:Entry Key="EmailAddress1">tplate@example.com</t:Entry>
          </t:EmailAddresses>
          <t:PhysicalAddresses>
            <t:Entry Key="Business">
              <t:Street>1234 56th Ave</t:Street>
              <t:City>La Habra</t:City>
              <t:State>CA</t:State>
              <t: CountryOrRegion>USA</t: CountryOrRegion>
            </t:Entry>
          </t:PhysicalAddresses>
          <t:PhoneNumbers>
            <t:Entry Key="BusinessPhone">4255550199</t:Entry>
          </t:PhoneNumbers>
          <t:JobTitle>Manager</t:JobTitle>
          <t:Surname>Plate</t:Surname>
        </t:Contact>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a>Elementos request

Os seguintes elementos são usados na resposta:
  
- [CreateItem](createitem.md)
    
- [SavedItemFolderId](saveditemfolderid.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md)
    
- [Contato](contact.md)
    
- [FileAs](fileas.md)
    
- [GivenName](givenname.md)
    
- [CompanyName](companyname.md)
    
- [EmailAddresses](emailaddresses.md)
    
- [Entry (EmailAddress)](entry-emailaddress.md)
    
- [PhysicalAddresses](physicaladdresses.md)
    
- [Entry (PhysicalAddress)](entry-physicaladdress.md)
    
- [Street](street.md)
    
- [Cidade](city.md)
    
- [State](state-ex15websvcsotherref.md)
    
- [CountryOrRegion](countryorregion.md)
    
- [PhoneNumbers](phonenumbers.md)
    
- [Entry (PhoneNumber)](entry-phonenumber.md)
    
- [JobTitle](jobtitle.md)
    
- [Sobrenome](surname.md)
    
## <a name="successful-createitem-request"></a>Solicitação CreateItem bem-sucedida

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta bem-sucedida à solicitação CreateItem que criou um contato. Neste exemplo, a resposta contém o identificador do item recém-criado.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Contact>
              <t:ItemId Id="AAAtA=" ChangeKey="EQAAAB" />
            </t:Contact>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comentários

O identificador de item foi reduzido para preservar a capacidade de leitura.
  
### <a name="successful-response-elements"></a>Elementos de resposta bem-sucedidos

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CreateItemResponse](createitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateItemResponseMessage](createitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md)
    
- [Contato](contact.md)
    
- [ItemId](itemid.md)
    
## <a name="invalid-createitem-request-example"></a>Exemplo de solicitação CreateItem inválida

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma solicitação que contém instruções XML válidas, mas incompatíveis. Um contato não pode ser criado em uma pasta de pesquisa.
  
### <a name="code"></a>Código

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns='https://schemas.microsoft.com/exchange/services/2006/messages'>
      <SavedItemFolderId>
        <t:DistinguishedFolderId Id='searchfolders'/>
      </SavedItemFolderId>
      <Items>
        <t:Contact>
          <t:ItemClass>IPM.Contact</t:ItemClass>
        </t:Contact>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="createitem-contact-error-response"></a>Resposta de erro CreateItem (Contato)

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta de erro a uma solicitação CreateItem (Contact).
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Error">
          <m:MessageText>Cannot create a contact in a non-contact Folder.</m:MessageText>
          <m:ResponseCode>ErrorCannotCreateContactInNonContactFolder</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Items />
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Elementos de resposta de erro

Os seguintes elementos são usados na resposta de erro:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CreateItemResponse](createitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateItemResponseMessage](createitemresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md)
    
## <a name="see-also"></a>Confira também



[Operação CreateItem](createitem-operation.md)

