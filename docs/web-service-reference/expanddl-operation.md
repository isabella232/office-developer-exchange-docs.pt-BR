---
title: Operação ExpandDL
manager: sethgros
ms.date: 07/27/2018
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExpandDL
api_type:
- schema
ms.assetid: 1f7837e7-9eff-4e10-9577-c40f7ed6af94
description: A operação ExpandDL expõe a associação completa de listas de distribuição.
ms.openlocfilehash: 8edaf057538e2c1136465f0ff7937c14477b2c47
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44454047"
---
# <a name="expanddl-operation"></a>Operação ExpandDL

A operação ExpandDL expõe a associação completa de listas de distribuição.
  
## <a name="using-the-expanddl-web-method"></a>Usando o método Web ExpandDL

A operação ExpandDL usa o serviço Web localizado no Exchange. asmx. Este método de serviço Web aceita um elemento de [caixa de correio](mailbox.md) que pode conter um elemento filho [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) para uma expansão de uma lista de distribuição pública ou um elemento filho [ItemId](itemid.md) para a expansão de uma lista de distribuição privada. 
  
As listas de distribuição pública podem ser expandidas usando um dos seguintes:
  
1. Alias da lista de distribuição
    
2. O endereço do Protocolo SMTP Seguro
    
3. X400
    
4. X500
    
5. Endereço herdado do Exchange
    
6. O nome da lista de distribuição
    
7. O nome de exibição
    
> [!IMPORTANT]
> Os nomes de exibição não são exclusivos. Várias contas podem compartilhar o mesmo nome de exibição. 
  
## <a name="remarks"></a>Comentários

A expansão recursiva não é suportada. Apenas uma lista de distribuição pode ser expandida em uma única chamada. Se mais de uma lista de distribuição corresponder aos critérios, o serviço Web relatará um erro. Um aplicativo cliente pode usar a ANR (resolução de nomes ambíguos) para localizar listas de distribuição ambíguas e, em seguida, escolher o endereço de email correto da lista de distribuição necessária como um parâmetro para a [operação ExpandDL](expanddl-operation.md). Para obter mais informações, consulte [ResolveNames Operation](resolvenames-operation.md).
  
As listas de distribuição pública estão localizadas no Active Directory. Eles podem ser qualquer grupo de distribuição dinâmico ou habilitado para email. O grupo não deve ser oculto na lista de endereços e cada membro deve ter um endereço de email não vazio. Os membros da lista de distribuição podem ser usuários e contatos habilitados para email, pastas públicas e listas de distribuição habilitadas para email e grupos dinâmicos.
  
As listas de distribuição privadas estão localizadas na pasta contatos da caixa de correio de um usuário. As listas de distribuição privada não têm endereços de email para que seus identificadores de item de repositório sejam usados em uma solicitação ExpandDL. Os membros de uma lista de distribuição privada podem ser qualquer usuário habilitado para email, contatos ou listas de distribuição do Active Directory ou de contatos ou listas de distribuição privada da pasta contatos de um usuário.
  
Para contatos ou listas de distribuição privadas, os identificadores de item são retornados na resposta. Isso pode ser usado para obter informações sobre o objeto ou para expandir a associação em uma lista de distribuição privada.
  
## <a name="expanddl-private-distribution-list-request-example"></a>Exemplo de solicitação de lista de distribuição privada ExpandDL

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação ExpandDL mostra como formar uma solicitação para expandir uma lista de distribuição privada.
  
### <a name="code"></a>Código

```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
  </soap:Header>
  <soap:Body>
    <m:ExpandDL>
      <m:Mailbox>
       <t:EmailAddress>test</t:EmailAddress>
      </m:Mailbox>
    </m:ExpandDL>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comentários

Para expandir uma lista de distribuição privada, o elemento [Mailbox](mailbox.md) conterá o elemento [ItemId](itemid.md) que identifica uma lista de distribuição privada na caixa de correio do usuário. 
  
## <a name="expanddl-public-distribution-list-request-example"></a>Exemplo de solicitação de lista de distribuição pública do ExpandDL

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação ExpandDL mostra como formar uma solicitação para expandir uma lista de distribuição pública. O exemplo mostra o uso de um nome de exibição para expandir uma lista de distribuição.
  
### <a name="code"></a>Código

```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
        <t:Mailbox>
          <t:EmailAddress>TheDistributionList</t:EmailAddress>
        </t:Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comentários

