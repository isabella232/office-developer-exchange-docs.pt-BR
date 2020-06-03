---
title: Mover e copiar mensagens de email usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 4771668f-5623-4397-a5c0-b75a7ba01698
description: Saiba como mover e copiar mensagens de email usando a API gerenciada do EWS ou o EWS no Exchange.
localization_priority: Priority
ms.openlocfilehash: d13e84648f194dd4f431cf128396daf016addb22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527933"
---
# <a name="move-and-copy-email-messages-by-using-ews-in-exchange"></a>Mover e copiar mensagens de email usando o EWS no Exchange

Saiba como mover e copiar mensagens de email usando a API gerenciada do EWS ou o EWS no Exchange.
  
Você pode usar a API gerenciada do EWS ou o EWS para mover e copiar mensagens de email em uma caixa de correio.
  
**Tabela 1. Métodos da API gerenciada do EWS e operações do EWS para mover e copiar mensagens de email**

|**Tarefa**|**Método de API gerenciada do EWS**|**Operação do EWS**|
|:-----|:-----|:-----|
|Mover uma mensagem de email  <br/> |[EmailMessage. move](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) <br/> |[MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> |
|Copiar uma mensagem de email  <br/> |[EmailMessage. Copy](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) <br/> |[CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |
   
É importante observar que quando você move ou copia uma mensagem de email em uma pasta diferente, um novo item é criado na nova pasta com uma ID de item exclusivo e a mensagem original é excluída. Se você estiver movendo ou copiando uma mensagem de email entre duas pastas na mesma caixa de correio, o novo item será retornado na resposta, o que fornece acesso à nova ID de item. No entanto, se você estiver movendo ou copiando uma mensagem de email entre duas caixas de correio ou entre uma caixa de correio e uma pasta pública, o novo item não será retornado na resposta. Para acessar a mensagem movida nesse cenário, use o método [FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) da API gerenciada do EWS ou a operação do EWS [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) , [crie uma definição de propriedade estendida](properties-and-extended-properties-in-ews-in-exchange.md) para a propriedade [PidTagSearchKey](https://msdn.microsoft.com/library/cc839918.aspx) (0x300B0102), ou crie e defina uma propriedade estendida personalizada e, em seguida, procure a propriedade estendida personalizada na nova pasta. 
  
Excluir uma mensagem de email é diferente de mover um item para a pasta itens excluídos. Se você usar o item da API gerenciada do EWS [. Delete](https://msdn.microsoft.com/library/office/dd635072%28v=exchg.80%29.aspx) ou a operação do EWS [DeleteItem](../web-service-reference/deleteitem-operation.md) , o item especificado na solicitação será removido da pasta original e uma cópia será colocada na pasta itens excluídos com uma nova ID de item. Diferentemente de quando você move ou copia qualquer item, o novo item não é retornado no método **delete** ou a resposta da operação **DeleteItem** . As etapas envolvidas na [exclusão de um email usando a API gerenciada do EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) ou [EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) são as mesmas que as para excluir qualquer item genérico do repositório do Exchange. 
  
## <a name="move-an-email-message-by-using-the-ews-managed-api"></a>Mover uma mensagem de email usando a API gerenciada do EWS
<a name="bk_moveewsma"> </a>

O exemplo de código a seguir mostra como usar o método [EmailMessage. move](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) para mover uma mensagem de email existente de uma pasta para outra. 
  
Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que **ItemId** é a [ID](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) da mensagem de email a ser movida ou copiada. 
  
```cs
// As a best practice, limit the properties returned by the Bind method to only those that are required.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, EmailMessageSchema.Subject, EmailMessageSchema.ParentFolderId);
// Bind to the existing item by using the ItemId.
// This method call results in a GetItem call to EWS.
EmailMessage beforeMessage = EmailMessage.Bind(service, ItemId, propSet);
// Move the specified mail to the JunkEmail folder and store the returned item.
Item item = beforeMessage.Move(WellKnownFolderName.JunkEmail);
// Check that the item was moved by binding to the moved email message 
// and retrieving the new ParentFolderId.
// This method call results in a GetItem call to EWS.
EmailMessage movedMessage = EmailMessage.Bind(service, item.Id, propSet);
Console.WriteLine("An email message with the subject '" + beforeMessage.Subject + "' has been moved from the '" + beforeMessage.ParentFolderId + "' folder to the '" + movedMessage.ParentFolderId + "' folder.");
```

## <a name="move-an-email-message-by-using-ews"></a>Mover uma mensagem de email usando o EWS
<a name="bk_moveews"> </a>

O exemplo de código a seguir mostra como usar a operação [MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) para mover uma mensagem de email para a pasta lixo eletrônico. 
  
Essa é também a solicitação XML que é enviada pela API gerenciada do EWS ao chamar o método [move](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) . Os valores de alguns atributos e elementos foram reduzidos para facilitar a leitura. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:MoveItem>
      <m:ToFolderId>
        <t:DistinguishedFolderId Id="junkemail" />
      </m:ToFolderId>
      <m:ItemIds>
        <t:ItemId Id="AfwDoAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF25sM1" />
      </m:ItemIds>
    </m:MoveItem>
  </soap:Body>
</soap:Envelope>
```

O servidor responde à solicitação **MoveItem** com uma mensagem [MoveItemResponse](https://msdn.microsoft.com/library/77be5104-1e09-4d50-abec-4fadb3a230e5%28Office.15%29.aspx) que inclui um valor de [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica que a mensagem de email foi movida com êxito. A resposta também inclui o **ItemId** para a mensagem de email na nova pasta, o que é importante armazenar porque **ItemId** é diferente na nova pasta. 
  
## <a name="copy-an-email-message-by-using-the-ews-managed-api"></a>Copiar uma mensagem de email usando a API gerenciada do EWS
<a name="bk_copyewsma"> </a>

O exemplo de código a seguir mostra como usar o método [EmailMessage. Copy](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) para copiar uma mensagem de email existente de uma pasta para outra. 
  
Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que **ItemId** é a [ID](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) da mensagem de email a ser copiada. Os valores de alguns parâmetros foram reduzidos para legibilidade. 
  
```cs
// As a best practice, limit the properties returned by the Bind method to only those that are required.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, EmailMessageSchema.Subject, EmailMessageSchema.ParentFolderId);
// Bind to the existing item by using the ItemId.
// This method call results in a GetItem call to EWS.
EmailMessage originalMessage = EmailMessage.Bind(service, ItemId, propSet);
// Copy the orignal message into another folder in the mailbox and store the returned item.
Item item = originalMessage.Copy("epQ/3AAA=");
// Check that the item was copied by binding to the copied email message 
// and retrieving the new ParentFolderId.
// This method call results in a GetItem call to EWS.
EmailMessage copiedMessage = EmailMessage.Bind(service, item.Id, propSet);
Console.WriteLine("An email message with the subject '" + originalMessage.Subject + "' has been copied from the '" + originalMessage.ParentFolderId + "' folder to the '" + copiedMessage.ParentFolderId + "' folder.");
```

## <a name="copy-an-email-message-by-using-ews"></a>Copiar uma mensagem de email usando EWS
<a name="bk_copyews"> </a>

O exemplo de código a seguir mostra como usar a operação [CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) para copiar uma mensagem de email para uma pasta diferente na mesma caixa de correio enviando o [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) da mensagem de email a ser movida e especificando a pasta de destino no elemento [ToFolderId](https://msdn.microsoft.com/library/bd6a4265-ad40-43f6-bcc4-0bf5df4e984c%28Office.15%29.aspx) . 
  
Essa é também a solicitação XML que é enviada pela API gerenciada do EWS ao chamar o método [Copy](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) . Os valores de alguns atributos e elementos foram reduzidos para facilitar a leitura. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:CopyItem>
      <m:ToFolderId>
        <t:FolderId Id="pQ/3AAA=" />
      </m:ToFolderId>
      <m:ItemIds>
        <t:ItemId Id="2TSeSAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF2d+3+" />
      </m:ItemIds>
    </m:CopyItem>
  </soap:Body>
</soap:Envelope>
```

O servidor responde à solicitação **CopyItem** com uma mensagem [CopyItemResponse](https://msdn.microsoft.com/library/ae402bc1-4589-45e0-a929-f368c916a7e4%28Office.15%29.aspx) que inclui um valor de [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica que a mensagem de email foi copiada com êxito. A resposta também inclui o **ItemId** para a mensagem de email na nova pasta, o que é importante armazenar porque **ItemId** é diferente na nova pasta. 
  
## <a name="see-also"></a>Confira também


- [Email e EWS no Exchange](email-and-ews-in-exchange.md)
    
- [Enviar mensagens de email usando o EWS no Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md)
    

