---
title: Operação FindItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindItem
api_type:
- schema
ms.assetid: ebad6aae-16e7-44de-ae63-a95b24539729
description: Encontre informações sobre o EWS FindItem operação.
ms.openlocfilehash: b033ac2930981819a20f1336d40058a5f7c03b89
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752289"
---
# <a name="finditem-operation"></a><span data-ttu-id="87d92-103">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="87d92-103">FindItem operation</span></span>

<span data-ttu-id="87d92-104">Encontre informações sobre a operação de EWS **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="87d92-104">Find information about the **FindItem** EWS operation.</span></span> 
  
<span data-ttu-id="87d92-105">A operação **FindItem** procura itens que estão localizados na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="87d92-105">The **FindItem** operation searches for items that are located in a user's mailbox.</span></span> <span data-ttu-id="87d92-106">Esta operação fornece várias maneiras para filtrar e formato como os resultados da pesquisa são retornados ao chamador.</span><span class="sxs-lookup"><span data-stu-id="87d92-106">This operation provides many ways to filter and format how search results are returned to the caller.</span></span> 
  
## <a name="using-the-finditem-operation"></a><span data-ttu-id="87d92-107">Usando a operação FindItem</span><span class="sxs-lookup"><span data-stu-id="87d92-107">Using the FindItem operation</span></span>

<span data-ttu-id="87d92-108">A solicitação de operação **FindItem** oferece diversas maneiras para pesquisar uma caixa de correio e o formato como os dados são retornados em uma resposta.</span><span class="sxs-lookup"><span data-stu-id="87d92-108">The **FindItem** operation request provides many ways for you to search a mailbox and format how the data is returned in a response.</span></span> <span data-ttu-id="87d92-109">Você pode especificar o seguinte em uma solicitação de **FindItem** :</span><span class="sxs-lookup"><span data-stu-id="87d92-109">You can specify the following in a **FindItem** request:</span></span> 
  
- <span data-ttu-id="87d92-110">Se a pesquisa é uma passagem superficial ou excluída.</span><span class="sxs-lookup"><span data-stu-id="87d92-110">Whether the search is a shallow or soft-deleted traversal.</span></span> <span data-ttu-id="87d92-111">É necessário especificar isso.</span><span class="sxs-lookup"><span data-stu-id="87d92-111">Specifying this is required.</span></span> <span data-ttu-id="87d92-112">Observe que uma passagem excluída combinada com uma restrição de pesquisa resultará em zero itens retornados, mesmo se houver itens que correspondam aos critérios de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="87d92-112">Note that a soft-deleted traversal combined with a search restriction will result in zero items returned, even if there are items that match the search criteria.</span></span>
    
- <span data-ttu-id="87d92-113">A forma de resposta de itens.</span><span class="sxs-lookup"><span data-stu-id="87d92-113">The response shape of items.</span></span> <span data-ttu-id="87d92-114">Isso identifica as propriedades que são retornadas na resposta.</span><span class="sxs-lookup"><span data-stu-id="87d92-114">This identifies the properties that are returned in the response.</span></span> <span data-ttu-id="87d92-115">É necessário especificar isso.</span><span class="sxs-lookup"><span data-stu-id="87d92-115">Specifying this is required.</span></span>
    
- <span data-ttu-id="87d92-116">As pastas do qual efetuar a pesquisa.</span><span class="sxs-lookup"><span data-stu-id="87d92-116">The folders from which to perform the search.</span></span> <span data-ttu-id="87d92-117">É necessário especificar isso.</span><span class="sxs-lookup"><span data-stu-id="87d92-117">Specifying this is required.</span></span>
    
- <span data-ttu-id="87d92-118">Os tipos de mecanismo e modo de exibição de paginação para retornar exibir dados nas páginas.</span><span class="sxs-lookup"><span data-stu-id="87d92-118">The paging mechanism and view types for returning view data in pages.</span></span> <span data-ttu-id="87d92-119">Especificar isso é opcional.</span><span class="sxs-lookup"><span data-stu-id="87d92-119">Specifying this is optional.</span></span>
    
