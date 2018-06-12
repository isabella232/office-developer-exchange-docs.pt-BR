---
title: Operação ExpandDL
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExpandDL
api_type:
- schema
ms.assetid: 1f7837e7-9eff-4e10-9577-c40f7ed6af94
description: A operação ExpandDL expõe a participação completa das listas de distribuição.
ms.openlocfilehash: e4654120881f81a79358e0e7c0ab016f94db3288
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752147"
---
# <a name="expanddl-operation"></a>Operação ExpandDL

A operação ExpandDL expõe a participação completa das listas de distribuição.
  
## <a name="using-the-expanddl-web-method"></a>Usando o método ExpandDL da Web

A operação ExpandDL usa o serviço Web que está localizado em Exchange.asmx. Este método de serviço Web aceita um elemento de [caixa de correio](mailbox.md) que pode conter um elemento filho de [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) uma expansão de uma lista de distribuição pública ou um elemento filho de [ItemId](itemid.md) para a expansão de uma privada lista de distribuição. 
  
Listas de distribuição pública podem ser expandidas usando um destes procedimentos:
  
1. Alias de lista de distribuição
    
2. O endereço de Simple Mail Transfer Protocol (SMTP)
    
3. X400
    
4. X500
    
5. Endereço herdado do Exchange
    
6. O nome da lista de distribuição
    
7. O nome para exibição
    
> [!IMPORTANT]
> Nomes de exibição não são exclusivos. Várias contas podem compartilhar o mesmo nome de exibição. 
  
## <a name="remarks"></a>Coment�rios

Expansão recursiva não é suportado. Lista de distribuição apenas um pode ser expandida em uma única chamada. Se mais de uma lista de distribuição corresponde aos critérios, o serviço Web relata um erro. Um aplicativo cliente pode usar a resolução de nome ambígua (ANR) para localizar a lista de distribuição ambígua e, em seguida, escolher o endereço de email correto da lista de distribuição necessários como um parâmetro para a [operação ExpandDL](expanddl-operation.md). Para obter mais informações, consulte [ResolveNames operação](resolvenames-operation.md).
  
Listas de distribuição pública estão localizadas no Active Directory. Eles podem ser qualquer grupo de distribuição dinâmico ou habilitados para email. O grupo não deve ser ocultado da lista de endereços e cada membro deve ter um endereço de email não vazias. Membros da lista de distribuição podem ser habilitado para email usuários e contatos, pastas públicas e listas de distribuição habilitado para email e grupos dinâmicos.
  
Listas de distribuição privada estão localizadas na pasta de contatos da caixa de correio do usuário. Listas de distribuição privada não têm endereços de email para que seus identificadores de item do repositório que são usados em uma solicitação de ExpandDL. Membros de uma lista de distribuição privada podem ser qualquer usuário habilitado para email, contatos ou listas de distribuição do Active Directory, ou listas de contatos ou distribuição particular da pasta de contatos do usuário.
  
Para os contatos ou listas de distribuição privada, os identificadores de item são retornados na resposta. Isso pode ser usado para obter informações sobre o objeto ou para expandir a associação em uma lista de distribuição particular.
  
## <a name="expanddl-private-distribution-list-request-example"></a>Exemplo de solicitação da lista de distribuição particular ExpandDL

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação de ExpandDL mostra como uma solicitação para expandir uma lista de distribuição particular de formulário.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
        <t:Mailbox>
          <t:ItemId Id="xASUAd==" ChangeKey="AAts0Q=="/>
        </t:Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comments

Para expandir uma lista de distribuição particular, o elemento de [caixa de correio](mailbox.md) conterá o elemento [ItemId](itemid.md) que identifica uma lista de distribuição particular na caixa de correio do usuário. 
  
## <a name="expanddl-public-distribution-list-request-example"></a>Exemplo de solicitação da lista de distribuição pública ExpandDL

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação de ExpandDL mostra como uma solicitação para expandir uma lista de distribuição pública de formulário. O exemplo mostra o uso de um nome de exibição para expandir uma lista de distribuição.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
        <t:Mailbox>
          <t:EmailAddress>TheDistributionList</t:EmailAddress>
        </t:Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comments

A resposta à solicitação conterá elementos de **caixa de correio** que identificam cada caixa de correio na lista de distribuição. Se uma lista de distribuição está contida em uma lista de distribuição, uma expansão de lista de distribuição separado deve ser executada na lista de distribuição incorporadas. Se a lista de distribuição não tem membros ou lista de distribuição solicitado não existir, o atributo **ResponseClass** conterá um valor igual ao sucesso. 
  
### <a name="request-elements"></a>Elementos de solicitação

Os seguintes elementos são usados na solicitação:
  
- [ExpandDL](expanddl.md)
    
- [Caixa de correio](mailbox.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) é usado para identificar as listas de distribuição pública. O elemento [ItemId](itemid.md) é usado para identificar as listas de distribuição particular. 
    
> [!NOTE]
> O esquema que descreve esses elementos está localizado no diretório virtual EWS do computador que está executando o MicrosoftExchange Server 2007 que possui a função de servidor acesso para cliente instalada. 
  
## <a name="successful-expanddl-response-example"></a>Exemplo de resposta bem-sucedida ExpandDL

### <a name="description"></a>Descrição

O exemplo a seguir de uma resposta ExpandDL mostra uma resposta à solicitação de descrito acima. A expansão de lista de distribuição descreve o seguinte: 
  
- O número de membros da lista de distribuição que são retornados na resposta.
    
- Se a resposta conterá todos os membros da lista de distribuição.
    
- O nome da caixa de correio.
    
- O endereço de email da caixa de correio.
    
- O tipo de roteamento da caixa de correio.
    
- O tipo de caixa de correio.
    
> [!NOTE]
> O nome da lista de distribuição não está incluído na resposta; Portanto, você deve ficar atento ao nome da solicitação. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ExpandDLResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-response-elements"></a>Elementos de resposta bem-sucedida

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [ExpandDLResponse](expanddlresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ExpandDLResponseMessage](expanddlresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [DLExpansion](dlexpansion.md)
    
- [Caixa de correio](mailbox.md)
    
- [Nome (EmailAddressType)](name-emailaddresstype.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)
    
- [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md)
    
- [MailboxType](mailboxtype.md)
    
Para localizar outras opções para a mensagem de resposta da operação ExpandDL, explore a hierarquia de esquema. Inicie o elemento [ExpandDLResponse](expanddlresponse.md) . 
  
## <a name="expanddl-error-response"></a>Resposta de erro ExpandDL

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta de erro a uma solicitação de ExpandDL.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ExpandDLResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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
    
Para localizar outras opções para a mensagem de resposta da operação ExpandDL, explore a hierarquia de esquema. Inicie o elemento [ExpandDLResponse](expanddlresponse.md) . 
  
## <a name="see-also"></a>Confira também

- [Operação ResolveNames](resolvenames-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