A resposta a essa solicitação conterá elementos de **caixa de correio** que identificam cada caixa de correio na lista de distribuição. Se uma lista de distribuição estiver contida em uma lista de distribuição, uma expansão de lista de distribuição separada deverá ser executada na lista de distribuição incorporada. Se a lista de distribuição não tiver membros ou a lista de distribuição solicitada não existir, o atributo **ResponseClass** conterá um valor igual a Success. 
  
### <a name="request-elements"></a>Elementos Request

Os seguintes elementos são usados na solicitação:
  
- [ExpandDL](expanddl.md)
    
- [Caixa de Correio](mailbox.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) é usado para identificar listas de distribuição públicas. O elemento [ItemId](itemid.md) é usado para identificar listas de distribuição privadas. 
    
> [!NOTE]
> O esquema que descreve esses elementos está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem a função de servidor de acesso para Cliente instalada. 
  
## <a name="successful-expanddl-response-example"></a>Exemplo de resposta ExpandDL bem-sucedida

### <a name="description"></a>Descrição

O exemplo a seguir de uma resposta ExpandDL mostra uma resposta à solicitação descrita acima. A expansão da lista de distribuição descreve o seguinte: 
  
- O número de membros da lista de distribuição que são retornados na resposta.
    
- Se a resposta contém todos os membros da lista de distribuição.
    
- O nome da caixa de correio.
    
- O endereço de email da caixa de correio.
    
- O tipo de roteamento para a caixa de correio.
    
- O tipo de caixa de correio.
    
> [!NOTE]
> O nome da lista de distribuição não está incluído na resposta; Portanto, você deve acompanhar o nome da solicitação. 
  
### <a name="code"></a>Código

```xml
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ExpandDLResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ExpandDLResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DLExpansion TotalItemsInView="3" IncludesLastItemInRange="true">
            <t:Mailbox>
              <t:Name>Dan Park</t:Name>
              <t:EmailAddress>dpark@exampledomain.com</t:EmailAddress>
              <t:RoutingType>SMTP</t:RoutingType>
              <t:MailboxType>Mailbox</t:MailboxType>
            </t:Mailbox>
            <t:Mailbox>
              <t:Name>Jeff Price</t:Name>
              <t:EmailAddress>jprice@exampledomain.com</t:EmailAddress>
              <t:RoutingType>SMTP</t:RoutingType>
              <t:MailboxType>Mailbox</t:MailboxType>
            </t:Mailbox>
            <t:Mailbox>
              <t:Name>Tanja Plate</t:Name>
              <t:EmailAddress>tplate@exampledomain.com</t:EmailAddress>
              <t:RoutingType>SMTP</t:RoutingType>
              <t:MailboxType>Mailbox</t:MailboxType>
            </t:Mailbox>
          </m:DLExpansion>
        </m:ExpandDLResponseMessage>
      </m:ResponseMessages>
    </ExpandDLResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a>Elementos de resposta bem-sucedidos

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [ExpandDLResponse](expanddlresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ExpandDLResponseMessage](expanddlresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [DLExpansion](dlexpansion.md)
    
- [Caixa de Correio](mailbox.md)
    
- [Nome (EmailAddresstype)](name-emailaddresstype.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)
    
- [RoutingType (EmailAddresstype)](routingtype-emailaddresstype.md)
    
- [MailboxType](mailboxtype.md)
    
Para encontrar outras opções para a mensagem de resposta da operação ExpandDL, explore a hierarquia do esquema. Inicie no elemento [ExpandDLResponse](expanddlresponse.md) . 
  
## <a name="expanddl-error-response"></a>Resposta de erro ExpandDL

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta de erro a uma solicitação ExpandDL.
  
### <a name="code"></a>Código

```xml
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ExpandDLResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ExpandDLResponseMessage ResponseClass="Error">
          <m:MessageText>No results are found.</m:MessageText>
          <m:ResponseCode>ErrorNameResolutionNoResults</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:ExpandDLResponseMessage>
      </m:ResponseMessages>
    </ExpandDLResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Elementos de resposta de erro

Os seguintes elementos são usados na resposta de erro:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [ExpandDLResponse](expanddlresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ExpandDLResponseMessage](expanddlresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
Para encontrar outras opções para a mensagem de resposta da operação ExpandDL, explore a hierarquia do esquema. Inicie no elemento [ExpandDLResponse](expanddlresponse.md) . 
  
## <a name="see-also"></a>Confira também

- [Operação ResolveNames](resolvenames-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