- <span data-ttu-id="87d92-120">Opções para agrupar e classificar os itens que são retornados.</span><span class="sxs-lookup"><span data-stu-id="87d92-120">Options for grouping and sorting the items that are returned.</span></span> <span data-ttu-id="87d92-121">Especificar isso é opcional.</span><span class="sxs-lookup"><span data-stu-id="87d92-121">Specifying this is optional.</span></span>
    
- <span data-ttu-id="87d92-122">Restrições de pesquisa ou cadeias de caracteres de sintaxe de consulta avançada (AQS) para filtrar os itens que são retornados.</span><span class="sxs-lookup"><span data-stu-id="87d92-122">Search restrictions or Advanced Query Syntax (AQS) strings for filtering the items that are returned.</span></span> <span data-ttu-id="87d92-123">Para obter mais informações sobre como usar o AQS para pesquisas de índice de conteúdo, consulte [QueryString (String)](querystring-string.md).</span><span class="sxs-lookup"><span data-stu-id="87d92-123">For more information about using AQS for content index searches, see [QueryString (String)](querystring-string.md).</span></span> <span data-ttu-id="87d92-124">Especificar isso é opcional.</span><span class="sxs-lookup"><span data-stu-id="87d92-124">Specifying this is optional.</span></span>
    
- <span data-ttu-id="87d92-125">A ordem de classificação para os itens retornados na resposta.</span><span class="sxs-lookup"><span data-stu-id="87d92-125">The sort order for items returned in the response.</span></span> <span data-ttu-id="87d92-126">Especificar isso é opcional.</span><span class="sxs-lookup"><span data-stu-id="87d92-126">Specifying this is optional.</span></span>
    
<span data-ttu-id="87d92-127">A operação **FindItem** retorna apenas os primeiros 512 bytes de qualquer propriedade transmissíveis.</span><span class="sxs-lookup"><span data-stu-id="87d92-127">The **FindItem** operation returns only the first 512 bytes of any streamable property.</span></span> <span data-ttu-id="87d92-128">Para Unicode, ele retorna os primeiros 255 caracteres, usando uma cadeia de caracteres Unicode terminada em nulo.</span><span class="sxs-lookup"><span data-stu-id="87d92-128">For Unicode, it returns the first 255 characters by using a null-terminated Unicode string.</span></span> <span data-ttu-id="87d92-129">Ele não retorna qualquer um dos formatos de corpo de mensagem ou as listas de destinatário.</span><span class="sxs-lookup"><span data-stu-id="87d92-129">It does not return any of the message body formats or the recipient lists.</span></span> <span data-ttu-id="87d92-130">**FindItem** retornará um destinatário resumo.</span><span class="sxs-lookup"><span data-stu-id="87d92-130">**FindItem** will return a recipient summary.</span></span> <span data-ttu-id="87d92-131">Você pode usar a [operação GetItem](getitem-operation.md) para obter os detalhes de um item.</span><span class="sxs-lookup"><span data-stu-id="87d92-131">You can use the [GetItem operation](getitem-operation.md) to get the details of an item.</span></span> 
  
 <span data-ttu-id="87d92-132">**FindItem** retorna somente o elemento de [nome (EmailAddressType)](name-emailaddresstype.md) e não retorna o elemento [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) no elemento de [caixa de correio](mailbox.md) para os seguintes campos:</span><span class="sxs-lookup"><span data-stu-id="87d92-132">**FindItem** returns only the [Name (EmailAddressType)](name-emailaddresstype.md) element and does not return the [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) element in the [Mailbox](mailbox.md) element for the following fields:</span></span> 
  
- <span data-ttu-id="87d92-133">Campo [de](from.md) mensagens</span><span class="sxs-lookup"><span data-stu-id="87d92-133">The [From](from.md) field for messages</span></span> 
    
