---
title: Adicionar e remover os endereços de email da lista de remetentes bloqueados usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: b88288ee-6af7-45b5-a55c-5929cd0c16f1
description: Descubra como usar a API gerenciada de EWS ou o EWS para adicionar endereços de e-mail e removê-los da lista de remetentes bloqueados.
ms.openlocfilehash: c03ed585ebd62802000179d8c837786ba5f9aab4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750667"
---
# <a name="add-and-remove-email-addresses-from-the-blocked-senders-list-by-using-ews-in-exchange"></a>Adicionar e remover os endereços de email da lista de remetentes bloqueados usando o EWS no Exchange

Descubra como usar a API gerenciada de EWS ou o EWS para adicionar endereços de e-mail e removê-los da lista de remetentes bloqueados.
  
A lista de remetentes bloqueados nas opções de lixo eletrônico do usuário fornece uma maneira de mover todos os emails de remetentes especificados para a pasta Lixo eletrônico. É possível habilitar o EWS Managed API ou o aplicativo de EWS adicionar endereços de e-mail ou removê-los da lista de remetentes bloqueados.
  
Observe que uma mensagem a partir do endereço de email deve existir na caixa de correio do usuário antes de adicionar o endereço de email para ou removê-lo da lista de remetentes bloqueados. O método [ExchangeService.MarkAsJunk](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx) EWS Managed API e a operação de EWS [MarkAsJunk](http://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) usam um conjunto de IDs de item. O item IDs na coleção indicam mensagens na caixa de correio para o qual o status de lixo eletrônico deve ser alterado. 
  
Você pode usar os cmdlets [Get-MailboxJunkEmailConfiguration](http://technet.microsoft.com/en-us/library/dd979784%28v=exchg.150%29.aspx) e o Shell de gerenciamento do Exchange [Set-MailboxJunkEmailConfiguration](http://technet.microsoft.com/en-us/library/dd979780%28v=exchg.150%29.aspx) para acessar a lista de remetentes bloqueados diretamente. 
  
## <a name="add-an-email-address-to-or-remove-it-from-the-blocked-senders-list-by-using-the-ews-managed-api"></a>Adicionar um endereço de email para ou removê-lo da lista de remetentes bloqueados usando a API gerenciada de EWS
<a name="bk_AddRemoveEWSMA"> </a>

Para adicionar o remetente de uma mensagem de email à lista de remetentes bloqueados, use o método **MarkAsJunk** e defina o parâmetro **isJunk** como **true**. Para remover o remetente de uma mensagem de email da lista de remetentes bloqueados, defina o parâmetro **isJunk** como **false**.
  
O exemplo a seguir mostra como usar o método **MarkAsJunk** para alterar o status de lixo eletrônico de uma mensagem. 
  
```cs
private static void MarkMessageAsJunk(ExchangeService service, ItemId messageId, bool isJunk, bool moveItem)
{
    List<ItemId> junkItemIds = new List<ItemId>();
    junkItemIds.Add(messageId);
    ServiceResponseCollection<MarkAsJunkResponse> responseCollection = null;
    try
    {
        // If isJunk is true, the sender of the email message is added to 
        // the Blocked Senders List. If isJunk is false, the sender is removed
        // from the list (if present).
        responseCollection = service.MarkAsJunk(junkItemIds, isJunk, moveItem);
    }
    catch (ServiceResponseException ex)
    {
        Console.WriteLine("Error marking item as junk: {0}", ex.ErrorCode);
        return;
    }
    foreach (MarkAsJunkResponse response in responseCollection)
    {
        if (response.Result == ServiceResult.Success)
        {
            Console.WriteLine("Successfully marked message as {0}junk.", isJunk ? "": "NOT ");
            if (moveItem)
            {
                Console.WriteLine("New item ID: {0}", response.MovedItemId.ToString());
            }
        }
        else
        {
            Console.WriteLine("[{0}]: {1}", response.Result.ToString(),
                response.ErrorCode.ToString());
        }
    }
}
```

## <a name="add-an-email-address-to-or-remove-it-from-the-blocked-senders-list-by-using-ews"></a>Adicionar um endereço de email para ou removê-lo da lista de remetentes bloqueados usando o EWS
<a name="bk_AddRemoveEWS"> </a>

A solicitação de EWS SOAP a seguir marca um item como lixo eletrônico, definindo o atributo **IsJunk** no elemento [MarkAsJunk](http://msdn.microsoft.com/library/f06bafc6-7ee3-4b2b-9fd1-7c51328f4729%28Office.15%29.aspx) como **true**. Ele também move a mensagem para a pasta Lixo eletrônico, definindo o atributo **MoveItem** no elemento **MarkAsJunk** como **true**.
  
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
        <t:ItemId Id="AAMkADg1OWUwODcyLTg4M2MtNDAyMS05YjI0LTI5ZGM5OTU4Njk3YwBGAAAAAADPriAxh444TpHj2GoQxWQNBwAN+VjmVZl5Rq1ymCq5eFKOAAAAAAENAAAN+VjmVZl5Rq1ymCq5eFKOAAAAAAEuAAA=" 
            ChangeKey="CQAAABYAAAAN+VjmVZl5Rq1ymCq5eFKOAAAAAADi" />
      </m:ItemIds>
    </m:MarkAsJunk>
  </soap:Body>
</soap:Envelope>
```

A seguinte resposta SOAP EWS mostra a resposta bem-sucedida. O elemento [MovedItemId](http://msdn.microsoft.com/library/7d5425ab-1e75-43d1-b801-802ff5139df6%28Office.15%29.aspx) na resposta contém a ID de item para o item depois que ele foi movido. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:MarkAsJunkResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:MarkAsJunkResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:MovedItemId Id="AAMkADg1OWUwODcyLTg4M2MtNDAyMS05YjI0LTI5ZGM5OTU4Njk3YwBGAAAAAADPriAxh444TpHj2GoQxWQNBwAN+VjmVZl5Rq1ymCq5eFKOAAAAAAEbAAAN+VjmVZl5Rq1ymCq5eFKOAAAE59DIAAA="
              ChangeKey="CQAAABYAAAAN+VjmVZl5Rq1ymCq5eFKOAAAE59E+" />
        </m:MarkAsJunkResponseMessage>
      </m:ResponseMessages>
    </m:MarkAsJunkResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a>Confira também

- [Gerenciamento de caixa de entrada e EWS no Exchange](inbox-management-and-ews-in-exchange.md)   
- [ExchangeService.MarkAsJunk](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx)   
- [Operação MarkAsJunk](http://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx)   
- [Get-MailboxJunkEmailConfiguration](http://technet.microsoft.com/en-us/library/dd979784%28v=exchg.150%29.aspx)   
- [Set-MailboxJunkEmailConfiguration](http://technet.microsoft.com/en-us/library/dd979780%28v=exchg.150%29.aspx) 
- [Shell de Gerenciamento do Exchange](../management/exchange-management-shell.md)
    

