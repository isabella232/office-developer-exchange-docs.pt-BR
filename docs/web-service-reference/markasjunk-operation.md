---
title: Operação MarkAsJunk
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 1f71f04d-56a9-4fee-a4e7-d1034438329e
description: Encontre informações sobre a operação MarkAsJunk EWS.
ms.openlocfilehash: b165b415ce9380846b49d15dd321bfddba72b749
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524732"
---
# <a name="markasjunk-operation"></a>Operação MarkAsJunk

Encontre informações sobre a **operação MarkAsJunk** EWS. 
  
A **operação MarkAsJunk** adiciona e remove usuários da lista de emails bloqueados e move mensagens de email para a pasta Lixo Eletrônico. 
  
This operation was introduced in Exchange Server 2013.
  
## <a name="using-the-markasjunk-operation"></a>Usando a operação MarkAsJunk

A **operação MarkAsJunk** contém duas opções booleanas para indicar se um remetente de email deve ser adicionado à lista de remetentes bloqueados e se a mensagem de email de destino deve ser movida para a pasta padrão Lixo Eletrônico ou a pasta Caixa de Entrada. As ações são determinadas pelos valores dos atributos **IsJunk** e **MoveItem.** Veja a seguir as ações possíveis com base nas combinações de valores dos atributos **IsJunk** e **MoveItem:** 
  
- Se o atributo **IsJunk** estiver definido como **true** e o atributo **MoveItem** estiver definido como **true**, o remetente da mensagem de email de destino será adicionado à lista de remetentes bloqueados e a mensagem de email será movida para a pasta Lixo Eletrônico do Dmail.
    
- Se o atributo **IsJunk** estiver definido como **true** e o atributo **MoveItem** estiver definido como **false**, o remetente da mensagem de email de destino será adicionado à lista de remetentes bloqueados e a mensagem de email não será movida da pasta.
    
- Se o atributo **IsJunk** for definido como **false** e o atributo **MoveItem** estiver definido como **true**, o remetente da mensagem de email de destino será removido da lista de remetentes bloqueados e a mensagem de email será movida para a pasta Caixa de Entrada.
    
- Se o atributo **IsJunk** for definido como **false** e o atributo **MoveItem** estiver definido como **false**, o remetente da mensagem de email de destino será removido da lista de remetentes bloqueados e a mensagem de email não será movida da pasta.
    
> [!IMPORTANT]
> O conteúdo da lista de remetentes bloqueados não pode ser descoberto pelo EWS. Se um remetente for adicionado à lista de remetentes bloqueados, você precisará manter uma cópia de uma mensagem de email enviada pelo remetente bloqueado para desbloquear o remetente no futuro. 
  
### <a name="markasjunk-operation-soap-headers"></a>Headers SOAP da operação MarkAsJunk

A **operação MarkAsJunk** pode usar os headers SOAP listados na tabela a seguir. 
  
|**Nome de cabeçalho**|**Elemento**|**Descrição**|
|:-----|:-----|:-----|
|**Representação** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifica o usuário que o aplicativo cliente está representando. Esse header é aplicável a uma solicitação.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifica a cultura, conforme definido na RFC 3066, "Marcas para a Identificação de Idiomas", a ser usada para acessar a caixa de correio. Esse header é aplicável a uma solicitação.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifica a versão do esquema para a solicitação de operação. Esse header é aplicável a uma solicitação.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifica a versão do servidor que respondeu à solicitação. Esse header é aplicável a uma resposta.  <br/> |
   
## <a name="markasjunk-operation-request-example-add-a-sender-to-the-blocked-sender-list"></a>Exemplo de solicitação de operação MarkAsJunk: Adicionar um remetente à lista de remetentes bloqueados

O exemplo a seguir de uma solicitação de operação **MarkAsJunk** mostra como adicionar o remetente de um email à lista de remetentes bloqueados e mover o email para a pasta lixo eletrônico. A **operação MarkAsJunk** aceita o identificador de mensagem de email exclusivo para identificar o email usado para fazer referência ao remetente adicionado à lista de remetentes bloqueados. 
  
