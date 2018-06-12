---
title: Operação MarkAsJunk
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1f71f04d-56a9-4fee-a4e7-d1034438329e
description: Encontre informações sobre o EWS MarkAsJunk operação.
ms.openlocfilehash: b9d79e6fbec87ce41030b4981f3c16f2f9ce9507
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824353"
---
# <a name="markasjunk-operation"></a>Operação MarkAsJunk

Encontre informações sobre a operação de EWS **MarkAsJunk** . 
  
A operação **MarkAsJunk** adiciona e remove usuários da lista de bloqueios de email e transfere mensagens de email para a pasta Lixo eletrônico. 
  
This operation was introduced in Exchange Server 2013.
  
## <a name="using-the-markasjunk-operation"></a>Usando a operação MarkAsJunk

A operação **MarkAsJunk** contém duas opções booleanas para indicar se um remetente do email deve ser adicionado à lista de remetentes bloqueados e se a mensagem de email de destino deve ser movida para a pasta de lixo eletrônico padrão ou a pasta de caixa de entrada. As ações são determinadas pelos valores dos atributos **IsJunk** e **MoveItem** . A seguir estão as ações possíveis com base nas combinações de valores para os atributos **IsJunk** e **MoveItem** : 
  
- Se o atributo **IsJunk** estiver definido como **true**e o atributo **MoveItem** estiver definido como **true**, o remetente da mensagem de email de destino é adicionado à lista de remetentes bloqueados e a mensagem de email é movida para a pasta de lixo eletrônico Dmail.
    
- Se o atributo **IsJunk** estiver definido como **true**e o atributo **MoveItem** estiver definido como **false**, o remetente da mensagem de email de destino é adicionado à lista de remetentes bloqueados e a mensagem de email não é movida da pasta.
    
- Se o atributo **IsJunk** está definido como **false**e o **MoveItem** atributo estiver definido como **true**, o remetente da messageis de email de destino removido da lista de remetentes bloqueados e a mensagem de email é movida para a pasta de caixa de entrada.
    
- Se o atributo **IsJunk** estiver definido como **false**e o atributo **MoveItem** estiver definido como **false**, o remetente da mensagem de email de destino é removido da lista de remetentes bloqueados e a mensagem de email não é movida da pasta.
    
> [!IMPORTANT]
> O conteúdo da lista de remetentes bloqueados não é detectável do EWS. Se um remetente é adicionado à lista de remetentes bloqueados, você precisa manter uma cópia de uma mensagem de email enviada pelo remetente bloqueado para desbloquear o remetente no futuro. 
  
### <a name="markasjunk-operation-soap-headers"></a>Cabeçalhos SOAP MarkAsJunk operação

A operação **MarkAsJunk** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir. 
  
|**Nome de cabeçalho**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**Representação** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifica o usuário que o aplicativo cliente está representando. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifica a cultura, conforme definido no RFC 3066, "Marcas para a identificação de idiomas", que será usada para acessar a caixa de correio. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Este cabeçalho é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Este cabeçalho é aplicável a uma resposta.  <br/> |
   
## <a name="markasjunk-operation-request-example-add-a-sender-to-the-blocked-sender-list"></a>Exemplo de solicitação de operação MarkAsJunk: adicionar um remetente à lista de remetentes bloqueados

O exemplo a seguir de uma solicitação de operação **MarkAsJunk** mostra como adicionar o remetente de um email à lista de remetentes bloqueados e mover o email para a pasta Lixo eletrônico. A operação **MarkAsJunk** aceita o identificador de mensagem de email exclusivo para identificar o email que é usado para referenciar o remetente que é adicionado à lista de remetentes bloqueados. 
  
> [!NOTE]
> Todos os identificadores de itens e teclas de alteração neste artigo foram diminuídas para preservar a legibilidade. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
    <soap:Header>
        <t:RequestServerVersion Version="Exchange2013" />
    </soap:Header>
    <soap:Body>
        <m:MarkAsJunk IsJunk="true" MoveItem="true">
            <m:ItemIds>
                <t:ItemId Id="AAMkAD=" ChangeKey="CQAAABYA" />
            </m:ItemIds>
        </m:MarkAsJunk>
    </soap:Body>
</soap:Envelope>

