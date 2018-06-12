---
title: Operação DeleteItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItem
api_type:
- schema
ms.assetid: 3e26c416-fa12-476e-bfd2-5c1f4bb7b348
description: A operação DeleteItem exclui os itens no armazenamento do Exchange.
ms.openlocfilehash: 87d7853daa5db0cd87b3f6469c228a584b4d9caf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751753"
---
# <a name="deleteitem-operation"></a><span data-ttu-id="5c2bd-103">Operação DeleteItem</span><span class="sxs-lookup"><span data-stu-id="5c2bd-103">DeleteItem operation</span></span>

<span data-ttu-id="5c2bd-104">A operação **DeleteItem** exclui os itens no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c2bd-104">The **DeleteItem** operation deletes items in the Exchange store.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="5c2bd-105">Uma resposta de erro que inclui o código de erro ErrorCannotDeleteObject será retornada para uma operação **DeleteItem** quando um delegado tenta excluir um item na caixa de correio do principal, definindo o DisposalType para MoveToDeletedItems.</span><span class="sxs-lookup"><span data-stu-id="5c2bd-105">An error response that includes the ErrorCannotDeleteObject error code will be returned for a **DeleteItem** operation when a delegate tries to delete an item in the principal's mailbox by setting the DisposalType to MoveToDeletedItems.</span></span> <span data-ttu-id="5c2bd-106">Para excluir um item, movendo-o para a pasta Itens excluídos, um representante deve usar a [operação MoveItem](moveitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="5c2bd-106">To delete an item by moving it to the Deleted Items folder, a delegate must use the [MoveItem operation](moveitem-operation.md).</span></span> 
  
## <a name="deleteitem-request-example"></a><span data-ttu-id="5c2bd-107">Exemplo de solicitação DeleteItem</span><span class="sxs-lookup"><span data-stu-id="5c2bd-107">DeleteItem request example</span></span>

### <a name="description"></a><span data-ttu-id="5c2bd-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c2bd-108">Description</span></span>

<span data-ttu-id="5c2bd-109">O exemplo a seguir de uma solicitação de **DeleteItem** mostra como realizar uma exclusão dura de um item de uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="5c2bd-109">The following example of a **DeleteItem** request shows how to perform a hard delete of an item from a mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="5c2bd-110">A ID do item foi reduzida para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5c2bd-110">The item ID has been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="5c2bd-111">Código</span><span class="sxs-lookup"><span data-stu-id="5c2bd-111">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <DeleteItem DeleteType="HardDelete" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemIds>
        <t:ItemId Id="AS4AUn=="/>
      </ItemIds>
    </DeleteItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="5c2bd-112">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5c2bd-112">Request elements</span></span>

<span data-ttu-id="5c2bd-113">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="5c2bd-113">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="5c2bd-114">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="5c2bd-114">DeleteItem</span></span>](deleteitem.md)
    
- [<span data-ttu-id="5c2bd-115">ItemIds</span><span class="sxs-lookup"><span data-stu-id="5c2bd-115">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="5c2bd-116">ItemId</span><span class="sxs-lookup"><span data-stu-id="5c2bd-116">ItemId</span></span>](itemid.md)
    
<span data-ttu-id="5c2bd-117">Para localizar outras opções para a mensagem de solicitação da operação **DeleteItem** , explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="5c2bd-117">To find other options for the request message of the **DeleteItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="5c2bd-118">Inicie o elemento [DeleteItem](deleteitem.md) .</span><span class="sxs-lookup"><span data-stu-id="5c2bd-118">Start at the [DeleteItem](deleteitem.md) element.</span></span> 
  
## <a name="successful-deleteitem-response"></a><span data-ttu-id="5c2bd-119">Resposta de DeleteItem bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="5c2bd-119">Successful DeleteItem response</span></span>

### <a name="description"></a><span data-ttu-id="5c2bd-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c2bd-120">Description</span></span>

<span data-ttu-id="5c2bd-121">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação **DeleteItem** .</span><span class="sxs-lookup"><span data-stu-id="5c2bd-121">The following example shows a successful response to the **DeleteItem** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="5c2bd-122">Código</span><span class="sxs-lookup"><span data-stu-id="5c2bd-122">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <DeleteItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteItemResponseMessage>
      </m:ResponseMessages>
    </DeleteItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="5c2bd-123">Elementos de resposta bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="5c2bd-123">Successful response elements</span></span>