> [!NOTE]
> Todos os identificadores de item e teclas de alteração neste artigo foram reduzidos para preservar a capacidade de leitura. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
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

O corpo SOAP de solicitação contém os seguintes elementos:
  
- [MarkAsJunk](markasjunk.md)
    
- [ItemIds](itemids.md)
    
- [ItemId](itemid.md)
    
## <a name="successful-markasjunk-operation-response"></a>Resposta bem-sucedida da operação MarkAsJunk

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **MarkAsJunk** para adicionar um remetente à lista de remetentes bloqueados e mover a mensagem de email para a pasta Lixo Eletrônico. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" 
                             MinorVersion="0" 
                             MajorBuildNumber="545" 
                             MinorBuildNumber="11" 
                             Version="Exchange2013" 
                             xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                             xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
            xmlns:xsd="http://www.w3.org/2001/XMLSchema">
        <m:MarkAsJunkResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

O corpo SOAP de resposta contém os seguintes elementos:
  
- [MarkAsJunkResponse](markasjunkresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MarkAsJunkResponseMessage](markasjunkresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [MovedItemId](moveditemid.md)
    
## <a name="markasjunk-operation-request-example-remove-a-sender-from-the-blocked-sender-list"></a>Exemplo de solicitação de operação MarkAsJunk: Remover um remetente da lista de remetentes bloqueados

O exemplo a seguir de uma solicitação de operação **MarkAsJunk** mostra como remover o remetente de uma mensagem de email da lista de remetentes bloqueados e mover a mensagem de email para a pasta Caixa de Entrada. Você precisa manter uma mensagem de email enviada pelo remetente bloqueado para remover o remetente da lista de remetentes bloqueados. O endereço de email do remetente está associado a mensagens de email enviadas pelo remetente. Remover um remetente da lista de remetentes bloqueados não terá êxito se a mensagem de email de referência não existir mais na caixa de correio do usuário. O identificador de item usado para associar uma mensagem de email ao remetente deve estar associado a um item que existe na caixa de correio Exchange. Recomendamos que você crie uma pasta oculta para armazenar itens enviados por enviados anteriormente bloqueados para que os envios possam ser desbloqueados do aplicativo cliente. No caso de um item ter sido removido da caixa de correio Exchange, um administrador deve usar o Console de Gerenciamento do Exchange para acessar a lista de remetentes bloqueados para remover um remetente da lista. Para obter informações sobre como desbloquear um usuário usando o Console de Gerenciamento do Exchange, consulte Como configurar as configurações de envios seguros e de [envios bloqueados em Office 365](https://support.microsoft.com/kb/2545137).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
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

Uma resposta bem-sucedida para remover um remetente da lista de remetentes bloqueados é a mesma que a resposta para adicionar um remetente à lista de remetentes bloqueados.
  
O corpo SOAP de solicitação contém os seguintes elementos:
  
- [MarkAsJunk](markasjunk.md)
    
- [ItemIds](itemids.md)
    
- [ItemId](itemid.md)
    
## <a name="markasjunk-operation-error-response"></a>Resposta de erro da operação MarkAsJunk

O exemplo a seguir mostra uma resposta de erro a **uma solicitação de operação MarkAsJunk.** Esta é uma resposta a uma solicitação para adicionar ou remover um remetente da lista de remetentes bloqueados quando a mensagem de email especificada pelo identificador de item não existir mais na caixa de correio. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="545" 
                         MinorBuildNumber="11" 
                         Version="Exchange2013" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:MarkAsJunkResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

O corpo SOAP da resposta de erro contém os seguintes elementos:
  
- [MarkAsJunkResponse](markasjunkresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MarkAsJunkResponseMessage](markasjunkresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>Confira também

- [Operações EWS em Exchange](ews-operations-in-exchange.md)
    
- [Operação GetItem](getitem-operation.md) Operação GetItem 
    
- [Operação FindItem](finditem-operation.md)
    

