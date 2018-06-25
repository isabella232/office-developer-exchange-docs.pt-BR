---
title: Criar grupos de contatos usando o EWS no Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: acec6e73-c016-419d-be1a-8ec5d993addb
description: Saiba como criar um grupo de contatos, usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: b3357f24e07a9c1b3b37ccb63b0f4f0d0a1d6fcf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750702"
---
# <a name="create-contact-groups-by-using-ews-in-exchange"></a>Criar grupos de contatos usando o EWS no Exchange

Saiba como criar um grupo de contatos, usando a API gerenciada de EWS ou EWS no Exchange.
  
Você pode criar um grupo de contatos, que é um [grupo de distribuição](distribution-groups-and-ews-in-exchange.md)privada, usando a API gerenciada de EWS ou EWS. Para criar grupos de contatos, use os métodos da classe de API gerenciada de EWS [ContactGroup](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) ou use a operação de EWS [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) . 
  
Observe que você não pode usar a API gerenciada de EWS ou o EWS para criar um grupo de distribuição universal ou grupo de segurança. Para criar um grupo de distribuição universal ou grupo de segurança, você pode usar o [New-DistributionGroup](http://technet.microsoft.com/en-us/library/aa998856%28v=exchg.150%29.aspx)[cmdlet do Shell de gerenciamento do Exchange](http://msdn.microsoft.com/en-us/library/ff326159%28v=exchg.140%29.aspx). 
  
## <a name="create-a-contact-group-by-using-the-ews-managed-api"></a>Criar um grupo de contatos usando a API gerenciada de EWS
<a name="bk_EWSMA"> </a>

Para criar um grupo de contatos, você precisa apenas algumas partes de informações: um nome para o grupo e os membros para adicionar ao grupo. O exemplo a seguir mostra como criar um grupo de contatos simple que contém dois membros do grupo.
  
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

Ela pode levar alguns mais linhas de código, mas você pode criar um grupo de contatos usando a operação de EWS [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) . O exemplo de solicitação XML a seguir mostra como você pode criar um grupo de contatos. Isso também é a solicitação XML que será enviada quando você [usar a API gerenciada de EWS para criar um grupo de contatos](#bk_EWSMA).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
   <CreateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
MessageDisposition="SaveOnly">
      <Items xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
         <DistributionList xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
            <DisplayName xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               My Contact Group
            </DisplayName>
            <Members xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <Member xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                  <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                     <EmailAddress xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                        sadie@contoso.com
                     </EmailAddress>
                  </Mailbox>
               </Member>
               <Member xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                  <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                     <EmailAddress xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                        alfred@contoso.com
                     </EmailAddress>
                  </Mailbox>
               </Member>
            </Members>
         </DistributionList>
      </Items>
   </CreateItem>
```

O exemplo a seguir é um exemplo de uma resposta XML bem-sucedida à solicitação. Observe que os valores retornados incluem uma ID de item para o novo grupo de contatos e uma chave de alteração que você pode usar em outro código para modificar o grupo de contatos ou expandir o grupo para ver os membros. A ID do item é abreviada para fins de legibilidade.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
   <CreateItemResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessages xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <CreateItemResponseMessage ResponseClass="Success" 
             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
            <ResponseCode xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
               NoError
            </ResponseCode>
            <Items xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
               <DistributionList xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
                  <ItemId xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
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
    
- [Expandir grupos de distribuição, usando o EWS no Exchange 2013](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    

