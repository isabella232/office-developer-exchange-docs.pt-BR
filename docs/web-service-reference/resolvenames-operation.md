---
title: Operação ResolveNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ResolveNames
api_type:
- schema
ms.assetid: 6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb
description: A operação ResolveNames resolve endereços de email ambíguos e nomes de exibição.
ms.openlocfilehash: f5ab0e3ee23cc085d8aa425c6eeb0ac7c392b9bb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509445"
---
# <a name="resolvenames-operation"></a>Operação ResolveNames

A **operação ResolveNames** resolve endereços de email ambíguos e nomes de exibição. 
  
## <a name="using-the-resolvenames-operation"></a>Usando a operação ResolveNames

Essa operação pode ser usada para verificar aliases e resolver nomes de exibição para o usuário de caixa de correio apropriado. Se existirem nomes ambíguos, a resposta da operação **ResolveNames** fornece informações sobre cada usuário de caixa de correio para que o aplicativo cliente possa resolver os nomes. 
  
## <a name="remarks"></a>Comentários

A resposta ResolveNames retorna um máximo de 100 candidatos. Os 100 candidatos retornados são os primeiros 100 encontrados na operação de procurar.
  
Endereços de email com tipos de roteamento prefixados, como smtp ou sip, são salvos em uma matriz de vários valores. A **operação ResolveNames** executa uma combinação parcial com cada valor dessa matriz quando você adiciona o tipo de roteamento no início do nome não resolvido, como "sip:User1@Contoso.com". Se você não especificar um tipo de roteamento, **ResolveNames** será padrão para o tipo de roteamento de smtp, corresponderá a uma propriedade de endereço smtp principal e não pesquisará a matriz de vários valores. 
  
Somente um nome ambíguo pode ser especificado em uma única solicitação. O Active Directory é pesquisado primeiro e, em seguida, a pasta de contato do usuário é pesquisada. Entradas resolvidas da pasta de contato de um usuário têm uma **propriedade ItemId** não nula, que pode ser usada em uma solicitação GetItem. Se for a ID de uma lista de distribuição privada, ela poderá ser usada em uma [operação ExpandDL.](expanddl-operation.md) Se o **atributo ReturnFullContactData** estiver definido como **true**, as entradas do Active Directory encontradas com a operação **ResolveNames** retornarão propriedades adicionais que descrevem um [Contact](contact.md). O **atributo ReturnFullContactData** não afeta os dados retornados para contatos e listas de distribuição privadas da pasta de contato do usuário. 
  
## <a name="resolvenames-request-example"></a>Exemplo de solicitação ResolveNames

### <a name="description"></a>Descrição

O exemplo a seguir de uma **solicitação ResolveNames** mostra como resolver a entrada do Usuário.
  
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

A resposta a essa solicitação retornará todas as entradas que começam com "Jo" ou "Mi". Os itens retornados são caixas de correio públicas, listas de distribuição públicas e privadas e contatos.
  
> [!NOTE]
> Somente contatos na pasta contatos pessoais padrão são pesquisados. 
  
Veja a seguir os resultados possíveis para uma **solicitação ResolveNames:** 
  
- As respostas que não contêm uma entidade resolvida retornarão um valor de atributo **ResponseClass** igual a **Error**. O **elemento MessageText** conterá " **Nenhum resultado é encontrado**."
    
- As respostas que contêm uma única entidade resolvida retornarão um **valor de atributo ResponseClass** igual a **Success**.
    
- As respostas que contêm várias entidades possíveis retornarão um **valor de atributo ResponseClass** igual a **Warning**. Nesse caso, a entidade não pôde ser resolvida para uma identidade exclusiva. O **elemento MessageText** conterá "Vários resultados são encontrados". 
    
### <a name="request-elements"></a>Elementos request

Os seguintes elementos são usados na solicitação:
  
- [ResolveNames](resolvenames.md)
    
- [UnresolvedEntry](unresolvedentry.md)
    
## <a name="successful-resolvenames-operation-response-example"></a>Exemplo de resposta de operação ResolveNames bem-sucedida

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta bem-sucedida a uma **solicitação ResolveNames.** 
  
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

### <a name="successful-resolvenames-response-elements"></a>Elementos de resposta ResolveNames bem-sucedidos

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [ResolveNamesResponse](resolvenamesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResolveNamesResponseMessage](resolvenamesresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [ResolutionSet](resolutionset.md)
    
- [Resolução](resolution.md)
    
- [Caixa de Correio](mailbox.md)
    
- [Name (EmailAddressType)](name-emailaddresstype.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)
    
- [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md)
    
- [MailboxType](mailboxtype.md)
    
- [Contato](contact.md)
    
- [DisplayName (cadeia de caracteres)](displayname-string.md)
    
- [EmailAddresses](emailaddresses.md)
    
- [Entry (EmailAddress)](entry-emailaddress.md)
    
- [ContactSource](contactsource.md)
    
## <a name="resolvenames-operation-error-response"></a>Resposta de erro da operação ResolveNames

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta de erro a uma **solicitação ResolveNames.** O erro é causado pela tentativa de resolver um nome que não pode ser resolvido. 
  
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

