---
title: Operação RemoveContactFromImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 28ec96c3-45af-48ff-9f17-718a527dc0ad
description: Encontre informações sobre o EWS RemoveContactFromImList operação.
ms.openlocfilehash: 036b295a84e86ad74c467572cc52fdf6bbae5191
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825080"
---
# <a name="removecontactfromimlist-operation"></a><span data-ttu-id="5c987-103">Operação RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="5c987-103">RemoveContactFromImList operation</span></span>

<span data-ttu-id="5c987-104">Encontre informações sobre a operação de EWS **RemoveContactFromImList** .</span><span class="sxs-lookup"><span data-stu-id="5c987-104">Find information about the **RemoveContactFromImList** EWS operation.</span></span> 
  
<span data-ttu-id="5c987-105">A operação **RemoveContactFromImList** remove contatos da lista de mensagens instantâneas (IM) de Lync quando o Lync usa o Exchange para o armazenamento de contato.</span><span class="sxs-lookup"><span data-stu-id="5c987-105">The **RemoveContactFromImList** operation removes contacts from the Lync instant messaging (IM) list when Lync uses Exchange for the contact store.</span></span> 
  
<span data-ttu-id="5c987-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5c987-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-removecontactfromimlist-operation"></a><span data-ttu-id="5c987-107">Usando a operação RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="5c987-107">Using the RemoveContactFromImList operation</span></span>

<span data-ttu-id="5c987-108">A operação **RemoveContactFromImList** aceita um argumento único que identifica um contato para remover da lista de contatos Lync armazenada em um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c987-108">The **RemoveContactFromImList** operation accepts a single argument that identifies a contact to remove from the Lync contact list stored on an Exchange server.</span></span> <span data-ttu-id="5c987-109">A lista de contatos que destinos essa operação é chamado de **Contatos do Lync** no Outlook 2013.</span><span class="sxs-lookup"><span data-stu-id="5c987-109">The list of contacts that this operation targets is called **Lync Contacts** in Outlook 2013.</span></span> 
  
> [!CAUTION]
> <span data-ttu-id="5c987-110">Não use a [operação DeleteItem](deleteitem-operation.md) para remover contatos de uma lista de contatos.</span><span class="sxs-lookup"><span data-stu-id="5c987-110">Do not use the [DeleteItem operation](deleteitem-operation.md) to remove contacts from a contact list.</span></span> <span data-ttu-id="5c987-111">Processamento do lado do servidor adicionais talvez seja necessário ocorrem para oferecer suporte à remoção de um contato da lista de **Contatos do Lync** .</span><span class="sxs-lookup"><span data-stu-id="5c987-111">Additional server-side processing might have to occur to support removing a contact from the **Lync Contacts** list.</span></span> <span data-ttu-id="5c987-112">Observe que a lista de **Contatos do Lync** é o equivalente conceitual da pasta padrão **Contatos do Lync** da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="5c987-112">Note that the **Lync Contacts** list is the conceptual equivalent of the default **Lync Contacts** mailbox folder.</span></span> 
  
### <a name="removecontactfromimlist-operation-soap-headers"></a><span data-ttu-id="5c987-113">Cabeçalhos SOAP RemoveContactFromImList operação</span><span class="sxs-lookup"><span data-stu-id="5c987-113">RemoveContactFromImList operation SOAP headers</span></span>

<span data-ttu-id="5c987-114">A operação **RemoveContactFromImList** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="5c987-114">The **RemoveContactFromImList** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="5c987-115">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="5c987-115">**Header name**</span></span>|<span data-ttu-id="5c987-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5c987-116">**Element**</span></span>|<span data-ttu-id="5c987-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5c987-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="5c987-118">**Representação**</span><span class="sxs-lookup"><span data-stu-id="5c987-118">**Impersonation**</span></span> <br/> |[<span data-ttu-id="5c987-119">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="5c987-119">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="5c987-120">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="5c987-120">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="5c987-121">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c987-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="5c987-122">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="5c987-122">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="5c987-123">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="5c987-123">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="5c987-124">Identifica a cultura, conforme definido no RFC 3066, "Marcas para a identificação de idiomas", que será usada para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="5c987-124">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="5c987-125">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c987-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="5c987-126">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="5c987-126">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="5c987-127">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="5c987-127">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="5c987-128">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="5c987-128">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="5c987-129">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c987-129">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="5c987-130">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="5c987-130">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="5c987-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5c987-131">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="5c987-132">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="5c987-132">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="5c987-133">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="5c987-133">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="removecontactfromimlist-operation-request-example-remove-a-contact-from-the-lync-contacts-list"></a><span data-ttu-id="5c987-134">Exemplo de solicitação de operação RemoveContactFromImList: remover um contato da lista Contatos do Lync</span><span class="sxs-lookup"><span data-stu-id="5c987-134">RemoveContactFromImList operation request example: Remove a contact from the Lync Contacts list</span></span>