```

A solicitação de corpo SOAP contém os seguintes elementos:
  
- [MarkAsJunk](markasjunk.md)
    
- [ItemIds](itemids.md)
    
- [ItemId](itemid.md)
    
## <a name="successful-markasjunk-operation-response"></a>Resposta de operação MarkAsJunk bem-sucedida

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **MarkAsJunk** para adicionar um remetente à lista de remetentes bloqueados e mover a mensagem de email para a pasta Lixo eletrônico. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" 
                             MinorVersion="0" 
                             MajorBuildNumber="545" 
                             MinorBuildNumber="11" 
                             Version="Exchange2013" 
                             xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                             xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
            xmlns:xsd="http://www.w3.org/2001/XMLSchema">
        <m:MarkAsJunkResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
           <m:ResponseMessages>
               <m:MarkAsJunkResponseMessage ResponseClass="Success">
                  <m:ResponseCode>NoError</m:ResponseCode>
                 <m:MovedItemId Id="AAMkAD=" ChangeKey="CQAAABYu" />
               </m:MarkAsJunkResponseMessage>
           </m:ResponseMessages>
        </m:MarkAsJunkResponse>
    </s:Body>
</s:Envelope>
```

A resposta SOAP body contém os seguintes elementos:
  
- [MarkAsJunkResponse](markasjunkresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MarkAsJunkResponseMessage](markasjunkresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [MovedItemId](moveditemid.md)
    
## <a name="markasjunk-operation-request-example-remove-a-sender-from-the-blocked-sender-list"></a>Exemplo de solicitação de operação MarkAsJunk: remover um remetente da lista de remetentes bloqueados

O exemplo a seguir de uma solicitação de operação **MarkAsJunk** mostra como remover o remetente de uma mensagem de email da lista de remetentes bloqueados e mover a mensagem de email para a pasta de caixa de entrada. Você precisa manter uma mensagem de email enviada pelo remetente bloqueado para remover o remetente da lista de remetentes bloqueados. Endereço de email do remetente é associado a mensagens de email que foram enviadas pelo remetente. Remover um remetente da lista de remetentes bloqueados não terá êxito se a mensagem de email de referência não existe mais na caixa de correio do usuário. O identificador de item usado para associar uma mensagem de email com seu remetente deve ser associado um item que existe na caixa de correio do Exchange. Recomendamos que você cria uma pasta oculta para armazenar itens enviados por remetentes bloqueados anteriormente, para que os remetentes possam ser desbloqueados do aplicativo cliente. Se um item foi removido da caixa de correio do Exchange, um administrador deve usar o Console de gerenciamento do Exchange para acessar a lista de remetentes bloqueados para remover um remetente da lista. Para obter informações sobre como desbloquear um usuário usando o Console de gerenciamento do Exchange, consulte [como definir as configurações de remetentes bloqueados no Office 365 e de remetentes confiáveis](http://support.microsoft.com/kb/2545137).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
    <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
    </soap:Header>
    <soap:Body>
      <m:MarkAsJunk IsJunk="false" MoveItem="true">
        <m:ItemIds>
          <t:ItemId Id="AAMkAD=" ChangeKey="CQAAABYu" />
        </m:ItemIds>
      </m:MarkAsJunk>
    </soap:Body>
 </soap:Envelope>

```

Uma resposta bem-sucedida para remover um remetente da lista de remetentes bloqueados é o mesmo que a resposta para adicionar um remetente à lista de remetentes bloqueados.
  
A solicitação de corpo SOAP contém os seguintes elementos:
  
- [MarkAsJunk](markasjunk.md)
    
- [ItemIds](itemids.md)
    
- [ItemId](itemid.md)
    
## <a name="markasjunk-operation-error-response"></a>Resposta de erro de operação MarkAsJunk

O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **MarkAsJunk** . Esta é uma resposta a uma solicitação para adicionar ou remover um remetente da lista de remetentes bloqueados quando a mensagem de email especificada pelo identificador de item não existe mais na caixa de correio. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="545" 
                         MinorBuildNumber="11" 
                         Version="Exchange2013" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:MarkAsJunkResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:MarkAsJunkResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:MarkAsJunkResponseMessage>
      </m:ResponseMessages>
    </m:MarkAsJunkResponse>
  </s:Body>
</s:Envelope>
```

A resposta de erro corpo SOAP contém os seguintes elementos:
  
- [MarkAsJunkResponse](markasjunkresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MarkAsJunkResponseMessage](markasjunkresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>Confira também

- [Operações do EWS no Exchange](ews-operations-in-exchange.md)
    
- [Operação GetItem](getitem-operation.md) Operação GetItem 
    
- [Operação FindItem](finditem-operation.md)
    

