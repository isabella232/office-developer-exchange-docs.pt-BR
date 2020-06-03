---
title: Operação ResolveNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolveNames
api_type:
- schema
ms.assetid: 6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb
description: A operação ResolveNames resolve endereços de email e nomes de exibição ambíguos.
ms.openlocfilehash: 51728addddd2bfb9d35b874ae8c11e83a4c8629b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468275"
---
# <a name="resolvenames-operation"></a>Operação ResolveNames

A operação **ResolveNames** resolve endereços de email e nomes de exibição ambíguos. 
  
## <a name="using-the-resolvenames-operation"></a>Usando a operação ResolveNames

Essa operação pode ser usada para verificar aliases e resolver nomes de exibição para o usuário de caixa de correio apropriado. Se houver nomes ambíguos, a resposta de operação **ResolveNames** fornecerá informações sobre cada usuário de caixa de correio para que o aplicativo cliente possa resolver os nomes. 
  
## <a name="remarks"></a>Comentários

A resposta ResolveNames retorna um máximo de 100 candidatos. Os candidatos 100 retornados são os primeiros 100 encontrados na operação de pesquisa.
  
Os endereços de email com tipos de roteamento prefixos, como SMTP ou SIP, são salvos em uma matriz de vários valores. A operação **ResolveNames** executa uma correspondência parcial em relação a cada valor dessa matriz quando você adiciona o tipo de roteamento no início do nome não resolvido, como "SIP:User1@Contoso.com". Se você não especificar um tipo de roteamento, **ResolveNames** usará como padrão o tipo de roteamento do SMTP, o corresponderá a uma propriedade de endereço SMTP primária e não pesquisará a matriz de vários valores. 
  
Apenas um nome ambíguo pode ser especificado em uma única solicitação. O Active Directory é pesquisado primeiro e, em seguida, a pasta de contatos do usuário é pesquisada. As entradas resolvidas da pasta de contatos de um usuário têm uma propriedade **ItemId** não nula, que pode ser usada em uma solicitação GetItem. Se for a ID de uma lista de distribuição privada, ela poderá ser usada em uma [operação ExpandDL](expanddl-operation.md). Se o atributo **ReturnFullContactData** for definido como **true**, as entradas do Active Directory localizadas com a operação **ResolveNames** retornarão propriedades adicionais que descrevem um [contato](contact.md). O atributo **ReturnFullContactData** não afeta os dados retornados para contatos e listas de distribuição privada da pasta de contatos do usuário. 
  
## <a name="resolvenames-request-example"></a>Exemplo de solicitação ResolveNames

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação **ResolveNames** mostra como resolver a entrada de User.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ResolveNames xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                  ReturnFullContactData="true">
      <UnresolvedEntry>User2</UnresolvedEntry>
    </ResolveNames>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comentários

A resposta a essa solicitação retornará todas as entradas que começam com "Jo" ou "mi". Os itens retornados são caixas de correio públicas, listas de distribuição pública e privada e contatos.
  
> [!NOTE]
> Somente os contatos na pasta contatos pessoais padrão são pesquisados. 
  
Estes são os resultados possíveis para uma solicitação **ResolveNames** : 
  
- As respostas que não contiverem uma entidade resolvida retornarão um valor de atributo **ResponseClass** igual a **erro**. O elemento **MessageText** conterá " **nenhum resultado encontrado**."
    
- As respostas que contenham uma única entidade resolvida retornarão um valor de atributo **ResponseClass** igual a **Success**.
    
- As respostas que contêm várias entidades possíveis retornarão um valor de atributo **ResponseClass** igual a **Warning**. Nesse caso, a entidade não pôde ser resolvida para uma identidade exclusiva. O elemento **MessageText** conterá "vários resultados encontrados." 
    
### <a name="request-elements"></a>Elementos Request

Os seguintes elementos são usados na solicitação:
  
- [ResolveNames](resolvenames.md)
    
- [UnresolvedEntry](unresolvedentry.md)
    
## <a name="successful-resolvenames-operation-response-example"></a>Exemplo de resposta de operação ResolveNames com êxito

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta bem-sucedida para uma solicitação **ResolveNames** . 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ResolveNamesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ResolutionSet TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Resolution>
              <t:Mailbox>
                <t:Name>User2</t:Name>
                <t:EmailAddress>User2@example.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Mailbox</t:MailboxType>
              </t:Mailbox>
              <t:Contact>
                <t:DisplayName>User2</t:DisplayName>
                <t:EmailAddresses>
                  <t:Entry Key="EmailAddress1">SMTP:User2@example.com</t:Entry>
                </t:EmailAddresses>
                <t:ContactSource>ActiveDirectory</t:ContactSource>
              </t:Contact>
            </t:Resolution>
          </m:ResolutionSet>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </ResolveNamesResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-resolvenames-response-elements"></a>Elementos de resposta resolvedos com êxito

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [ResolveNamesResponse](resolvenamesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResolveNamesResponseMessage](resolvenamesresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [ResolutionSet](resolutionset.md)
    
- [Resolução](resolution.md)
    
- [Caixa de Correio](mailbox.md)
    
- [Nome (EmailAddresstype)](name-emailaddresstype.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)
    
- [RoutingType (EmailAddresstype)](routingtype-emailaddresstype.md)
    
- [MailboxType](mailboxtype.md)
    
- [Contato](contact.md)
    
- [DisplayName (cadeia de caracteres)](displayname-string.md)
    
- [EmailAddresses](emailaddresses.md)
    
- [Entrada (EmailAddress)](entry-emailaddress.md)
    
- [Contato](contactsource.md)
    
## <a name="resolvenames-operation-error-response"></a>Resposta de erro de operação ResolveNames

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta de erro para uma solicitação **ResolveNames** . O erro é causado pela tentativa de resolver um nome que não pode ser resolvido. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ResolveNamesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Error">
          <m:MessageText>No results were found.</m:MessageText>
          <m:ResponseCode>ErrorNameResolutionNoResults</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </ResolveNamesResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Elementos de resposta de erro

Os seguintes elementos são usados na resposta de erro:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [ResolveNamesResponse](resolvenamesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResolveNamesResponseMessage](resolvenamesresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>Confira também



[Operação ExpandDL](expanddl-operation.md)


[Usando a resolução de nome](https://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