<span data-ttu-id="5c987-135">O exemplo a seguir de uma solicitação de operação **RemoveContactFromImList** mostra como remover um contato da lista **Contatos do Lync** .</span><span class="sxs-lookup"><span data-stu-id="5c987-135">The following example of a **RemoveContactFromImList** operation request shows how to remove a contact from the **Lync Contacts** list.</span></span> <span data-ttu-id="5c987-136">A operação **RemoveContactFromImList** aceita um único identificador exclusivo de contato para identificar o contato que é removido da lista de **Contatos do Lync** .</span><span class="sxs-lookup"><span data-stu-id="5c987-136">The **RemoveContactFromImList** operation accepts a single unique contact identifier to identify the contact that is removed from the **Lync Contacts** list.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="5c987-137">Todos os identificadores de itens e teclas de alteração neste artigo foram diminuídas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5c987-137">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
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
      <m:RemoveContactFromImList>
         <m:ContactId Id=""/>
      </m:RemoveContactFromImList>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="5c987-138">Os seguintes elementos são usados na solicitação de corpo SOAP:</span><span class="sxs-lookup"><span data-stu-id="5c987-138">The following elements are used in the request SOAP body:</span></span>
  
- [<span data-ttu-id="5c987-139">RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="5c987-139">RemoveContactFromImList</span></span>](removecontactfromimlist.md)
    
- [<span data-ttu-id="5c987-140">ID de contato</span><span class="sxs-lookup"><span data-stu-id="5c987-140">ContactId</span></span>](contactid.md)
    
## <a name="successful-removecontactfromimlist-operation-response"></a><span data-ttu-id="5c987-141">Resposta de operação RemoveContactFromImList bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="5c987-141">Successful RemoveContactFromImList operation response</span></span>

<span data-ttu-id="5c987-142">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **RemoveContactFromImList** para remover um contato da lista de **Contatos do Lync** .</span><span class="sxs-lookup"><span data-stu-id="5c987-142">The following example shows a successful response to a **RemoveContactFromImList** operation request to remove a contact from the **Lync Contacts** list.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveContactFromImListResponse ResponseClass="Success" 
                                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveContactFromImListResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="5c987-143">Os seguintes elementos são usados no corpo SOAP de resposta:</span><span class="sxs-lookup"><span data-stu-id="5c987-143">The following elements are used in the response SOAP body:</span></span>
  
- [<span data-ttu-id="5c987-144">RemoveContactFromImListResponse</span><span class="sxs-lookup"><span data-stu-id="5c987-144">RemoveContactFromImListResponse</span></span>](removecontactfromimlistresponse.md)
    
- [<span data-ttu-id="5c987-145">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5c987-145">ResponseCode</span></span>](responsecode.md)
    
## <a name="removecontactfromimlist-operation-error-response"></a><span data-ttu-id="5c987-146">Resposta de erro de operação RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="5c987-146">RemoveContactFromImList operation error response</span></span>

<span data-ttu-id="5c987-147">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **RemoveContactFromImList** .</span><span class="sxs-lookup"><span data-stu-id="5c987-147">The following example shows an error response to a **RemoveContactFromImList** operation request.</span></span> <span data-ttu-id="5c987-148">Esta é uma resposta a uma solicitação para remover um contato da lista **Contatos do Lync** , quando o contato não existe mais na lista.</span><span class="sxs-lookup"><span data-stu-id="5c987-148">This is a response to a request to remove a contact from the **Lync Contacts** list when the contact no longer exists in the list.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveContactFromImListResponse ResponseClass="Error" 
                                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified object was not found in the store.</MessageText>
         <ResponseCode>ErrorItemNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveContactFromImListResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="5c987-149">A resposta de erro corpo SOAP são usados os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="5c987-149">The following elements are used in the error response SOAP body:</span></span>
  
- [<span data-ttu-id="5c987-150">RemoveContactFromImListResponse</span><span class="sxs-lookup"><span data-stu-id="5c987-150">RemoveContactFromImListResponse</span></span>](removecontactfromimlistresponse.md)
    
- [<span data-ttu-id="5c987-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="5c987-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="5c987-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5c987-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="5c987-153">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="5c987-153">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="5c987-154">Confira também</span><span class="sxs-lookup"><span data-stu-id="5c987-154">See also</span></span>

- [<span data-ttu-id="5c987-155">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5c987-155">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="5c987-156">Operação GetImItemList</span><span class="sxs-lookup"><span data-stu-id="5c987-156">GetImItemList operation</span></span>](getimitemlist-operation.md)
    

