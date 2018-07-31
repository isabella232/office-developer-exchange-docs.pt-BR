---
title: Trabalhar com itens de caixa de correio do Exchange usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 721deb84-f85d-45d0-84c1-0ed55f359969
description: Saiba como criar, obter, atualizar e excluir itens usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: a40cd7ae682c1fb0a8d2f9cfcb10d99d4ab08052
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353963"
---
# <a name="work-with-exchange-mailbox-items-by-using-ews-in-exchange"></a><span data-ttu-id="4b86a-103">Trabalhar com itens de caixa de correio do Exchange usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4b86a-103">Work with Exchange mailbox items by using EWS in Exchange</span></span>

<span data-ttu-id="4b86a-104">Saiba como criar, obter, atualizar e excluir itens usando a API gerenciada de EWS ou EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="4b86a-104">Learn how to create, get, update, and delete items by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="4b86a-105">Você pode usar a API gerenciada de EWS ou o EWS para trabalhar com itens em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="4b86a-105">You can use the EWS Managed API or EWS to work with items in a mailbox.</span></span> <span data-ttu-id="4b86a-106">Você pode usar itens genéricos — objetos de API gerenciada de EWS [Item](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) ou tipos EWS [Item](http://msdn.microsoft.com/library/4dfe8f48-e7b4-444d-bdf9-a34e180f598b%28Office.15%29.aspx) — para executar algumas operações (Obtendo um item ou excluir um item usando o identificador do item); No entanto, na maioria das vezes, que você precisará usar um [item de digitado fortemente](folders-and-items-in-ews-in-exchange.md#bk_item) para realizar um get ou operação de atualização, pois você precisará ter acesso às propriedades que são específicas para o item fortemente tipado.</span><span class="sxs-lookup"><span data-stu-id="4b86a-106">You can use generic items — EWS Managed API [Item](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) objects or EWS [Item](http://msdn.microsoft.com/library/4dfe8f48-e7b4-444d-bdf9-a34e180f598b%28Office.15%29.aspx) types — to perform some operations (getting an item or deleting an item by using the item's identifier); however, most of the time you'll have to use a [strongly typed item](folders-and-items-in-ews-in-exchange.md#bk_item) to perform a get or update operation because you'll need access to the properties that are specific to the strongly typed item.</span></span> 

<span data-ttu-id="4b86a-107">Por exemplo, você não pode usar um item genérico para recuperar um item que contém um início e data de término - você precisa de um objeto de API gerenciada de EWS [compromisso](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) ou um tipo EWS [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) para fazer isso.</span><span class="sxs-lookup"><span data-stu-id="4b86a-107">For example, you can't use a generic item to retrieve an item that contains a start and end date - you need an EWS Managed API [Appointment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object or an EWS [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) type to do that.</span></span> <span data-ttu-id="4b86a-108">E se você estiver usando a API gerenciada de EWS, você sempre precisará criar itens fortemente tipadas, porque a classe genérica do **Item** não tem um construtor.</span><span class="sxs-lookup"><span data-stu-id="4b86a-108">And if you're using the EWS Managed API, you always have to create strongly typed items, because the generic **Item** class does not have a constructor.</span></span> <span data-ttu-id="4b86a-109">Se você estiver trabalhando com um item que não é digitado fortemente, você sempre pode usar a classe do **Item** base para funcionar com o item.</span><span class="sxs-lookup"><span data-stu-id="4b86a-109">If you're working with an item that is not strongly typed, you can always use the base **Item** class to work with the item.</span></span> 
  
<span data-ttu-id="4b86a-110">**Tabela 1. Métodos de API gerenciada de EWS e operações de EWS para trabalhar com itens**</span><span class="sxs-lookup"><span data-stu-id="4b86a-110">**Table 1. EWS Managed API methods and EWS operations for working with items**</span></span>

|<span data-ttu-id="4b86a-111">**Para...**</span><span class="sxs-lookup"><span data-stu-id="4b86a-111">**In order to…**</span></span>|<span data-ttu-id="4b86a-112">**Método API gerenciada de EWS**</span><span class="sxs-lookup"><span data-stu-id="4b86a-112">**EWS Managed API method**</span></span>|<span data-ttu-id="4b86a-113">**Operação do EWS**</span><span class="sxs-lookup"><span data-stu-id="4b86a-113">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="4b86a-114">Criar um item genérico</span><span class="sxs-lookup"><span data-stu-id="4b86a-114">Create a generic item</span></span>  <br/> |<span data-ttu-id="4b86a-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4b86a-115">None.</span></span> <span data-ttu-id="4b86a-116">Você só pode criar tipos de item específico usando a API gerenciada de EWS; não é possível criar itens genéricos.</span><span class="sxs-lookup"><span data-stu-id="4b86a-116">You can only create specific item types by using the EWS Managed API; you cannot create generic items.</span></span>  <br/> |[<span data-ttu-id="4b86a-117">CreateItem</span><span class="sxs-lookup"><span data-stu-id="4b86a-117">CreateItem</span></span>](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="4b86a-118">Obtenha um item</span><span class="sxs-lookup"><span data-stu-id="4b86a-118">Get an item</span></span>  <br/> |[<span data-ttu-id="4b86a-119">Item.Bind</span><span class="sxs-lookup"><span data-stu-id="4b86a-119">Item.Bind</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="4b86a-120">GetItem</span><span class="sxs-lookup"><span data-stu-id="4b86a-120">GetItem</span></span>](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="4b86a-121">Atualização de um item</span><span class="sxs-lookup"><span data-stu-id="4b86a-121">Update an item</span></span>  <br/> |[<span data-ttu-id="4b86a-122">Item.Update</span><span class="sxs-lookup"><span data-stu-id="4b86a-122">Item.Update</span></span>](http://msdn.microsoft.com/en-us/library/office/dd635915%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="4b86a-123">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="4b86a-123">UpdateItem</span></span>](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="4b86a-124">Excluir um item</span><span class="sxs-lookup"><span data-stu-id="4b86a-124">Delete an item</span></span>  <br/> |[<span data-ttu-id="4b86a-125">Item</span><span class="sxs-lookup"><span data-stu-id="4b86a-125">Item.Delete</span></span>](http://msdn.microsoft.com/en-us/library/office/dd635072%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="4b86a-126">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="4b86a-126">DeleteItem</span></span>](../web-service-reference/deleteitem-operation.md) <br/> |
   
<span data-ttu-id="4b86a-127">Neste artigo, você saberá quando você pode usar a classe base genérica e quando você precisa usar um item fortemente tipado para concluir a tarefa.</span><span class="sxs-lookup"><span data-stu-id="4b86a-127">In this article, you'll learn when you can use the generic base class and when you need to use a strongly typed item to complete your task.</span></span> <span data-ttu-id="4b86a-128">Os exemplos de código mostra como usar a classe base e o que fazer quando você não pode usar a classe base ou ele não atender às suas necessidades.</span><span class="sxs-lookup"><span data-stu-id="4b86a-128">The code examples will show you how to use the base class, and what to do when you can't use the base class or it doesn't fit your needs.</span></span>
  
## <a name="create-an-item-by-using-the-ews-managed-api"></a><span data-ttu-id="4b86a-129">Criar um item usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="4b86a-129">Create an item by using the EWS Managed API</span></span>
<span data-ttu-id="4b86a-130"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="4b86a-130"></span></span>

<span data-ttu-id="4b86a-131">A API gerenciada de EWS não tem um construtor publicamente disponível para a classe de [Item](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) , portanto, você deve usar o construtor para o tipo de item específico que você deseja criar para criar um item.</span><span class="sxs-lookup"><span data-stu-id="4b86a-131">The EWS Managed API does not have a publicly available constructor for the [Item](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) class, so you must use the constructor for the specific item type you want to create in order to create an item.</span></span> <span data-ttu-id="4b86a-132">Por exemplo, use o [Construtor de classe EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.emailmessage%28v=exchg.80%29.aspx) para criar uma nova mensagem de email e o [Construtor de classe de contato](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) para criar um novo contato.</span><span class="sxs-lookup"><span data-stu-id="4b86a-132">For example, use the [EmailMessage class constructor](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.emailmessage%28v=exchg.80%29.aspx) to create a new email message, and the [Contact class constructor](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) to create a new contact.</span></span> <span data-ttu-id="4b86a-133">Da mesma forma, o servidor retorna nunca genéricos objetos de **Item** nas respostas; todos os itens genéricos são retornados como objetos **EmailMessage** .</span><span class="sxs-lookup"><span data-stu-id="4b86a-133">Likewise, the server never returns generic **Item** objects in responses; all generic items are returned as **EmailMessage** objects.</span></span> 
  
<span data-ttu-id="4b86a-134">Quando você sabe o tipo de item para criar, você pode concluir a tarefa em apenas algumas etapas.</span><span class="sxs-lookup"><span data-stu-id="4b86a-134">When you know the type of item to create, you can complete the task in just a few steps.</span></span> <span data-ttu-id="4b86a-135">As etapas são semelhantes para todos os tipos de item:</span><span class="sxs-lookup"><span data-stu-id="4b86a-135">The steps are similar for all item types:</span></span>
  
1. <span data-ttu-id="4b86a-136">Inicialize uma nova instância de uma das classes de [Item](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) com o objeto [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) como um parâmetro.</span><span class="sxs-lookup"><span data-stu-id="4b86a-136">Initialize a new instance of one of the [Item](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) classes with the [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object as a parameter.</span></span> 
    
2. <span data-ttu-id="4b86a-137">Definir as propriedades do item.</span><span class="sxs-lookup"><span data-stu-id="4b86a-137">Set properties on the item.</span></span> <span data-ttu-id="4b86a-138">Os esquemas são diferentes para cada tipo de item, portanto propriedades diferentes estão disponíveis para itens diferentes.</span><span class="sxs-lookup"><span data-stu-id="4b86a-138">The schemas are different for each item type, so different properties are available for different items.</span></span>
    
3. <span data-ttu-id="4b86a-139">Salvar o item, ou salvar e enviar o item.</span><span class="sxs-lookup"><span data-stu-id="4b86a-139">Save the item, or save and send the item.</span></span>
    
<span data-ttu-id="4b86a-140">Por exemplo, você pode criar um objeto [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) , definir o [assunto](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.subject%28v=exchg.80%29.aspx), [corpo](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.body%28v=exchg.80%29.aspx)e propriedades [ToRecipients](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.torecipients%28v=exchg.80%29.aspx) e depois enviá-la usando o método [EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="4b86a-140">For example, you can create an [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object, set the [Subject](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.subject%28v=exchg.80%29.aspx), [Body](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.body%28v=exchg.80%29.aspx), and [ToRecipients](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.torecipients%28v=exchg.80%29.aspx) properties, and then send it by using the [EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) method.</span></span> 
  
```cs
// Create an email message and provide it with connection 
// configuration information by using an ExchangeService object named service.
EmailMessage message = new EmailMessage(service);
// Set properties on the email message.
message.Subject = "Company Soccer Team";
message.Body = "Are you interested in joining?";
message.ToRecipients.Add("sadie@contoso.com");
// Send the email message and save a copy.
// This method call results in a CreateItem call to EWS.
message.SendAndSaveCopy();
```

<span data-ttu-id="4b86a-141">Para saber como criar uma reunião ou um item de compromisso usando a API gerenciada de EWS, consulte [criar compromissos e reuniões usando o EWS no Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md).</span><span class="sxs-lookup"><span data-stu-id="4b86a-141">To learn how to create a meeting or appointment item by using the EWS Managed API, see [Create appointments and meetings by using EWS in Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md).</span></span>
  
## <a name="create-an-item-by-using-ews"></a><span data-ttu-id="4b86a-142">Criar um item usando o EWS</span><span class="sxs-lookup"><span data-stu-id="4b86a-142">Create an item by using EWS</span></span>
<span data-ttu-id="4b86a-143"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="4b86a-143"></span></span>

<span data-ttu-id="4b86a-144">Você pode criar um item genérico ou um item de fortemente tipado usando o EWS.</span><span class="sxs-lookup"><span data-stu-id="4b86a-144">You can create a generic item or a strongly typed item by using EWS.</span></span> <span data-ttu-id="4b86a-145">As etapas são semelhantes para todos os tipos de item:</span><span class="sxs-lookup"><span data-stu-id="4b86a-145">The steps are similar for all item types:</span></span>
  
1. <span data-ttu-id="4b86a-146">Use a operação [CreateItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) para criar um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4b86a-146">Use the [CreateItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) operation to create an item in the Exchange store.</span></span> 
    
2. <span data-ttu-id="4b86a-147">Use o elemento de [itens](http://msdn.microsoft.com/library/0811a73e-bf1f-4889-9219-73902dd47639%28Office.15%29.aspx) para conter um ou mais itens para criar.</span><span class="sxs-lookup"><span data-stu-id="4b86a-147">Use the [Items](http://msdn.microsoft.com/library/0811a73e-bf1f-4889-9219-73902dd47639%28Office.15%29.aspx) element to contain one or more items to create.</span></span> 
    
3. <span data-ttu-id="4b86a-148">Definir as propriedades do item.</span><span class="sxs-lookup"><span data-stu-id="4b86a-148">Set properties on the item.</span></span>
    
<span data-ttu-id="4b86a-149">Por exemplo, você pode criar uma mensagem de email e enviá-la usando o código no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="4b86a-149">For example, you can create an email message and send it by using the code in the following example.</span></span> <span data-ttu-id="4b86a-150">Isso também é a solicitação XML que o EWS Managed API envia ao chamar o método [SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="4b86a-150">This is also the XML request that the EWS Managed API sends when you call the [SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) method.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="sentitems" />
      </m:SavedItemFolderId>
      <m:Items>
        <t:Message>
          <t:Subject>Company Soccer Team</t:Subject>
          <t:Body BodyType="HTML">Are you interested in joining?</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sadie@contoso.com </t:EmailAddress>
              </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="4b86a-151">O servidor responde à solicitação **CreateItem** com uma mensagem de [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) que inclui um valor de [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) de **NoError**, que indica se o email foi criado com êxito e o [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) do recentemente mensagem criada.</span><span class="sxs-lookup"><span data-stu-id="4b86a-151">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was created successfully, and the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the newly created message.</span></span> 
  
<span data-ttu-id="4b86a-152">Para saber como criar um item de compromisso ou uma reunião usando o EWS, consulte [criar compromissos e reuniões usando o EWS no Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md).</span><span class="sxs-lookup"><span data-stu-id="4b86a-152">To learn how to create a meeting or appointment item by using EWS, see [Create appointments and meetings by using EWS in Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md).</span></span>
  
## <a name="get-an-item-by-using-the-ews-managed-api"></a><span data-ttu-id="4b86a-153">Obter um item usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="4b86a-153">Get an item by using the EWS Managed API</span></span>
<span data-ttu-id="4b86a-154"><a name="bk_getewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="4b86a-154"></span></span>

<span data-ttu-id="4b86a-155">Para usar a API gerenciada de EWS para obter um item se você souber a [Item.Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) do item para recuperar, basta chamar um dos métodos [vincular](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) no item e o item será recuperado.</span><span class="sxs-lookup"><span data-stu-id="4b86a-155">To use the EWS Managed API to get an item if you know the [Item.Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to retrieve, you simply call one of the [Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) methods on the item, and the item is retrieved.</span></span> <span data-ttu-id="4b86a-156">Como prática recomendada, recomendamos que você limite as propriedades retornadas somente àqueles que são necessários.</span><span class="sxs-lookup"><span data-stu-id="4b86a-156">As a best practice, we recommend that you limit the properties returned to only those that are required.</span></span> <span data-ttu-id="4b86a-157">Este exemplo retorna a propriedade de **Id** de item e a propriedade **Subject** .</span><span class="sxs-lookup"><span data-stu-id="4b86a-157">This example returns the item **Id** property and the **Subject** property.</span></span> 
  
<span data-ttu-id="4b86a-158">Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="4b86a-158">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="4b86a-159">A variável local *itemId* é a [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) do item para atualizar.</span><span class="sxs-lookup"><span data-stu-id="4b86a-159">The local variable  *itemId*  is the [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to update.</span></span> 
  
```cs
// As a best practice, limit the properties returned to only those that are required.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, ItemSchema.Subject);
// Bind to the existing item by using the ItemId.
// This method call results in a GetItem call to EWS.
Item item = Item.Bind(service, itemId, propSet);

```

<span data-ttu-id="4b86a-160">Se você estiver procurando por um item que atenda a critérios específicos, faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="4b86a-160">If you're searching for an item that meets specific criteria, do the following:</span></span>
  
1. <span data-ttu-id="4b86a-161">Ligar para a pasta que contém os itens a ser obtido.</span><span class="sxs-lookup"><span data-stu-id="4b86a-161">Bind to the folder that contains the items to get.</span></span>
    
2. <span data-ttu-id="4b86a-162">Criar uma instância de um [SearchFilter.SearchFilterCollection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) ou um [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) para filtrar os itens a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="4b86a-162">Instantiate a [SearchFilter.SearchFilterCollection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) or a [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) to filter the items to return.</span></span> 
    
3. <span data-ttu-id="4b86a-163">Criar uma instância de um objeto [CalendarView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) ou de [ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) para especificar o número de itens para retornar.</span><span class="sxs-lookup"><span data-stu-id="4b86a-163">Instantiate an [ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) or [CalendarView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) object to specify the number of items to return.</span></span> 
    
4. <span data-ttu-id="4b86a-164">Chame o método [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) ou [ExchangeService.FindAppointments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="4b86a-164">Call the [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) or [ExchangeService.FindAppointments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) method.</span></span> 
    
<span data-ttu-id="4b86a-165">Por exemplo, se você quiser recuperar mensagens de email não lido na caixa de entrada, use o código no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="4b86a-165">For example, if you want to retrieve unread email messages in the Inbox, use the code in the following example.</span></span> <span data-ttu-id="4b86a-166">Este exemplo usa um **SearchFilterCollection** para limitar os resultados do método **FindItems** a mensagens não lidas e limita a **ItemView** para limitar os resultados para um item.</span><span class="sxs-lookup"><span data-stu-id="4b86a-166">This example uses a **SearchFilterCollection** to limit the results of the **FindItems** method to unread messages, and limits the **ItemView** to limit results to one item.</span></span> <span data-ttu-id="4b86a-167">Este código determinado funciona somente em objetos [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) porque o valor de [EmailMessageSchema.IsRead](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessageschema.isread%28v=exchg.80%29.aspx) é parte do **SearchFilter**.</span><span class="sxs-lookup"><span data-stu-id="4b86a-167">This particular code only works on [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) objects because the [EmailMessageSchema.IsRead](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessageschema.isread%28v=exchg.80%29.aspx) value is part of the **SearchFilter**.</span></span> 
  
```cs
// Bind the Inbox folder to the service object.
Folder inbox = Folder.Bind(service, WellKnownFolderName.Inbox);
// The search filter to get unread email.
SearchFilter sf = new SearchFilter.SearchFilterCollection(LogicalOperator.And, new SearchFilter.IsEqualTo(EmailMessageSchema.IsRead, false));
ItemView view = new ItemView(1);
// Fire the query for the unread items.
// This method call results in a FindItem call to EWS.
FindItemsResults<Item> findResults = service.FindItems(WellKnownFolderName.Inbox, sf, view);
```

<span data-ttu-id="4b86a-168">Como alternativa, você pode usar um [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) para limitar os resultados da pesquisa, conforme mostrado no exemplo de código a seguir.</span><span class="sxs-lookup"><span data-stu-id="4b86a-168">Alternatively, you can use a [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) to limit the results of the search as shown in the following code example.</span></span> <span data-ttu-id="4b86a-169">Este exemplo usa o método [FindAppointments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) para recuperar até cinco compromissos que ocorrem nos próximos 30 dias.</span><span class="sxs-lookup"><span data-stu-id="4b86a-169">This example uses the [FindAppointments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) method to retrieve up to five appointments that occur in the next 30 days.</span></span> <span data-ttu-id="4b86a-170">Este código Obviamente só funciona nos itens de calendário.</span><span class="sxs-lookup"><span data-stu-id="4b86a-170">This code of course only works on calendar items.</span></span> 
  
```cs
// Initialize values for the start and end times, and the number of appointments to retrieve.
DateTime startDate = DateTime.Now;
DateTime endDate = startDate.AddDays(30);
const int NUM_APPTS = 5;
// Bind the Calendar folder to the service object.
// This method call results in a GetFolder call to EWS.
CalendarFolder calendar = CalendarFolder.Bind(service, WellKnownFolderName.Calendar, new PropertySet());
// Set the start and end time and number of appointments to retrieve.
CalendarView cView = new CalendarView(startDate, endDate, NUM_APPTS);
// Limit the properties returned to the appointment's subject, start time, and end time.
cView.PropertySet = new PropertySet(AppointmentSchema.Subject, AppointmentSchema.Start, AppointmentSchema.End);
// Retrieve a collection of appointments by using the calendar view.
// This method call results in a FindAppointments call to EWS.
FindItemsResults<Appointment> appointments = calendar.FindAppointments(cView);
```

<span data-ttu-id="4b86a-171">Observe que as informações do servidor retorna a resposta do método **vincular** é diferente do que as informações que o servidor retorna uma resposta de método **FindItem** ou **FindAppointment** .</span><span class="sxs-lookup"><span data-stu-id="4b86a-171">Note that the information the server returns in the **Bind** method response is different than the information that the server returns for a **FindItem** or **FindAppointment** method response.</span></span> <span data-ttu-id="4b86a-172">O método **vincular** pode retornar todas as propriedades esquematizadas, enquanto os métodos **FindItem** e **FindAppointment** não retornará todas as propriedades esquematizadas.</span><span class="sxs-lookup"><span data-stu-id="4b86a-172">The **Bind** method can return all the schematized properties, whereas the **FindItem** and **FindAppointment** methods do not return all the schematized properties.</span></span> <span data-ttu-id="4b86a-173">Tão se precisar de acesso completo ao item, você terá que usar o método **vincular** .</span><span class="sxs-lookup"><span data-stu-id="4b86a-173">So if you need full access to the item, you'll have to use the **Bind** method.</span></span> <span data-ttu-id="4b86a-174">Se você não tiver o item a **Id** do item você gostaria de recuperar, use os métodos **FindItem** ou **FindAppointment** para recuperar o Id e, em seguida, use o método **ligar** para recuperar as propriedades que você precisa.</span><span class="sxs-lookup"><span data-stu-id="4b86a-174">If you don't have the item **Id** of the item you'd like to retrieve, use the **FindItem** or **FindAppointment** methods to retrieve the Id, and then use the **Bind** method to retrieve the properties you need.</span></span> 
  
<span data-ttu-id="4b86a-175">Para saber como obter uma reunião ou um item de compromisso usando a API gerenciada de EWS, consulte [obter compromissos e reuniões usando o EWS no Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="4b86a-175">To learn how to get a meeting or appointment item by using the EWS Managed API, see [Get appointments and meetings by using EWS in Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).</span></span>
  
## <a name="get-an-item-by-using-ews"></a><span data-ttu-id="4b86a-176">Obter um item usando o EWS</span><span class="sxs-lookup"><span data-stu-id="4b86a-176">Get an item by using EWS</span></span>
<span data-ttu-id="4b86a-177"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="4b86a-177"></span></span>

<span data-ttu-id="4b86a-178">Se você souber o [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) do item para recuperar, você pode obter o item usando a operação [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="4b86a-178">If you know the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the item to retrieve, you can get the item by using the [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) operation.</span></span> 
  
<span data-ttu-id="4b86a-179">O exemplo a seguir mostra a solicitação XML para obter o [assunto](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) de um item com um específicos **ItemId**.</span><span class="sxs-lookup"><span data-stu-id="4b86a-179">The following example shows the XML request to get the [Subject](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) of an item with a specific **ItemId**.</span></span> <span data-ttu-id="4b86a-180">Isso também é a solicitação XML que o EWS Managed API envia ao chamar o método [ligar](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) em um **ItemId**.</span><span class="sxs-lookup"><span data-stu-id="4b86a-180">This is also the XML request that the EWS Managed API sends when calling the [Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) method on an **ItemId**.</span></span> <span data-ttu-id="4b86a-181">Os valores de alguns atributos e elementos foram diminuídos para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4b86a-181">The values of some attributes and elements have been shortened for readability.</span></span>
  
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
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="GJc/NAAA=" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

O exemplo a seguir mostra a resposta XML que o servidor retorna após processa a operação **GetItem** . A resposta indica que o item foi recuperado com êxito. <span data-ttu-id="4b86a-184">Os valores de alguns atributos e elementos foram diminuídos para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4b86a-184">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="815" 
                         MinorBuildNumber="6" 
                         Version="V2_7" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemId Id="GJc/NAAA=" ChangeKey="CQAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAGJd9Z"/>
              <t:Subject>Company Soccer Team</t:Subject>
            </t:Message>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="4b86a-185">Se você não souber o **ItemId** do item que deseja recuperar, você pode usar a operação [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) para localizar o item.</span><span class="sxs-lookup"><span data-stu-id="4b86a-185">If you do not know the **ItemId** of the item you want to retrieve, you can use the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation to find the item.</span></span> <span data-ttu-id="4b86a-186">Para usar a operação **FindItem** , você deve primeiro identificar a pasta que você está procurando.</span><span class="sxs-lookup"><span data-stu-id="4b86a-186">In order to use the **FindItem** operation, you must first identify the folder that you're searching.</span></span> <span data-ttu-id="4b86a-187">Você pode identificar a pasta usando seu **DistinguinguishedFolderName** ou usando o [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="4b86a-187">You can identify the folder by using its **DistinguinguishedFolderName** or by using the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx).</span></span> <span data-ttu-id="4b86a-188">Você pode usar o [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) ou [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) operações para obter **FolderId** você precisa.</span><span class="sxs-lookup"><span data-stu-id="4b86a-188">You can use either the [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) or [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) operations to get the **FolderId** you need.</span></span> <span data-ttu-id="4b86a-189">Em seguida, use a operação de **FindItem** para pesquisar dessa pasta para obter os resultados que correspondem ao filtro de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4b86a-189">Then use the **FindItem** operation to search that folder for results that match the search filter.</span></span> <span data-ttu-id="4b86a-190">Diferentemente da API gerenciada de EWS, EWS não fornece uma operação de localização separado para compromissos.</span><span class="sxs-lookup"><span data-stu-id="4b86a-190">Unlike the EWS Managed API, EWS does not provide a separate find operation for appointments.</span></span> <span data-ttu-id="4b86a-191">A operação **FindItem** recupera itens de todos os tipos.</span><span class="sxs-lookup"><span data-stu-id="4b86a-191">The **FindItem** operation retrieves items of all types.</span></span> 
  
<span data-ttu-id="4b86a-192">O exemplo a seguir mostra a solicitação de operação de XML **FindItem** que será enviada para o servidor para encontrar os compromissos na pasta de calendário que ocorrem nos próximos 30 dias.</span><span class="sxs-lookup"><span data-stu-id="4b86a-192">The following example shows the XML **FindItem** operation request that is sent to the server to find appointments in the Calendar folder that occur in the next 30 days.</span></span> <span data-ttu-id="4b86a-193">Os valores de alguns atributos e elementos foram diminuídos para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4b86a-193">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="calendar:Start" />
          <t:FieldURI FieldURI="calendar:End" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:CalendarView MaxEntriesReturned="5" StartDate="2013-10-16T17:04:28.722Z" EndDate="2013-11-15T18:04:28.722Z" />
      <m:ParentFolderIds>
        <t:FolderId Id="AAAEOAAA=" ChangeKey="AgAAABYAAAAqRr3mNdNMSasqx/o9J13UAAAAAAA3" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="4b86a-194">O servidor responde à solicitação **FindItem** com uma mensagem de [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) que inclui o valor de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica que a operação foi concluída com êxito.</span><span class="sxs-lookup"><span data-stu-id="4b86a-194">The server responds to the **FindItem** request with a [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) message that includes the [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the operation completed successfully.</span></span> <span data-ttu-id="4b86a-195">Se quaisquer itens de calendário de acordo com os critérios de filtragem, eles são incluídos na resposta.</span><span class="sxs-lookup"><span data-stu-id="4b86a-195">If any calendar items meet the filtering criteria, they are included in the response.</span></span>
  
<span data-ttu-id="4b86a-196">Observe que as informações do servidor retorna a resposta de operação **GetItem** é diferente do que as informações que o servidor retorna em uma **FindItem** ou a resposta de operação **FindAppointment** .</span><span class="sxs-lookup"><span data-stu-id="4b86a-196">Note that the information the server returns in the **GetItem** operation response is different than the information the server returns in a **FindItem** or **FindAppointment** operation response.</span></span> <span data-ttu-id="4b86a-197">A operação **GetItem** pode retornar todas as propriedades esquematizadas, enquanto as operações **FindItem** e **FindAppointment** não retornará todas as propriedades esquematizadas.</span><span class="sxs-lookup"><span data-stu-id="4b86a-197">The **GetItem** operation can return all the schematized properties, whereas the **FindItem** and **FindAppointment** operations do not return all the schematized properties.</span></span> <span data-ttu-id="4b86a-198">Isso se você precisar de acesso completo ao item, você terá que usar a operação **GetItem** .</span><span class="sxs-lookup"><span data-stu-id="4b86a-198">So if you need full access to the item, you'll have to use the **GetItem** operation.</span></span> <span data-ttu-id="4b86a-199">Se você não tiver o **ItemId** do item você gostaria de recuperar, use as operações **FindItem** ou **FindAppointment** para recuperar o **ItemId**e, em seguida, use a operação de **GetItem** para recuperar os elementos que você precisa.</span><span class="sxs-lookup"><span data-stu-id="4b86a-199">If you don't have the **ItemId** of the item you'd like to retrieve, use the **FindItem** or **FindAppointment** operations to retrieve the **ItemId**, and then use the **GetItem** operation to retrieve the elements you need.</span></span> 
  
<span data-ttu-id="4b86a-200">Para saber como obter um item de compromisso ou uma reunião usando o EWS, consulte [obter compromissos e reuniões usando o EWS no Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="4b86a-200">To learn how to get a meeting or appointment item by using EWS, see [Get appointments and meetings by using EWS in Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).</span></span>
  
## <a name="update-an-item-by-using-the-ews-managed-api"></a><span data-ttu-id="4b86a-201">Atualização de um item usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="4b86a-201">Update an item by using the EWS Managed API</span></span>
<span data-ttu-id="4b86a-202"><a name="bk_updateewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="4b86a-202"></span></span>

<span data-ttu-id="4b86a-203">As etapas para atualizar um item usando a API gerenciada de EWS são semelhantes para todos os tipos de item. No entanto, as propriedades do item são diferentes para cada tipo de item e o método [Update](http://msdn.microsoft.com/en-us/library/office/dd635915%28v=exchg.80%29.aspx) tem vários métodos sobrecarregados à sua escolha.</span><span class="sxs-lookup"><span data-stu-id="4b86a-203">The steps to update an item by using the EWS Managed API are similar for all item types; however, the item properties are different for each item type, and the [Update](http://msdn.microsoft.com/en-us/library/office/dd635915%28v=exchg.80%29.aspx) method has many overloaded methods to choose from.</span></span> <span data-ttu-id="4b86a-204">Para atualizar um item:</span><span class="sxs-lookup"><span data-stu-id="4b86a-204">To update an item:</span></span> 
  
1. <span data-ttu-id="4b86a-205">Use o método [ligar](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) para obter a versão mais recente do item, a menos que você já tem.</span><span class="sxs-lookup"><span data-stu-id="4b86a-205">Use the [Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) method to get the latest version of the item, unless you already have it.</span></span> <span data-ttu-id="4b86a-206">Para atualizar propriedades específicas para um item fortemente tipado, você terá que associar a esse tipo de item.</span><span class="sxs-lookup"><span data-stu-id="4b86a-206">To update properties specific to a strongly typed item, you'll have to bind to that item type.</span></span> <span data-ttu-id="4b86a-207">Para atualizar as propriedades disponíveis no tipo de item genérico, é possível vincular o objeto de [Item](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="4b86a-207">To update properties available on the generic item type, you can bind to the [Item](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) object.</span></span> 
    
2. <span data-ttu-id="4b86a-208">Atualize as propriedades no item.</span><span class="sxs-lookup"><span data-stu-id="4b86a-208">Update the properties on the item.</span></span>
    
3. <span data-ttu-id="4b86a-209">Chame o método **Update** .</span><span class="sxs-lookup"><span data-stu-id="4b86a-209">Call the **Update** method.</span></span> 
    
<span data-ttu-id="4b86a-210">Por exemplo, você pode atualizar o assunto de um email usando o tipo de item genérico, conforme mostrado no código no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="4b86a-210">For example, you can update the subject of an email by using the generic item type, as shown in the code in the following example.</span></span>
  
<span data-ttu-id="4b86a-211">Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="4b86a-211">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="4b86a-212">A variável local *itemId* é a [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) do item para atualizar.</span><span class="sxs-lookup"><span data-stu-id="4b86a-212">The local variable  *itemId*  is the [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to update.</span></span> 
  
```cs
// Bind to the existing item, using the ItemId.
// This method call results in a GetItem call to EWS.
Item item = Item.Bind(service, itemId);
// Update the Subject of the email.
item.Subject = "New subject";
// Save the updated email.
// This method call results in an UpdateItem call to EWS.
item.Update(ConflictResolutionMode.AlwaysOverwrite);
```

<span data-ttu-id="4b86a-213">Para saber como atualizar de uma reunião ou um item de compromisso usando a API gerenciada de EWS, consulte [atualizar compromissos e reuniões usando o EWS no Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="4b86a-213">To learn how to update a meeting or appointment item by using the EWS Managed API, see [Update appointments and meetings by using EWS in Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md).</span></span>
  
## <a name="update-an-item-by-using-ews"></a><span data-ttu-id="4b86a-214">Atualizar um item usando o EWS</span><span class="sxs-lookup"><span data-stu-id="4b86a-214">Update an item by using EWS</span></span>
<span data-ttu-id="4b86a-215"><a name="bk_updateews"> </a></span><span class="sxs-lookup"><span data-stu-id="4b86a-215"></span></span>

<span data-ttu-id="4b86a-216">Para atualizar um item usando o EWS, faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="4b86a-216">To update an item by using EWS, do the following:</span></span>
  
1. <span data-ttu-id="4b86a-217">Use a operação de [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) obter a versão mais recente do item, a menos que você já possui.</span><span class="sxs-lookup"><span data-stu-id="4b86a-217">Use the [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) operation to get the latest version of the item, unless you already have it.</span></span> 
    
2. <span data-ttu-id="4b86a-218">Use a operação [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) para especificar os campos para atualizar e destinar novos valores aos campos.</span><span class="sxs-lookup"><span data-stu-id="4b86a-218">Use the [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) operation to specify fields to update and assign new values to those fields.</span></span> 
    
<span data-ttu-id="4b86a-219">O exemplo a seguir mostra a solicitação de operação de XML **UpdateItem** que será enviada para o servidor para atualizar o valor de [assunto](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) da mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="4b86a-219">The following example shows the XML **UpdateItem** operation request that is sent to the server to update the [Subject](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) value of the email message.</span></span> <span data-ttu-id="4b86a-220">Os valores de alguns atributos e elementos foram diminuídos para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4b86a-220">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AlwaysOverwrite">
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="APdZjAAA=" ChangeKey="CQAAABYAAAAqRr3mNdNMSasqx/o9J13UAAAAPdgr" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:Message>
                <t:Subject>New subject</t:Subject>
              </t:Message>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="4b86a-221">O servidor responde à solicitação **UpdateItem** com uma mensagem de [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) que inclui o valor [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError**, que indica se a atualização de item foi bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="4b86a-221">The server responds to the **UpdateItem** request with a [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) message that includes the a [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the item update was successful.</span></span>
  
<span data-ttu-id="4b86a-222">Para saber como atualizar de uma reunião ou um item de compromisso usando o EWS, consulte [atualizar compromissos e reuniões usando o EWS no Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="4b86a-222">To learn how to update a meeting or appointment item by using EWS, see [Update appointments and meetings by using EWS in Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md).</span></span>
  
## <a name="delete-an-item-by-using-the-ews-managed-api"></a><span data-ttu-id="4b86a-223">Excluir um item usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="4b86a-223">Delete an item by using the EWS Managed API</span></span>
<span data-ttu-id="4b86a-224"><a name="bk_deleteewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="4b86a-224"></span></span>

<span data-ttu-id="4b86a-225">Você pode excluir itens ao movê-las para a pasta Itens excluídos ou para o dumpster.</span><span class="sxs-lookup"><span data-stu-id="4b86a-225">You can delete items by moving them to the Deleted Items folder or to the dumpster.</span></span> <span data-ttu-id="4b86a-226">Se você souber o [ItemId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) do item para excluir, chame o método [Delete](http://msdn.microsoft.com/en-us/library/office/dd635072%28v=exchg.80%29.aspx) no item.</span><span class="sxs-lookup"><span data-stu-id="4b86a-226">If you know the [ItemId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to delete, just call the [Delete](http://msdn.microsoft.com/en-us/library/office/dd635072%28v=exchg.80%29.aspx) method on the item.</span></span> 
  
<span data-ttu-id="4b86a-227">Se você precisar localizar o item antes de excluí-lo, faça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="4b86a-227">If you need to find the item before deleting it, do the following:</span></span>
  
1. <span data-ttu-id="4b86a-228">Chame o método [FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) ou [FindAppointments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) para localizar o item a ser excluído.</span><span class="sxs-lookup"><span data-stu-id="4b86a-228">Call the [FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) or [FindAppointments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) method to find the item to delete.</span></span> 
    
1. <span data-ttu-id="4b86a-229">Instanciar um [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) e limitar o às propriedades para retornar ou usar um [SearchFilterCollection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) para encontrar itens específicos.</span><span class="sxs-lookup"><span data-stu-id="4b86a-229">Instantiate a [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) and limit it to the properties to return, or use a [SearchFilterCollection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) to find specific items.</span></span> 
    
2. <span data-ttu-id="4b86a-230">Criar uma instância de um [ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) ou [CalendarView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) para especificar o número de itens para retornar.</span><span class="sxs-lookup"><span data-stu-id="4b86a-230">Instantiate an [ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) or [CalendarView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) to specify the number of items to return.</span></span> 
    
2. <span data-ttu-id="4b86a-231">Chame o método [Delete](http://msdn.microsoft.com/en-us/library/office/dd635072%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="4b86a-231">Call the [Delete](http://msdn.microsoft.com/en-us/library/office/dd635072%28v=exchg.80%29.aspx) method.</span></span> 
    
<span data-ttu-id="4b86a-232">Por exemplo, o código a seguir mostra como mover uma mensagem de email para a pasta Itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="4b86a-232">For example, the following code shows how to move an email message to the Deleted Items folder.</span></span>
  
<span data-ttu-id="4b86a-233">Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="4b86a-233">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="4b86a-234">A variável local *itemId* é a [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) do item para atualizar.</span><span class="sxs-lookup"><span data-stu-id="4b86a-234">The local variable  *itemId*  is the [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to update.</span></span> 
  
```cs
// Bind to the existing item, using the ItemId.
// This method call results in a GetItem call to EWS.
Item item = Item.Bind(service, itemId);
// Delete the item by moving it to the Deleted Items folder.
// This method call results in a DeleteItem call to EWS.
item.Delete(DeleteMode.MoveToDeletedItems);
```

<span data-ttu-id="4b86a-235">Para obter mais detalhes sobre a exclusão de itens, consulte [Excluindo itens usando o EWS no Exchange](deleting-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="4b86a-235">For more details about deleting items, see [Deleting items by using EWS in Exchange](deleting-items-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="4b86a-236">Para saber como excluir um item de compromisso ou uma reunião usando a API gerenciada de EWS, consulte [Excluir compromissos e cancelar reuniões usando o EWS no Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="4b86a-236">To learn how to delete a meeting or appointment item by using the EWS Managed API, see [Delete appointments and cancel meetings by using EWS in Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).</span></span>
  
## <a name="delete-an-item-by-using-ews"></a><span data-ttu-id="4b86a-237">Excluir um item usando o EWS</span><span class="sxs-lookup"><span data-stu-id="4b86a-237">Delete an item by using EWS</span></span>
<span data-ttu-id="4b86a-238"><a name="bk_deleteews"> </a></span><span class="sxs-lookup"><span data-stu-id="4b86a-238"></span></span>

<span data-ttu-id="4b86a-239">Você pode excluir um item usando a operação [DeleteItem](../web-service-reference/deleteitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4b86a-239">You can delete an item by using the [DeleteItem](../web-service-reference/deleteitem-operation.md) operation.</span></span> 
  
<span data-ttu-id="4b86a-240">O exemplo a seguir mostra a solicitação XML que será enviada para o servidor para mover a mensagem de email para a pasta Itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="4b86a-240">The following example shows the XML request that is sent to the server to move the email message to the Deleted Items folder.</span></span> <span data-ttu-id="4b86a-241">Os valores de alguns atributos e elementos foram diminuídos para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4b86a-241">The values of some attributes and elements have been shortened for readability.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:DeleteItem DeleteType="MoveToDeletedItems">
      <m:ItemIds>
        <t:ItemId Id="APdZjAAA=" ChangeKey="CQAAABYAAAAqRr3mNdNMSasqx/o9J13UAAANIFzC" />
      </m:ItemIds>
    </m:DeleteItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="4b86a-242">O servidor responde à solicitação **DeleteItem** com uma mensagem de [DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) que inclui o valor [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError**, que indica que a exclusão de item foi bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="4b86a-242">The server responds to the **DeleteItem** request with a [DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) message that includes the a [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the item deletion was successful.</span></span>
  
<span data-ttu-id="4b86a-243">Para obter mais detalhes sobre a exclusão de itens, consulte [Excluindo itens usando o EWS no Exchange](deleting-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="4b86a-243">For more details about deleting items, see [Deleting items by using EWS in Exchange](deleting-items-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="4b86a-244">Para saber como excluir um item de compromisso ou uma reunião usando o EWS, consulte [Excluir compromissos e cancelar reuniões usando o EWS no Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="4b86a-244">To learn how to delete a meeting or appointment item by using EWS, see [Delete appointments and cancel meetings by using EWS in Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).</span></span>
  
## <a name="move-or-copy-items-to-another-mailbox"></a><span data-ttu-id="4b86a-245">Mover ou copiar itens para outra caixa de correio</span><span class="sxs-lookup"><span data-stu-id="4b86a-245">Move or copy items to another mailbox</span></span>
<span data-ttu-id="4b86a-246"><a name="bk_movecopybtnmailboxes"> </a></span><span class="sxs-lookup"><span data-stu-id="4b86a-246"></span></span>

<span data-ttu-id="4b86a-247">Você pode mover ou copiar itens entre caixas de correio usando as operações [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) e [UploadItems](http://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="4b86a-247">You can move or copy items between mailboxes by using the [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) and [UploadItems](http://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) operations.</span></span> <span data-ttu-id="4b86a-248">Para saber mais, consulte [Exportar e importar itens usando o EWS no Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="4b86a-248">To learn more, see [Exporting and importing items by using EWS in Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="4b86a-249">Confira também</span><span class="sxs-lookup"><span data-stu-id="4b86a-249">See also</span></span>

- [<span data-ttu-id="4b86a-250">Pastas e itens no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4b86a-250">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)    
- [<span data-ttu-id="4b86a-251">Trabalhar com pastas usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4b86a-251">Work with folders by using EWS in Exchange</span></span>](how-to-work-with-folders-by-using-ews-in-exchange.md)    
- [<span data-ttu-id="4b86a-252">Excluindo itens usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4b86a-252">Deleting items by using EWS in Exchange</span></span>](deleting-items-by-using-ews-in-exchange.md)
    

