---
title: Operação RemoveContactFromImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 28ec96c3-45af-48ff-9f17-718a527dc0ad
description: Encontre informações sobre a operação do EWS do RemoveContactFromImList.
ms.openlocfilehash: 8b3d83a0b53bad169d9f3478540e5087901f3a12
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458464"
---
# <a name="removecontactfromimlist-operation"></a><span data-ttu-id="a5869-103">Operação RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="a5869-103">RemoveContactFromImList operation</span></span>

<span data-ttu-id="a5869-104">Encontre informações sobre a operação do EWS do **RemoveContactFromImList** .</span><span class="sxs-lookup"><span data-stu-id="a5869-104">Find information about the **RemoveContactFromImList** EWS operation.</span></span> 
  
<span data-ttu-id="a5869-105">A operação **RemoveContactFromImList** remove contatos da lista de IM (mensagens instantâneas) do Lync quando o Lync usa o Exchange para o repositório de contatos.</span><span class="sxs-lookup"><span data-stu-id="a5869-105">The **RemoveContactFromImList** operation removes contacts from the Lync instant messaging (IM) list when Lync uses Exchange for the contact store.</span></span> 
  
<span data-ttu-id="a5869-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a5869-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-removecontactfromimlist-operation"></a><span data-ttu-id="a5869-107">Usando a operação RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="a5869-107">Using the RemoveContactFromImList operation</span></span>

<span data-ttu-id="a5869-108">A operação **RemoveContactFromImList** aceita um único argumento que identifica um contato a ser removido da lista de contatos do Lync armazenado em um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="a5869-108">The **RemoveContactFromImList** operation accepts a single argument that identifies a contact to remove from the Lync contact list stored on an Exchange server.</span></span> <span data-ttu-id="a5869-109">A lista de contatos que esta operação direciona é chamada **contatos do Lync** no Outlook 2013.</span><span class="sxs-lookup"><span data-stu-id="a5869-109">The list of contacts that this operation targets is called **Lync Contacts** in Outlook 2013.</span></span> 
  
> [!CAUTION]
> <span data-ttu-id="a5869-110">Não use a [Operação DeleteItem](deleteitem-operation.md) para remover contatos de uma lista de contatos.</span><span class="sxs-lookup"><span data-stu-id="a5869-110">Do not use the [DeleteItem operation](deleteitem-operation.md) to remove contacts from a contact list.</span></span> <span data-ttu-id="a5869-111">É possível que o processamento adicional no servidor tenha que ocorrer para dar suporte à remoção de um contato da lista de **contatos do Lync** .</span><span class="sxs-lookup"><span data-stu-id="a5869-111">Additional server-side processing might have to occur to support removing a contact from the **Lync Contacts** list.</span></span> <span data-ttu-id="a5869-112">Observe que a lista de **contatos do Lync** é o equivalente conceitual da pasta de caixa de correio padrão do **Lync Contacts** .</span><span class="sxs-lookup"><span data-stu-id="a5869-112">Note that the **Lync Contacts** list is the conceptual equivalent of the default **Lync Contacts** mailbox folder.</span></span> 
  
### <a name="removecontactfromimlist-operation-soap-headers"></a><span data-ttu-id="a5869-113">Cabeçalhos SOAP de operação RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="a5869-113">RemoveContactFromImList operation SOAP headers</span></span>

