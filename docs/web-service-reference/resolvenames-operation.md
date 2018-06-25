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
description: Os endereços de email ambíguo ResolveNames operação resolve e nomes para exibição.
ms.openlocfilehash: 8443cf834dfdf104daeaaa92fdee3742c3fa3719
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825162"
---
# <a name="resolvenames-operation"></a>Operação ResolveNames

Os endereços de email ambíguo **ResolveNames** operação resolve e nomes para exibição. 
  
## <a name="using-the-resolvenames-operation"></a>Usando a operação ResolveNames

Esta operação pode ser usada para verificar aliases e resolver nomes para exibição para o usuário de caixa de correio apropriado. Se nomes ambíguos existirem, a resposta de operação **ResolveNames** fornece informações sobre cada usuário de caixa de correio para que o aplicativo cliente possa resolver os nomes. 
  
## <a name="remarks"></a>Comentários

A resposta ResolveNames retorna um máximo de 100 candidatos. Os 100 candidatos que são retornados são os primeiros 100 encontradas na operação de pesquisa.
  
Endereços de email com tipos de roteamento de prefixados, como smtp ou sip, são salvas em uma matriz de valores múltiplos. A operação **ResolveNames** realiza uma correspondência parcial contra cada valor dessa matriz, quando você adiciona o tipo de roteamento no início do nome não resolvido, como "sip:User1@Contoso.com". Se você não especificar um tipo de roteamento, **ResolveNames** será o padrão para o tipo de roteamento de smtp, associá-lo a uma propriedade de endereço smtp principal e não pesquisar a matriz de valores múltiplos. 
  
Apenas um nome ambíguo pode ser especificado em uma única solicitação. Active Directory é pesquisado primeiro e, em seguida, a pasta de contato do usuário é pesquisada. Resolvido entradas da pasta de contato de um usuário tem uma propriedade de **ItemId** não-nulo, que pode ser usada em uma solicitação de GetItem. Se for a ID de uma lista de distribuição particular, pode ser usada em uma [operação ExpandDL](expanddl-operation.md). Se o atributo **ReturnFullContactData** for definido como **true**, entradas do Active Directory encontradas com a operação **ResolveNames** retornará propriedades adicionais que descrevem um [contato](contact.md). O atributo **ReturnFullContactData** não afeta os dados que são retornados para contatos e privadas listas de distribuição da pasta de contatos do usuário. 
  
## <a name="resolvenames-request-example"></a>Exemplo de solicitação ResolveNames

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação de **ResolveNames** mostra como resolver a entrada do usuário.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ResolveNames xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                  ReturnFullContactData="true">
      <UnresolvedEntry>User2</UnresolvedEntry>
    </ResolveNames>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comments

A resposta à solicitação retornará todas as entradas que começam com "Joana" ou "Mi". Os itens retornados são caixas de correio públicas, listas de distribuição pública e privada e contatos.
  
> [!NOTE]
> Somente os contatos da pasta Contatos pessoal padrão são pesquisados. 
  
Estes são os resultados possíveis para uma solicitação de **ResolveNames** : 
  
- Respostas que não contêm uma entidade resolvida retornará um valor de atributo **ResponseClass** igual a **erro**. O elemento **MessageText** conterá " **Nenhum resultado é encontrado**."
    
- As respostas que contêm uma única entidade resolvida retornará um valor de atributo **ResponseClass** igual ao **sucesso**.
    
- As respostas que contêm várias entidades possíveis retornará um valor de atributo **ResponseClass** igual a **Aviso**. Nesse caso, a entidade não pôde ser resolvida para uma identidade exclusiva. O elemento **MessageText** conterá "vários resultados encontrados." 
    
### <a name="request-elements"></a>Elementos de solicitação

Os seguintes elementos são usados na solicitação:
  
- [ResolveNames](resolvenames.md)
    
- [UnresolvedEntry](unresolvedentry.md)
    
## <a name="successful-resolvenames-operation-response-example"></a>Exemplo de resposta bem-sucedida da operação ResolveNames

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de **ResolveNames** . 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-resolvenames-response-elements"></a>Elementos de resposta bem-sucedida ResolveNames

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [ResolveNamesResponse](resolvenamesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResolveNamesResponseMessage](resolvenamesresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [ResolutionSet](resolutionset.md)
    
- [Resolução](resolution.md)
    
- [Caixa de correio](mailbox.md)
    
- [Nome (EmailAddressType)](name-emailaddresstype.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)
    
- [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md)
    
- [MailboxType](mailboxtype.md)
    
- [Contato](contact.md)
    
- [DisplayName (string)](displayname-string.md)
    
- [EmailAddresses](emailaddresses.md)
    
- [Entrada (EmailAddress)](entry-emailaddress.md)
    
- [ContactSource](contactsource.md)
    
## <a name="resolvenames-operation-error-response"></a>Resposta de erro de operação ResolveNames

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta de erro a uma solicitação de **ResolveNames** . O erro é causado por tentar resolver um nome que não pode ser resolvido. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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


[Usando a resolução de nome](http://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

