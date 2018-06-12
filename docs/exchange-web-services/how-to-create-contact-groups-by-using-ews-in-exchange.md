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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750702"
---
# <a name="create-contact-groups-by-using-ews-in-exchange"></a><span data-ttu-id="03886-103">Criar grupos de contatos usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="03886-103">Create contact groups by using EWS in Exchange</span></span>

<span data-ttu-id="03886-104">Saiba como criar um grupo de contatos, usando a API gerenciada de EWS ou EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="03886-104">Learn how to create a contact group by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="03886-105">Você pode criar um grupo de contatos, que é um [grupo de distribuição](distribution-groups-and-ews-in-exchange.md)privada, usando a API gerenciada de EWS ou EWS.</span><span class="sxs-lookup"><span data-stu-id="03886-105">You can create a contact group, which is a private [distribution group](distribution-groups-and-ews-in-exchange.md), by using the EWS Managed API or EWS.</span></span> <span data-ttu-id="03886-106">Para criar grupos de contatos, use os métodos da classe de API gerenciada de EWS [ContactGroup](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) ou use a operação de EWS [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="03886-106">To create contact groups, use the methods in the [ContactGroup](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contactgroup%28v=exchg.80%29.aspx) EWS Managed API class, or use the [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation.</span></span> 
  
<span data-ttu-id="03886-107">Observe que você não pode usar a API gerenciada de EWS ou o EWS para criar um grupo de distribuição universal ou grupo de segurança.</span><span class="sxs-lookup"><span data-stu-id="03886-107">Note that you can't use the EWS Managed API or EWS to create a universal distribution group or security group.</span></span> <span data-ttu-id="03886-108">Para criar um grupo de distribuição universal ou grupo de segurança, você pode usar o [New-DistributionGroup](http://technet.microsoft.com/en-us/library/aa998856%28v=exchg.150%29.aspx)[cmdlet do Shell de gerenciamento do Exchange](http://msdn.microsoft.com/en-us/library/ff326159%28v=exchg.140%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="03886-108">To create a universal distribution group or security group, you can use the [New-DistributionGroup](http://technet.microsoft.com/en-us/library/aa998856%28v=exchg.150%29.aspx)[Exchange Management Shell cmdlet](http://msdn.microsoft.com/en-us/library/ff326159%28v=exchg.140%29.aspx).</span></span> 
  
## <a name="create-a-contact-group-by-using-the-ews-managed-api"></a><span data-ttu-id="03886-109">Criar um grupo de contatos usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="03886-109">Create a contact group by using the EWS Managed API</span></span>
<span data-ttu-id="03886-110"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="03886-110"></span></span>

<span data-ttu-id="03886-111">Para criar um grupo de contatos, você precisa apenas algumas partes de informações: um nome para o grupo e os membros para adicionar ao grupo.</span><span class="sxs-lookup"><span data-stu-id="03886-111">To create a contact group, you just need a couple pieces of information: a name for the group, and the members to add to the group.</span></span> <span data-ttu-id="03886-112">O exemplo a seguir mostra como criar um grupo de contatos simple que contém dois membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="03886-112">The following example shows how to create a simple contact group that contains a couple of group members.</span></span>
  
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

## <a name="create-a-contact-group-by-using-ews"></a><span data-ttu-id="03886-113">Criar um grupo de contatos usando o EWS</span><span class="sxs-lookup"><span data-stu-id="03886-113">Create a contact group by using EWS</span></span>
<span data-ttu-id="03886-114"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="03886-114"></span></span>

<span data-ttu-id="03886-115">Ela pode levar alguns mais linhas de código, mas você pode criar um grupo de contatos usando a operação de EWS [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="03886-115">It might take a few more lines of code, but you can create a contact group by using the [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation.</span></span> <span data-ttu-id="03886-116">O exemplo de solicitação XML a seguir mostra como você pode criar um grupo de contatos.</span><span class="sxs-lookup"><span data-stu-id="03886-116">The following XML request example shows how you can create a contact group.</span></span> <span data-ttu-id="03886-117">Isso também é a solicitação XML que será enviada quando você [usar a API gerenciada de EWS para criar um grupo de contatos](#bk_EWSMA).</span><span class="sxs-lookup"><span data-stu-id="03886-117">This is also the XML request that is sent when you [use the EWS Managed API to create a contact group](#bk_EWSMA).</span></span>
  
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

<span data-ttu-id="03886-118">O exemplo a seguir é um exemplo de uma resposta XML bem-sucedida à solicitação.</span><span class="sxs-lookup"><span data-stu-id="03886-118">The following is an example of a successful XML response to the request.</span></span> <span data-ttu-id="03886-119">Observe que os valores retornados incluem uma ID de item para o novo grupo de contatos e uma chave de alteração que você pode usar em outro código para modificar o grupo de contatos ou expandir o grupo para ver os membros.</span><span class="sxs-lookup"><span data-stu-id="03886-119">Notice that the values returned include an item ID for the new contact group and a change key that you can use in other code to modify the contact group or expand the group to see the members.</span></span> <span data-ttu-id="03886-120">A ID do item é abreviada para fins de legibilidade.</span><span class="sxs-lookup"><span data-stu-id="03886-120">The item ID is shortened for readability.</span></span>
  
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

## <a name="see-also"></a><span data-ttu-id="03886-121">Confira também</span><span class="sxs-lookup"><span data-stu-id="03886-121">See also</span></span>


- [<span data-ttu-id="03886-122">Grupos de distribuição e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="03886-122">Distribution groups and EWS in Exchange</span></span>](distribution-groups-and-ews-in-exchange.md)
    
- [<span data-ttu-id="03886-123">Expandir grupos de distribuição, usando o EWS no Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="03886-123">Expand distribution groups by using EWS in Exchange 2013</span></span>](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    

