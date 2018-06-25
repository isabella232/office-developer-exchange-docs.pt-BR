---
title: Mover e copiar mensagens de email usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 4771668f-5623-4397-a5c0-b75a7ba01698
description: Aprenda a mover e copiar mensagens de email usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: 16f0604a16785c34dd04bdabedeedd331668a479
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750792"
---
# <a name="move-and-copy-email-messages-by-using-ews-in-exchange"></a>Mover e copiar mensagens de email usando o EWS no Exchange

Aprenda a mover e copiar mensagens de email usando a API gerenciada de EWS ou EWS no Exchange.
  
Você pode usar a API gerenciada de EWS ou EWS mover e copiar mensagens de email em uma caixa de correio.
  
**Tabela 1. Métodos de API gerenciada de EWS e operações de EWS para mover e copiar mensagens de email**

|**Task**|**Método API gerenciada de EWS**|**Operação do EWS**|
|:-----|:-----|:-----|
|Mover uma mensagem de email  <br/> |[EmailMessage.Move](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) <br/> |[MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> |
|Copiar uma mensagem de email  <br/> |[EmailMessage.Copy](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) <br/> |[CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |
   
É importante observar que, quando você move ou copia uma mensagem de email em uma pasta diferente, um novo item for criado na nova pasta com uma ID exclusiva de item, e a mensagem original é excluída. Se você estiver movendo ou copiando uma mensagem de email entre as duas pastas na mesma caixa de correio, o novo item será retornado na resposta, que fornece acesso a ID do item novo. No entanto, se você estiver movendo ou copiando uma mensagem de email entre duas caixas de correio ou entre uma caixa de correio e uma pasta pública, o novo item não será retornado na resposta. Para acessar a mensagem movida nesse cenário, use o método de API gerenciada de EWS [FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) ou a operação de EWS [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) , [criar uma definição de propriedade estendida](properties-and-extended-properties-in-ews-in-exchange.md) para a propriedade [PidTagSearchKey](http://msdn.microsoft.com/en-us/library/cc839918.aspx) (0x300B0102), ou como criar e configurar um sinalizador estendido propriedade e, em seguida, procure a propriedade estendida personalizada na nova pasta. 
  
Excluir uma mensagem de email é diferente de mover um item para a pasta Itens excluídos. Se você usar o método de API gerenciada de EWS [item](http://msdn.microsoft.com/en-us/library/office/dd635072%28v=exchg.80%29.aspx) ou a operação de EWS [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) , o item especificado na solicitação é removido da pasta original e uma cópia é colocada na pasta Itens excluídos com uma nova ID de item. Ao contrário de quando você move ou copia qualquer item, o novo item não será retornado o método **Delete** ou a resposta de operação **DeleteItem** . As etapas envolvidas na [exclusão de um email usando a API gerenciada de EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) ou [EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) são os mesmos para excluir qualquer item genérica do armazenamento do Exchange. 
  
## <a name="move-an-email-message-by-using-the-ews-managed-api"></a>Mover uma mensagem de email usando a API gerenciada de EWS
<a name="bk_moveewsma"> </a>

O exemplo de código a seguir mostra como usar o método [EmailMessage.Move](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) para mover uma mensagem de email existentes de uma pasta para outro. 
  
Este exemplo pressupõe que o **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , e esse **ItemId** é a [Id](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) da mensagem de email para mover ou copiar. 
  
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

O exemplo de código a seguir mostra como usar a operação [MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) para mover uma mensagem de email para a pasta Lixo eletrônico. 
  
Isso também é a solicitação XML que é enviada pelo EWS Managed API ao chamar o método [Move](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) . Os valores de alguns atributos e elementos foram diminuídos para melhorar a legibilidade. 
  
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

O servidor responde à solicitação **MoveItem** com uma mensagem de [MoveItemResponse](http://msdn.microsoft.com/library/77be5104-1e09-4d50-abec-4fadb3a230e5%28Office.15%29.aspx) que inclui um valor de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica que a mensagem de email foi movida com êxito. A resposta também inclui o **ItemId** da mensagem de email na nova pasta, que é importante para armazenar porque o **ItemId** é diferente na nova pasta. 
  
## <a name="copy-an-email-message-by-using-the-ews-managed-api"></a>Copiar uma mensagem de email usando a API gerenciada de EWS
<a name="bk_copyewsma"> </a>

O exemplo de código a seguir mostra como usar o método [EmailMessage.Copy](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) para copiar uma mensagem de email existentes de uma pasta para outro. 
  
Este exemplo pressupõe que o **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , e esse **ItemId** é a [Id](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) da mensagem de email para copiar. Os valores de alguns parâmetros foram diminuídos para melhorar a legibilidade. 
  
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

## <a name="copy-an-email-message-by-using-ews"></a>Copiar uma mensagem de email usando o EWS
<a name="bk_copyews"> </a>

O exemplo de código a seguir mostra como usar a operação [CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) para copiar uma mensagem de email para uma pasta diferente na caixa de correio mesma enviando o [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) da mensagem de email para mover e especificando a pasta de destino no [ToFolderId ](http://msdn.microsoft.com/library/bd6a4265-ad40-43f6-bcc4-0bf5df4e984c%28Office.15%29.aspx)elemento. 
  
Isso também é a solicitação XML que é enviada pelo EWS Managed API ao chamar o método [Copy](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) . Os valores de alguns atributos e elementos foram diminuídos para melhorar a legibilidade. 
  
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

O servidor responde à solicitação **CopyItem** com uma mensagem de [CopyItemResponse](http://msdn.microsoft.com/library/ae402bc1-4589-45e0-a929-f368c916a7e4%28Office.15%29.aspx) que inclui um valor de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica que a mensagem de email foi copiada com êxito. A resposta também inclui o **ItemId** da mensagem de email na nova pasta, que é importante para armazenar porque o **ItemId** é diferente na nova pasta. 
  
## <a name="see-also"></a>Confira também


- [Email e EWS no Exchange](email-and-ews-in-exchange.md)
    
- [Enviar mensagens de email usando o EWS no Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md)
    

