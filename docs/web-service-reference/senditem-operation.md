---
title: Operação SendItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SendItem
api_type:
- schema
ms.assetid: 337b89ef-e1b7-45ed-92f3-8abe4200e4c7
description: A operação SendItem é usada para enviar mensagens de email localizadas no Exchange store.
ms.openlocfilehash: d1e43cdceb3a594c3fa2f028502a3bfedbbf85a1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521582"
---
# <a name="senditem-operation"></a>Operação SendItem

A operação SendItem é usada para enviar mensagens de email localizadas no Exchange store.
  
## <a name="senditem-e-mail-message-request-example"></a>Exemplo de solicitação SendItem (Email Message)

### <a name="description"></a>Descrição

O exemplo a seguir mostra como enviar uma mensagem de email.
  
### <a name="code"></a>Código

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SendItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
              SaveItemToFolder="true">
      <ItemIds>
        <t:ItemId Id="AAAtAEF=" ChangeKey="CQAAABY+T" />
      </ItemIds>
    </SendItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comentários

O identificador de item foi reduzido para preservar a capacidade de leitura.
  
### <a name="request-elements"></a>Elementos request

Os seguintes elementos são usados na solicitação:
  
- [SendItem](senditem.md)
    
- [ItemIds](itemids.md)
    
- [ItemId](itemid.md)
    
## <a name="successful-senditem-e-mail-message-response"></a>Resposta bem-sucedida de SendItem (Mensagem de Email)

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta SendItem bem-sucedida.
  
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
    <SendItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SendItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:SendItemResponseMessage>
      </m:ResponseMessages>
    </SendItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a>Elementos de resposta bem-sucedidos

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [SendItemResponse](senditemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [SendItemResponseMessage](senditemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
### <a name="comments"></a>Comentários

Um representante que tenta enviar uma mensagem de email localizada na pasta Rascunhos da entidade principal com a opção SendAndSaveCopy definida para salvar uma cópia na pasta de destaque Itens Enviados falhará silenciosamente ao mover uma cópia do item enviado para a pasta distinta Itens Enviados. O item permanecerá na pasta Rascunhos da entidade. A solução alternativa para esse problema é especificar a caixa de correio da entidade no [elemento DistinguishedFolderId.](distinguishedfolderid.md) 
  
Um cenário adicional a ser considerado é quando um representante cria uma mensagem de email e salva-a na pasta Rascunhos da caixa de correio do representante. Se o representante tentar enviar o item e salvar uma cópia para a pasta distinta Itens Enviados da entidade principal, a mensagem será enviada corretamente, a mensagem de rascunho permanecerá na pasta Rascunhos do representante, a mensagem enviada não aparecerá na pasta Itens Enviados do representante ou da entidade principal e a resposta será um sucesso.
  
## <a name="invalid-senditem-e-mail-message-request-example"></a>Exemplo de solicitação SendItem inválido (Mensagem de Email)

### <a name="description"></a>Descrição

O exemplo de código a seguir mostra um exemplo de uma solicitação com um identificador inválido.
  
### <a name="code"></a>Código

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SendItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
              SaveItemToFolder="true">
      <ItemIds>
        <t:ItemId Id="%BadItemId%" ChangeKey="CQAAABYAAA" />
      </ItemIds>
    </SendItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="senditem-e-mail-message-error-response"></a>Resposta de erro SendItem (Email Message)

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta de erro a uma solicitação SendItem que contém um identificador inválido.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SendItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SendItemResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:SendItemResponseMessage>
      </m:ResponseMessages>
    </SendItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Elementos de resposta de erro

Os seguintes elementos são usados na resposta de erro:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [SendItemResponse](senditemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [SendItemResponseMessage](senditemresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>Confira também



[Operação SendItem](senditem-operation.md)
  
 **SendItemType**


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