<span data-ttu-id="a5869-114">A operação **RemoveContactFromImList** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="a5869-114">The **RemoveContactFromImList** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="a5869-115">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="a5869-115">**Header name**</span></span>|<span data-ttu-id="a5869-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a5869-116">**Element**</span></span>|<span data-ttu-id="a5869-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a5869-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a5869-118">**Representação**</span><span class="sxs-lookup"><span data-stu-id="a5869-118">**Impersonation**</span></span> <br/> |[<span data-ttu-id="a5869-119">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="a5869-119">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="a5869-120">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="a5869-120">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="a5869-121">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5869-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="a5869-122">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="a5869-122">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="a5869-123">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="a5869-123">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="a5869-124">Identifica a cultura, conforme definido na RFC 3066, "marcas de identificação de idiomas", a ser usado para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="a5869-124">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="a5869-125">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5869-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="a5869-126">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="a5869-126">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="a5869-127">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="a5869-127">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="a5869-128">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="a5869-128">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="a5869-129">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5869-129">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="a5869-130">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="a5869-130">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="a5869-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="a5869-131">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="a5869-132">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="a5869-132">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="a5869-133">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="a5869-133">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="removecontactfromimlist-operation-request-example-remove-a-contact-from-the-lync-contacts-list"></a><span data-ttu-id="a5869-134">Exemplo de solicitação de operação RemoveContactFromImList: remover um contato da lista de contatos do Lync</span><span class="sxs-lookup"><span data-stu-id="a5869-134">RemoveContactFromImList operation request example: Remove a contact from the Lync Contacts list</span></span>

<span data-ttu-id="a5869-135">O exemplo a seguir de uma solicitação de operação do **RemoveContactFromImList** mostra como remover um contato da lista de **contatos do Lync** .</span><span class="sxs-lookup"><span data-stu-id="a5869-135">The following example of a **RemoveContactFromImList** operation request shows how to remove a contact from the **Lync Contacts** list.</span></span> <span data-ttu-id="a5869-136">A operação **RemoveContactFromImList** aceita um único identificador de contato exclusivo para identificar o contato removido da lista de **contatos do Lync** .</span><span class="sxs-lookup"><span data-stu-id="a5869-136">The **RemoveContactFromImList** operation accepts a single unique contact identifier to identify the contact that is removed from the **Lync Contacts** list.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="a5869-137">Todos os identificadores de item e as chaves de alteração deste artigo foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a5869-137">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
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

<span data-ttu-id="a5869-138">Os seguintes elementos são usados na solicitação de corpo SOAP:</span><span class="sxs-lookup"><span data-stu-id="a5869-138">The following elements are used in the request SOAP body:</span></span>
  
- [<span data-ttu-id="a5869-139">RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="a5869-139">RemoveContactFromImList</span></span>](removecontactfromimlist.md)
    
- [<span data-ttu-id="a5869-140">ContactID</span><span class="sxs-lookup"><span data-stu-id="a5869-140">ContactId</span></span>](contactid.md)
    
## <a name="successful-removecontactfromimlist-operation-response"></a><span data-ttu-id="a5869-141">Resposta de operação RemoveContactFromImList bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="a5869-141">Successful RemoveContactFromImList operation response</span></span>

<span data-ttu-id="a5869-142">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação do **RemoveContactFromImList** para remover um contato da lista de **contatos do Lync** .</span><span class="sxs-lookup"><span data-stu-id="a5869-142">The following example shows a successful response to a **RemoveContactFromImList** operation request to remove a contact from the **Lync Contacts** list.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveContactFromImListResponse ResponseClass="Success" 
                                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveContactFromImListResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="a5869-143">Os seguintes elementos são usados no corpo SOAP de resposta:</span><span class="sxs-lookup"><span data-stu-id="a5869-143">The following elements are used in the response SOAP body:</span></span>
  
- [<span data-ttu-id="a5869-144">RemoveContactFromImListResponse</span><span class="sxs-lookup"><span data-stu-id="a5869-144">RemoveContactFromImListResponse</span></span>](removecontactfromimlistresponse.md)
    
- [<span data-ttu-id="a5869-145">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a5869-145">ResponseCode</span></span>](responsecode.md)
    
## <a name="removecontactfromimlist-operation-error-response"></a><span data-ttu-id="a5869-146">Resposta de erro de operação RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="a5869-146">RemoveContactFromImList operation error response</span></span>

<span data-ttu-id="a5869-147">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **RemoveContactFromImList** .</span><span class="sxs-lookup"><span data-stu-id="a5869-147">The following example shows an error response to a **RemoveContactFromImList** operation request.</span></span> <span data-ttu-id="a5869-148">Esta é uma resposta a uma solicitação para remover um contato da lista de **contatos do Lync** quando o contato não existe mais na lista.</span><span class="sxs-lookup"><span data-stu-id="a5869-148">This is a response to a request to remove a contact from the **Lync Contacts** list when the contact no longer exists in the list.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveContactFromImListResponse ResponseClass="Error" 
                                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified object was not found in the store.</MessageText>
         <ResponseCode>ErrorItemNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveContactFromImListResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="a5869-149">Os seguintes elementos são usados no corpo SOAP de resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="a5869-149">The following elements are used in the error response SOAP body:</span></span>
  
- [<span data-ttu-id="a5869-150">RemoveContactFromImListResponse</span><span class="sxs-lookup"><span data-stu-id="a5869-150">RemoveContactFromImListResponse</span></span>](removecontactfromimlistresponse.md)
    
- [<span data-ttu-id="a5869-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="a5869-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="a5869-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a5869-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a5869-153">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="a5869-153">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="a5869-154">Também consulte</span><span class="sxs-lookup"><span data-stu-id="a5869-154">See also</span></span>

- [<span data-ttu-id="a5869-155">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a5869-155">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="a5869-156">Operação GetImItemList</span><span class="sxs-lookup"><span data-stu-id="a5869-156">GetImItemList operation</span></span>](getimitemlist-operation.md)
    