- <span data-ttu-id="87d92-134">Campo de [destinatário](sender.md) para mensagens</span><span class="sxs-lookup"><span data-stu-id="87d92-134">The [Sender](sender.md) field for messages</span></span> 
    
- <span data-ttu-id="87d92-135">O campo [Organizador](organizer.md) para itens de calendário</span><span class="sxs-lookup"><span data-stu-id="87d92-135">The [Organizer](organizer.md) field for calendar items</span></span> 
    
> [!NOTE]
> <span data-ttu-id="87d92-136">A operação **FindItem** pode retornar resultados em um elemento de [exibição de calendário](calendarview.md) .</span><span class="sxs-lookup"><span data-stu-id="87d92-136">The **FindItem** operation can return results in a [CalendarView](calendarview.md) element.</span></span> <span data-ttu-id="87d92-137">O elemento **CalendarView** retorna todas as ocorrências de reuniões recorrentes e de itens de calendário único.</span><span class="sxs-lookup"><span data-stu-id="87d92-137">The **CalendarView** element returns single calendar items and all occurrences of recurring meetings.</span></span> <span data-ttu-id="87d92-138">Se um elemento de **exibição de calendário** não for usado, itens de calendário único e itens de calendário mestre recorrentes são retornadas.</span><span class="sxs-lookup"><span data-stu-id="87d92-138">If a **CalendarView** element is not used, single calendar items and recurring master calendar items are returned.</span></span> <span data-ttu-id="87d92-139">Se um elemento de **exibição de calendário** não for usado, as ocorrências devem ser expandidas do mestre recorrente.</span><span class="sxs-lookup"><span data-stu-id="87d92-139">The occurrences must be expanded from the recurring master if a **CalendarView** element is not used.</span></span> 
  
<span data-ttu-id="87d92-140">A operação **FindItem** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="87d92-140">The **FindItem** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
<span data-ttu-id="87d92-141">**Tabela 1. Cabeçalhos SOAP FindItem operação**</span><span class="sxs-lookup"><span data-stu-id="87d92-141">**Table 1. FindItem operation SOAP headers**</span></span>