<span data-ttu-id="5c2bd-124">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="5c2bd-124">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="5c2bd-125">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5c2bd-125">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="5c2bd-126">DeleteItemResponse</span><span class="sxs-lookup"><span data-stu-id="5c2bd-126">DeleteItemResponse</span></span>](deleteitemresponse.md)
    
- [<span data-ttu-id="5c2bd-127">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5c2bd-127">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5c2bd-128">DeleteItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5c2bd-128">DeleteItemResponseMessage</span></span>](deleteitemresponsemessage.md)
    
- [<span data-ttu-id="5c2bd-129">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5c2bd-129">ResponseCode</span></span>](responsecode.md)
    
<span data-ttu-id="5c2bd-130">Para localizar outras opções para a mensagem de resposta da operação **DeleteItem** , explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="5c2bd-130">To find other options for the response message of the **DeleteItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="5c2bd-131">Inicie o elemento [DeleteItemResponse](deleteitemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="5c2bd-131">Start at the [DeleteItemResponse](deleteitemresponse.md) element.</span></span> 
  
## <a name="deleteitem-error-response"></a><span data-ttu-id="5c2bd-132">Resposta de erro DeleteItem</span><span class="sxs-lookup"><span data-stu-id="5c2bd-132">DeleteItem error response</span></span>

### <a name="description"></a><span data-ttu-id="5c2bd-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c2bd-133">Description</span></span>

<span data-ttu-id="5c2bd-134">O exemplo a seguir mostra uma resposta de erro a uma solicitação de **DeleteItem** .</span><span class="sxs-lookup"><span data-stu-id="5c2bd-134">The following example shows an error response to a **DeleteItem** request.</span></span> <span data-ttu-id="5c2bd-135">O erro foi criado porque a operação tentou excluir um item que não foi encontrado no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c2bd-135">The error was created because the operation tried to delete an item that was not found in the Exchange store.</span></span> 
  
### <a name="code"></a><span data-ttu-id="5c2bd-136">Código</span><span class="sxs-lookup"><span data-stu-id="5c2bd-136">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <DeleteItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteItemResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DeleteItemResponseMessage>
      </m:ResponseMessages>
    </DeleteItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="5c2bd-137">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="5c2bd-137">Error response elements</span></span>

<span data-ttu-id="5c2bd-138">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="5c2bd-138">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="5c2bd-139">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5c2bd-139">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="5c2bd-140">DeleteItemResponse</span><span class="sxs-lookup"><span data-stu-id="5c2bd-140">DeleteItemResponse</span></span>](deleteitemresponse.md)
    
- [<span data-ttu-id="5c2bd-141">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5c2bd-141">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5c2bd-142">DeleteItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5c2bd-142">DeleteItemResponseMessage</span></span>](deleteitemresponsemessage.md)
    
- [<span data-ttu-id="5c2bd-143">MessageText</span><span class="sxs-lookup"><span data-stu-id="5c2bd-143">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="5c2bd-144">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5c2bd-144">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="5c2bd-145">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="5c2bd-145">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="5c2bd-146">Para localizar outras opções para a mensagem de resposta de erro da operação **DeleteItem** , explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="5c2bd-146">To find other options for the error response message of the **DeleteItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="5c2bd-147">Inicie o elemento [DeleteItemResponse](deleteitemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="5c2bd-147">Start at the [DeleteItemResponse](deleteitemresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="5c2bd-148">Confira também</span><span class="sxs-lookup"><span data-stu-id="5c2bd-148">See also</span></span>

- [<span data-ttu-id="5c2bd-149">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5c2bd-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="5c2bd-150">Excluindo contatos</span><span class="sxs-lookup"><span data-stu-id="5c2bd-150">Deleting Contacts</span></span>](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)  
- [<span data-ttu-id="5c2bd-151">Excluindo emails</span><span class="sxs-lookup"><span data-stu-id="5c2bd-151">Deleting E-mail Messages</span></span>](http://msdn.microsoft.com/library/c40f2f0b-dae0-412f-b716-727e8c0949b4%28Office.15%29.aspx) 
- [<span data-ttu-id="5c2bd-152">A exclusão de tarefas</span><span class="sxs-lookup"><span data-stu-id="5c2bd-152">Deleting Tasks</span></span>](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

