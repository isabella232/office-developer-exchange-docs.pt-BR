---
title: Criar grupos de contatos usando o EWS em Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: acec6e73-c016-419d-be1a-8ec5d993addb
description: Saiba como criar um grupo de contatos usando a API Gerenciada do EWS ou o EWS Exchange.
ms.openlocfilehash: ade7fa68b00b055268cd5f0c34a75e0abbdb18ee
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513217"
---
# <a name="create-contact-groups-by-using-ews-in-exchange"></a>Criar grupos de contatos usando o EWS em Exchange

Saiba como criar um grupo de contatos usando a API Gerenciada do EWS ou o EWS Exchange.
  
Você pode criar um grupo de contatos, que é um grupo de distribuição [privado,](distribution-groups-and-ews-in-exchange.md)usando a API Gerenciada do EWS ou o EWS. Para criar grupos de contatos, use os métodos na classe API Gerenciada do [ContactGroup](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) EWS ou use a [operação CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS. 
  
Observe que você não pode usar a API Gerenciada do EWS ou o EWS para criar um grupo de distribuição universal ou um grupo de segurança. Para criar um grupo de distribuição universal ou grupo de segurança, você pode usar o[cmdlet](https://msdn.microsoft.com/library/ff326159%28v=exchg.140%29.aspx) [New-DistributionGroup](https://technet.microsoft.com/library/aa998856%28v=exchg.150%29.aspx)Exchange Management Shell . 
  
## <a name="create-a-contact-group-by-using-the-ews-managed-api"></a>Criar um grupo de contatos usando a API Gerenciada do EWS
<a name="bk_EWSMA"> </a>

Para criar um grupo de contatos, você só precisa de algumas informações: um nome para o grupo e os membros a adicionar ao grupo. O exemplo a seguir mostra como criar um grupo de contatos simples que contém alguns membros do grupo.
  
```cs
// Create a new contact group object.
ContactGroup myContactGroup = new ContactGroup(service);
// Give the group a name.
myContactGroup.DisplayName = "My Contact Group";
// Add some members to the group.
myContactGroup.Members.Add(new GroupMember("sadie@contoso.com"));
myContactGroup.Members.Add(new GroupMember("alfred@contoso.com"));
// Save the group.
myContactGroup.Save();

```

## <a name="create-a-contact-group-by-using-ews"></a>Criar um grupo de contatos usando o EWS
<a name="bk_EWSMA"> </a>

Pode levar mais algumas linhas de código, mas você pode criar um grupo de contatos usando a [operação CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS. O exemplo de solicitação XML a seguir mostra como você pode criar um grupo de contatos. Essa também é a solicitação XML que é enviada quando você usa a API Gerenciada [do EWS para criar um grupo de contatos.](#bk_EWSMA)
  
```XML
<?xml version="1.0" encoding="utf-8"?>
   <CreateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
MessageDisposition="SaveOnly">
      <Items xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
         <DistributionList xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
            <DisplayName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               My Contact Group
            </DisplayName>
            <Members xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <Member xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                  <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                     <EmailAddress xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                        sadie@contoso.com
                     </EmailAddress>
                  </Mailbox>
               </Member>
               <Member xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                  <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                     <EmailAddress xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                        alfred@contoso.com
                     </EmailAddress>
                  </Mailbox>
               </Member>
            </Members>
         </DistributionList>
      </Items>
   </CreateItem>
```

A seguir, um exemplo de uma resposta XML bem-sucedida à solicitação. Observe que os valores retornados incluem uma ID de item para o novo grupo de contatos e uma chave de alteração que você pode usar em outro código para modificar o grupo de contatos ou expandir o grupo para ver os membros. A ID do item é reduzida para capacidade de leitura.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
   <CreateItemResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessages xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <CreateItemResponseMessage ResponseClass="Success" 
             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
            <ResponseCode xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
               NoError
            </ResponseCode>
            <Items xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
               <DistributionList xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                  <ItemId xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                          Id="AAMkADBlY…" 
                          ChangeKey="EgAAABYAAAAD7hO1SJPWTbICFWZ4U3NMAABXzQiK" />
               </DistributionList>
            </Items>
         </CreateItemResponseMessage>
      </ResponseMessages>
   </CreateItemResponse>
```

## <a name="see-also"></a>Confira também


- [Grupos de distribuição e EWS no Exchange](distribution-groups-and-ews-in-exchange.md)
    
- [Expandir grupos de distribuição usando o EWS no Exchange 2013](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    

