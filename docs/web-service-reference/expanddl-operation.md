---
title: Operação ExpandDL
manager: sethgros
ms.date: 07/27/2018
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ExpandDL
api_type:
- schema
ms.assetid: 1f7837e7-9eff-4e10-9577-c40f7ed6af94
description: A operação ExpandDL expõe a associação completa das listas de distribuição.
ms.openlocfilehash: 9878ecff0eeee1ef386c7bb26a092eec47f471de
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513777"
---
# <a name="expanddl-operation"></a>Operação ExpandDL

A operação ExpandDL expõe a associação completa das listas de distribuição.
  
## <a name="using-the-expanddl-web-method"></a>Usando o método Web ExpandDL

A operação ExpandDL usa o serviço Web localizado em Exchange.asmx. Este método de serviço Web aceita um elemento [Mailbox](mailbox.md) que pode conter um [elemento filho EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) para uma expansão de uma lista de distribuição pública ou um [elemento filho ItemId](itemid.md) para a expansão de uma lista de distribuição privada. 
  
As listas de distribuição pública podem ser expandidas usando uma das seguintes:
  
1. Alias de lista de distribuição
    
2. O endereço do Protocolo SMTP Seguro
    
3. X400
    
4. X500
    
5. Exchange Endereço herddo
    
6. O nome da lista de distribuição
    
7. O nome para exibição
    
> [!IMPORTANT]
> Os nomes de exibição não são exclusivos. Várias contas podem compartilhar o mesmo nome de exibição. 
  
## <a name="remarks"></a>Comentários

Não há suporte para expansão recursiva. Somente uma lista de distribuição pode ser expandida em uma única chamada. Se mais de uma lista de distribuição corresponder aos critérios, o serviço Web relata um erro. Um aplicativo cliente pode usar anr (resolução de nome ambígua) para encontrar listas de distribuição ambíguas e, em seguida, escolher o endereço de email correto da lista de distribuição necessária como parâmetro para a operação [ExpandDL](expanddl-operation.md). Para obter mais informações, consulte [ResolveNames operation](resolvenames-operation.md).
  
As listas de distribuição pública estão localizadas no Active Directory. Eles podem ser qualquer grupo de distribuição dinâmico ou habilitado para email. O grupo não deve estar oculto da lista de endereços e cada membro deve ter um endereço de email não vazio. Os membros da lista de distribuição podem ser usuários habilitados para email e contatos, pastas públicas e listas de distribuição habilitadas para email e grupos dinâmicos.
  
Listas de distribuição privadas estão localizadas na pasta Contatos da caixa de correio de um usuário. As listas de distribuição privadas não têm endereços de email, portanto, os identificadores de item da loja são usados em uma solicitação ExpandDL. Membros de uma lista de distribuição privada podem ser qualquer usuário habilitado para email, contatos ou listas de distribuição do Active Directory ou contatos ou listas de distribuição privada da pasta Contatos de um usuário.
  
Para contatos ou listas de distribuição privadas, os identificadores de item são retornados na resposta. Isso pode ser usado para obter informações sobre o objeto ou expandir a associação em uma lista de distribuição privada.
  
## <a name="expanddl-private-distribution-list-request-example"></a>Exemplo de solicitação da Lista de Distribuição Privada expandDL

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

Para expandir uma lista de distribuição privada, o elemento [Mailbox](mailbox.md) conterá o [elemento ItemId](itemid.md) que identifica uma lista de distribuição privada na caixa de correio do usuário. 
  
## <a name="expanddl-public-distribution-list-request-example"></a>Exemplo de solicitação da Lista de Distribuição Pública expandDL

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

A resposta a essa solicitação conterá elementos **de Caixa** de Correio que identificam cada caixa de correio na lista de distribuição. Se uma lista de distribuição estiver contida em uma lista de distribuição, uma expansão de lista de distribuição separada deve ser executada na lista de distribuição incorporada. Se a lista de distribuição não tiver membros ou a lista de distribuição solicitada não existir, o atributo **ResponseClass** conterá um valor igual a Success. 
  
### <a name="request-elements"></a>Elementos request

Os seguintes elementos são usados na solicitação:
  
- [ExpandDL](expanddl.md)
    
- [Caixa de Correio](mailbox.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) é usado para identificar listas de distribuição pública. O [elemento ItemId](itemid.md) é usado para identificar listas de distribuição privadas. 
    
> [!NOTE]
> O esquema que descreve esses elementos está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem a função de servidor de Acesso para Cliente instalada. 
  
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
> O nome da lista de distribuição não está incluído na resposta; portanto, você deve manter o controle do nome da solicitação. 
  
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
    
- [Name (EmailAddressType)](name-emailaddresstype.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)
    
- [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md)
    
- [MailboxType](mailboxtype.md)
    
Para encontrar outras opções para a mensagem de resposta da operação ExpandDL, explore a hierarquia de esquema. Comece no [elemento ExpandDLResponse.](expanddlresponse.md) 
  
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
    
Para encontrar outras opções para a mensagem de resposta da operação ExpandDL, explore a hierarquia de esquema. Comece no [elemento ExpandDLResponse.](expanddlresponse.md) 
  
## <a name="see-also"></a>Confira também

- [Operação ResolveNames](resolvenames-operation.md)
- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

