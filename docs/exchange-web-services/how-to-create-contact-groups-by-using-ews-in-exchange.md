---
title: Criar grupos de contatos usando o EWS no Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: acec6e73-c016-419d-be1a-8ec5d993addb
description: Saiba como criar um grupo de contatos usando a API gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: 1da876bbda72f5bea08fd9855aa3f554135d54aa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528136"
---
# <a name="create-contact-groups-by-using-ews-in-exchange"></a><span data-ttu-id="7acc4-103">Criar grupos de contatos usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7acc4-103">Create contact groups by using EWS in Exchange</span></span>

<span data-ttu-id="7acc4-104">Saiba como criar um grupo de contatos usando a API gerenciada do EWS ou o EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="7acc4-104">Learn how to create a contact group by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="7acc4-105">Você pode criar um grupo de contatos, que é um [grupo de distribuição](distribution-groups-and-ews-in-exchange.md)privado, usando a API gerenciada do EWS ou o EWS.</span><span class="sxs-lookup"><span data-stu-id="7acc4-105">You can create a contact group, which is a private [distribution group](distribution-groups-and-ews-in-exchange.md), by using the EWS Managed API or EWS.</span></span> <span data-ttu-id="7acc4-106">Para criar grupos de contatos, use os métodos na classe da API gerenciada EWS de grupo de [contatos](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) ou use a operação [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS.</span><span class="sxs-lookup"><span data-stu-id="7acc4-106">To create contact groups, use the methods in the [ContactGroup](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) EWS Managed API class, or use the [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation.</span></span> 
  
<span data-ttu-id="7acc4-107">Observe que você não pode usar a API gerenciada do EWS ou o EWS para criar um grupo de distribuição ou grupo de segurança universal.</span><span class="sxs-lookup"><span data-stu-id="7acc4-107">Note that you can't use the EWS Managed API or EWS to create a universal distribution group or security group.</span></span> <span data-ttu-id="7acc4-108">Para criar um grupo de distribuição ou grupo de segurança universal, você pode usar o[cmdlet do Shell de gerenciamento do Exchange](https://msdn.microsoft.com/library/ff326159%28v=exchg.140%29.aspx) [de nova distribuição](https://technet.microsoft.com/library/aa998856%28v=exchg.150%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="7acc4-108">To create a universal distribution group or security group, you can use the [New-DistributionGroup](https://technet.microsoft.com/library/aa998856%28v=exchg.150%29.aspx)[Exchange Management Shell cmdlet](https://msdn.microsoft.com/library/ff326159%28v=exchg.140%29.aspx).</span></span> 
  
## <a name="create-a-contact-group-by-using-the-ews-managed-api"></a><span data-ttu-id="7acc4-109">Criar um grupo de contatos usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="7acc4-109">Create a contact group by using the EWS Managed API</span></span>
<span data-ttu-id="7acc4-110"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="7acc4-110"><a name="bk_EWSMA"> </a></span></span>

<span data-ttu-id="7acc4-111">Para criar um grupo de contatos, você precisa apenas de algumas informações: um nome para o grupo e os membros a serem adicionados ao grupo.</span><span class="sxs-lookup"><span data-stu-id="7acc4-111">To create a contact group, you just need a couple pieces of information: a name for the group, and the members to add to the group.</span></span> <span data-ttu-id="7acc4-112">O exemplo a seguir mostra como criar um grupo de contatos simples que contenha alguns membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="7acc4-112">The following example shows how to create a simple contact group that contains a couple of group members.</span></span>
  
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

## <a name="create-a-contact-group-by-using-ews"></a><span data-ttu-id="7acc4-113">Criar um grupo de contatos usando o EWS</span><span class="sxs-lookup"><span data-stu-id="7acc4-113">Create a contact group by using EWS</span></span>
<span data-ttu-id="7acc4-114"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="7acc4-114"><a name="bk_EWSMA"> </a></span></span>

<span data-ttu-id="7acc4-115">Pode levar mais algumas linhas de código, mas você pode criar um grupo de contatos usando a operação [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS.</span><span class="sxs-lookup"><span data-stu-id="7acc4-115">It might take a few more lines of code, but you can create a contact group by using the [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation.</span></span> <span data-ttu-id="7acc4-116">O exemplo de solicitação XML a seguir mostra como você pode criar um grupo de contatos.</span><span class="sxs-lookup"><span data-stu-id="7acc4-116">The following XML request example shows how you can create a contact group.</span></span> <span data-ttu-id="7acc4-117">Essa é também a solicitação XML que é enviada quando você [usa a API gerenciada do EWS para criar um grupo de contatos](#bk_EWSMA).</span><span class="sxs-lookup"><span data-stu-id="7acc4-117">This is also the XML request that is sent when you [use the EWS Managed API to create a contact group](#bk_EWSMA).</span></span>
  
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

<span data-ttu-id="7acc4-118">Veja a seguir um exemplo de uma resposta XML bem-sucedida à solicitação.</span><span class="sxs-lookup"><span data-stu-id="7acc4-118">The following is an example of a successful XML response to the request.</span></span> <span data-ttu-id="7acc4-119">Observe que os valores retornados incluem uma ID de item para o novo grupo de contatos e uma chave de alteração que você pode usar em outro código para modificar o grupo de contatos ou expandir o grupo para ver os membros.</span><span class="sxs-lookup"><span data-stu-id="7acc4-119">Notice that the values returned include an item ID for the new contact group and a change key that you can use in other code to modify the contact group or expand the group to see the members.</span></span> <span data-ttu-id="7acc4-120">A ID do item é reduzida para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="7acc4-120">The item ID is shortened for readability.</span></span>
  
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

## <a name="see-also"></a><span data-ttu-id="7acc4-121">Confira também</span><span class="sxs-lookup"><span data-stu-id="7acc4-121">See also</span></span>


- [<span data-ttu-id="7acc4-122">Grupos de distribuição e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7acc4-122">Distribution groups and EWS in Exchange</span></span>](distribution-groups-and-ews-in-exchange.md)
    
- [<span data-ttu-id="7acc4-123">Expandir grupos de distribuição usando EWS no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="7acc4-123">Expand distribution groups by using EWS in Exchange 2013</span></span>](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    