|<span data-ttu-id="87d92-142">**Header**</span><span class="sxs-lookup"><span data-stu-id="87d92-142">**Header**</span></span>|<span data-ttu-id="87d92-143">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="87d92-143">**Element**</span></span>|<span data-ttu-id="87d92-144">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="87d92-144">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="87d92-145">**DateTimePrecision**</span><span class="sxs-lookup"><span data-stu-id="87d92-145">**DateTimePrecision**</span></span> <br/> |[<span data-ttu-id="87d92-146">DateTimePrecision</span><span class="sxs-lookup"><span data-stu-id="87d92-146">DateTimePrecision</span></span>](datetimeprecision.md) <br/> |<span data-ttu-id="87d92-147">Especifica a resolução dos valores de data/hora nas respostas do servidor, em segundos ou em milissegundos.</span><span class="sxs-lookup"><span data-stu-id="87d92-147">Specifies the resolution of data/time values in responses from the server, either in seconds or in milliseconds.</span></span> <span data-ttu-id="87d92-148">Isso é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="87d92-148">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="87d92-149">**Representação**</span><span class="sxs-lookup"><span data-stu-id="87d92-149">**Impersonation**</span></span> <br/> |[<span data-ttu-id="87d92-150">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="87d92-150">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="87d92-151">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="87d92-151">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="87d92-152">Isso é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="87d92-152">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="87d92-153">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="87d92-153">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="87d92-154">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="87d92-154">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="87d92-155">Identifica a cultura RFC3066 a ser usado para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="87d92-155">Identifies the RFC3066 culture to be used to access the mailbox.</span></span> <span data-ttu-id="87d92-156">Isso é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="87d92-156">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="87d92-157">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="87d92-157">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="87d92-158">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="87d92-158">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="87d92-159">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="87d92-159">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="87d92-160">Isso é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="87d92-160">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="87d92-161">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="87d92-161">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="87d92-162">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="87d92-162">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="87d92-163">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="87d92-163">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="87d92-164">Isso é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="87d92-164">This is applicable to a response.</span></span>  <br/> |
|<span data-ttu-id="87d92-165">**TimeZoneContext**</span><span class="sxs-lookup"><span data-stu-id="87d92-165">**TimeZoneContext**</span></span> <br/> |[<span data-ttu-id="87d92-166">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="87d92-166">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="87d92-167">Identifica o fuso horário a ser usado para todas as respostas do servidor.</span><span class="sxs-lookup"><span data-stu-id="87d92-167">Identifies the time zone to be used for all responses from the server.</span></span> <span data-ttu-id="87d92-168">Isso é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="87d92-168">This is applicable to a request.</span></span>  <br/> |
   
## <a name="finditem-operation-request-example"></a><span data-ttu-id="87d92-169">Exemplo de solicitação de operação FindItem</span><span class="sxs-lookup"><span data-stu-id="87d92-169">FindItem operation request example</span></span>

<span data-ttu-id="87d92-170">O exemplo a seguir de uma solicitação de **FindItem** mostra como obter o identificador do item que é definido pela enumeração **IdOnly** do elemento [BaseShape](baseshape.md) para itens que estão localizados na pasta Itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="87d92-170">The following example of a **FindItem** request shows how to obtain the item identifier that is defined by the **IdOnly** enumeration of the [BaseShape](baseshape.md) element for items that are found in the Deleted Items folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
              Traversal="Shallow">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
      </ItemShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="deleteditems"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="87d92-171">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="87d92-171">The following elements are used in the request:</span></span> 
  
- [<span data-ttu-id="87d92-172">FindItem</span><span class="sxs-lookup"><span data-stu-id="87d92-172">FindItem</span></span>](finditem.md)
    
- [<span data-ttu-id="87d92-173">ItemShape</span><span class="sxs-lookup"><span data-stu-id="87d92-173">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="87d92-174">BaseShape</span><span class="sxs-lookup"><span data-stu-id="87d92-174">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="87d92-175">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="87d92-175">ParentFolderIds</span></span>](parentfolderids.md)
    
- [<span data-ttu-id="87d92-176">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="87d92-176">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
<span data-ttu-id="87d92-177">Para obter mais opções para uma mensagem de solicitação **FindItem** , explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="87d92-177">For more options for a **FindItem** request message, explore the schema hierarchy.</span></span> <span data-ttu-id="87d92-178">Inicie o elemento [FindItem](finditem.md) .</span><span class="sxs-lookup"><span data-stu-id="87d92-178">Start at the [FindItem](finditem.md) element.</span></span> 
  
## <a name="successful-finditem-operation-response"></a><span data-ttu-id="87d92-179">Resposta de operação FindItem bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="87d92-179">Successful FindItem operation response</span></span>

<span data-ttu-id="87d92-180">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="87d92-180">The following example shows a successful response to the **FindItem** request.</span></span> 
  
<span data-ttu-id="87d92-181">Elementos de [mensagem](message-ex15websvcsotherref.md) representam as mensagens de email e outros itens que não são fortemente tipados pelo esquema do EWS.</span><span class="sxs-lookup"><span data-stu-id="87d92-181">[Message](message-ex15websvcsotherref.md) elements represent email messages and all other items that are not strongly typed by the EWS schema.</span></span> <span data-ttu-id="87d92-182">Itens como IPM. Compartilhamento e IPM.InfoPath são retornados como elementos da [mensagem](message-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="87d92-182">Items such as IPM.Sharing and IPM.InfoPath are returned as [Message](message-ex15websvcsotherref.md) elements.</span></span> <span data-ttu-id="87d92-183">Exchange não retorna o elemento do [Item](item.md) base nas respostas.</span><span class="sxs-lookup"><span data-stu-id="87d92-183">Exchange does not return the base [Item](item.md) element in responses.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder TotalItemsInView="10" IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AS4AUn=" ChangeKey="fsVU4==" />
              </t:Message>
              <t:Message>
                <t:ItemId Id="AS4AUM=" ChangeKey="fsVUA==" />
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </FindItemResponse>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="87d92-184">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="87d92-184">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="87d92-185">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="87d92-185">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="87d92-186">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="87d92-186">FindItemResponse</span></span>](finditemresponse.md)
    
- [<span data-ttu-id="87d92-187">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="87d92-187">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="87d92-188">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="87d92-188">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
    
- [<span data-ttu-id="87d92-189">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="87d92-189">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="87d92-190">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="87d92-190">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md)
    
- [<span data-ttu-id="87d92-191">Items</span><span class="sxs-lookup"><span data-stu-id="87d92-191">Items</span></span>](items.md)
    
- [<span data-ttu-id="87d92-192">Mensagem</span><span class="sxs-lookup"><span data-stu-id="87d92-192">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="87d92-193">ItemId</span><span class="sxs-lookup"><span data-stu-id="87d92-193">ItemId</span></span>](itemid.md)
    
<span data-ttu-id="87d92-194">Para obter mais opções para uma mensagem de resposta **FindItem** , explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="87d92-194">For more options for a **FindItem** response message, explore the schema hierarchy.</span></span> <span data-ttu-id="87d92-195">Inicie o elemento [FindItemResponse](finditemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="87d92-195">Start at the [FindItemResponse](finditemresponse.md) element.</span></span> 
  
## <a name="finditem-operation-error-response"></a><span data-ttu-id="87d92-196">Resposta de erro de operação FindItem</span><span class="sxs-lookup"><span data-stu-id="87d92-196">FindItem operation error response</span></span>

<span data-ttu-id="87d92-197">O exemplo a seguir mostra uma resposta de erro a uma solicitação de **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="87d92-197">The following example shows an error response to a **FindItem** request.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </FindItemResponse>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="87d92-198">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="87d92-198">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="87d92-199">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="87d92-199">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="87d92-200">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="87d92-200">FindItemResponse</span></span>](finditemresponse.md)
    
- [<span data-ttu-id="87d92-201">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="87d92-201">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="87d92-202">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="87d92-202">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
    
- [<span data-ttu-id="87d92-203">MessageText</span><span class="sxs-lookup"><span data-stu-id="87d92-203">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="87d92-204">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="87d92-204">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="87d92-205">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="87d92-205">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="87d92-206">Para obter mais opções para uma mensagem de resposta de erro **FindItem** , explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="87d92-206">For more options for a **FindItem** error response message, explore the schema hierarchy.</span></span> <span data-ttu-id="87d92-207">Inicie o elemento [FindItemResponse](finditemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="87d92-207">Start at the [FindItemResponse](finditemresponse.md) element.</span></span> 
  
## <a name="version-differences"></a><span data-ttu-id="87d92-208">Diferenças de versão</span><span class="sxs-lookup"><span data-stu-id="87d92-208">Version differences</span></span>

<span data-ttu-id="87d92-209">Versões do Exchange, começando com a versão principal 15 e terminando com compilação 15.0.898.11 retornar um valor de ErrorInvalidOperation no elemento [ResponseCode](responsecode.md) quando a operação **FindItem** é usada para pesquisar várias pastas em uma caixa de correio de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="87d92-209">Versions of Exchange starting with major version 15 and ending with build 15.0.898.11 return an ErrorInvalidOperation value in the [ResponseCode](responsecode.md) element when the **FindItem** operation is used to search multiple folders in an archive mailbox.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="87d92-210">Confira também</span><span class="sxs-lookup"><span data-stu-id="87d92-210">See also</span></span>

- [<span data-ttu-id="87d92-211">Localizando itens</span><span class="sxs-lookup"><span data-stu-id="87d92-211">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)
    
- [<span data-ttu-id="87d92-212">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="87d92-212">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
    
- <span data-ttu-id="87d92-213">**FindItemType**</span><span class="sxs-lookup"><span data-stu-id="87d92-213">**FindItemType**</span></span>
    

